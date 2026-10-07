# 定时任务配置与核验

任务名称：近期研究周报。

- 平台：ChatGPT Work Automations，云端定时执行。
- 创建状态：工具返回success=true、is_enabled=true；创建前检查已有任务，未发现同名或相同研究周报。
- 时区：Asia/Singapore。
- 计划：每周一08:00，exact_schedule。
- DTSTART：2026-10-12T08:00:00+08:00。
- 下一次计划运行：2026-10-12 08:00（Asia/Singapore），依据已接受的VEVENT计算；创建响应的next_run_time字段为null。
- 完成通知：执行完成后在本对话通知，并记录实际完成时间。

```ical
BEGIN:VEVENT
DTSTART;TZID=Asia/Singapore:20261012T080000
RRULE:FREQ=WEEKLY;BYDAY=MO;BYHOUR=8;BYMINUTE=0;BYSECOND=0
END:VEVENT
```

定时任务prompt包含研究背景、Ida HOLD经验、仓库与授权边界、主题和期刊、阅读深度、时间判定、去重、数据证据层级、文件路径与通知要求。其正文与[BRIEFING_RULES.md](BRIEFING_RULES.md)的单次执行规则一致。必要背景已写入prompt，不依赖项目上传文件。

外部连接创建前已通过GitHub get_repo、fetch_file等无害读取核实。当前会话已完成仓库写入和文件回读。首次定时运行尚未发生，因此未来运行中的连接状态由每次开始时重新实测；读取成功后重新加载main配置与索引。连接失效或审批阻断时在当前运行交付文件并记录待发布状态。

每次运行保存计划时刻、实际开始、内容完成与发布回读完成时刻。时间窗口固定为计划时刻向前7天，迟到运行保留原窗口。2026-10-12首轮窗口为2026-10-05 08:00至2026-10-12 08:00（Asia/Singapore）；与基线有重叠时依索引去重。
