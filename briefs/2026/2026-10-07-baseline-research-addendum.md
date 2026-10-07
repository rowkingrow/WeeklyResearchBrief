# 首期基线研究补注｜2026-10-07

作者：ChatGPT研究总控。被补充版本为 `15b7abb1d0a2d14089547f797f892fd378e32634` 的 `briefs/2026/2026-10-07-baseline.md`。本补注依据本轮出版社、论文方法/数据声明及官方数据站点核查。原简报与原索引保留其阅读时点，新增信息由本页与配套JSON记录。研究候选属于研究者推论，立项仍由总控决定。

## B15 气旋与腹泻：数据取得条件及代码入口已进一步明确

原条目阅读为摘要级。本轮补读出版社36页接收稿的方法、限制与数据/代码声明。第26页说明资料来自ClimED协作项目，按地区采用不同的空间单位和发病资料；第29–32页描述分地区的双向固定效应、当周与后一周暴露及敏感性分析。第32页明确处理后的疾病—气候时间序列须通过ClimED申请，并经资料提供方批准。

代码声明给出 `https://github.com/linszuyu/tc-diarrhea-multi-region`。本轮GitHub连接实际读取了仓库根目录，返回README.md及code目录；代码运行、复算及疾病样例取得尚未进行。数据状态更新为“已核实申请入口，提供方批准条件明确，样例未取得”；代码状态更新为“论文声明与仓库目录已核实，执行待检验”。

暴露定义改变会影响关联估计的可比性；依据结果选择最强定义，需要额外的留出验证和多重比较考虑。新增疾病研究应预定致害路径与结局，区分发病、门诊、住院和监测报告。病例报告或就诊变化还可能受灾后服务可及性影响。

来源：
- 论文及接收稿：https://doi.org/10.1038/s44304-026-00246-z ；https://www.nature.com/articles/s44304-026-00246-z_reference.pdf
- 数据申请入口（本轮依据论文声明）：https://paulcarlos.quarto.pub/climed/
- 代码目录：https://github.com/linszuyu/tc-diarrhea-multi-region

## B07/B15 疾病问题的直接先例与新的识别要求

“气旋后是否增加健康负担”已有重要先例。Young与Hsiang的Nature 2024论文评估长期死亡效应；Lynch与Shaman的Emerging Infectious Diseases 2023论文分析美国1996–2018年六类水传播疾病，比较风、雨和路径暴露；npj Natural Hazards 2026论文进一步比较亚洲多地区腹泻定义。mBio 2023研究还结合灾后水/牡蛎样本与环境资料考察Ian之后的Vibrio。

新的可检验问题可落在不同洪水来源、暴露路径、恢复服务和病种的区别。海水倒灌与雨洪的判别需要独立暴露证据。遥感淹没图可以描述水体范围，其病原、盐度或感染作用需要相应测量。沿海位置应作为比较设计中的共同背景，地区与季节差异、服务中断和报告过程需明确处理。

来源：
- https://doi.org/10.1038/s41586-024-07945-5 （摘要和相关结果段）
- https://doi.org/10.3201/eid2908.221906 （摘要、方法与讨论）
- https://doi.org/10.1128/mbio.01476-23 （摘要、相关结果和数据声明）

## B09 渔业：年度捕获量与短时生物响应分层

本轮出版社索引返回的引言、方法和限制明确，主分析覆盖1993–2019年，采用物种—EEZ年度序列；温度和净初级生产力极端按年度异常分位数定义。6659序列、1246物种、254区域的规模保留。年度捕获量支持产出/移除异常的分析，生物量与种群变化需要调查证据。年度聚合不足以直接恢复单场气旋数日内的影响或恢复过程。

资料拓展入口为NOAA/SEAMAP独立于商业捕捞的调查。SEAMAP-SA Coastal Trawl Survey提供季节性丰度、生物量和站位、日期、温盐资料；其采样季节2023年开始变化，船舶更换也涉及可比性。数据门户要求先阅读知识产权协议并建立账户。当前核查达到官方方法和门户说明，样例下载及事件前后样本配对均待执行。海洋生物响应、捕捞努力和食物供给分别建立证据。

来源：
- https://doi.org/10.1038/s41467-026-77077-z （出版社搜索索引中的引言、方法与限制；正文直连本轮返回缓存错误）
- https://seamap.org/seamap-sa-coastal-trawl/ （官方方法和Data Availability）
- https://seamap.org/data-portal/ （账户与使用协议）
- https://www.fisheries.noaa.gov/southeast/funding-financial-services/southeast-area-monitoring-and-assessment-program-seamap

原简报曾核实Zenodo版本。本轮该Zenodo直连访问失败，原有版本核查归属原周报，当前未新增样例验证。

## B12 海上风电扩展：直接先例需要前置比较

气旋对风机极端载荷、风场产能恢复及并网系统韧性均有直接研究。本轮新增核查：
- Increasing extreme winds challenge offshore wind energy resilience，Nature Communications，2025-11-04，https://doi.org/10.1038/s41467-025-65105-3 （摘要、部分结果）
- 60 years of typhoon-induced impacts on offshore wind farms: A holistic high-resolution evaluation of resilience，Applied Energy 410 (2026) 127542，https://doi.org/10.1016/j.apenergy.2026.127542 （摘要和Highlights，卷期日期与首次在线日期分列）
- Resilient preventive strategies for offshore wind-integrated power systems against typhoons under decision-dependent uncertainty，Applied Energy 411 (2026) 127608，https://doi.org/10.1016/j.apenergy.2026.127608 （摘要和Highlights）

新问题应比较结构损伤、保护性停机、检修时间、发电可用性与供电服务恢复的证据。居民停电后果还需要电网连接、其他电源及负荷信息。新的海上风电研究资格待判断。

## B14 老龄化：从人口加权推进到服务需求

年龄结构变化可以形成暴露分解，但健康负担或服务不足的判断还需年龄特异风险、医疗依赖或实际服务资料。Nature Communications 2023已有Florida老年人气旋住院差异研究；同年还有美国停电、社会脆弱性和医疗设备依赖的联合分析。因此，老年人口与灾害图的叠加已有近邻研究。

HHS emPOWER公开地图提供按月更新的去标识汇总和历史数据入口，覆盖Medicare人群及电力依赖医疗设备需求。人群包含65岁以上参保者和部分65岁以下残疾参保者，统计口径与全部老年人口不同；公开地图、受限应急规划资料和个人医疗记录分别标识。EAGLE-I的Scientific Data 2024资料描述提供2014–2022年县级15分钟停电与覆盖/质量辅助表。两类资料的实际共同空间/时间覆盖、许可和最小样例仍需核验。县级停电比例与患者所在家庭停电情况之间需要额外假设或验证。

来源：
- https://doi.org/10.1038/s41467-023-37675-7
- https://doi.org/10.1038/s41467-023-38084-6
- https://doi.org/10.1016/j.ijdrr.2023.103844 （摘要）
- https://empowerprogram.hhs.gov/about-empowermap.html
- https://empowerprogram.hhs.gov/de-identified-dataset.html
- https://doi.org/10.1038/s41597-024-03095-5

## B02 灾后遮阴启发的适用时段

B02论文研究九城日常步行遮阴及分布差异，原文未检验灾后道路通行或修缮。总控据此调整研究启发：抢险阶段的路障、设施开放和通行能力应单独定义；树冠热服务问题可设在道路基本恢复后的热季，考察树冠结构、复绿、降温与居民暴露的恢复。后者为待查新假设。

来源：https://doi.org/10.1038/s41467-026-69190-w （摘要及相关引言）。

## 阅读与执行记录

本轮为文献核查与问题重构。疾病论文方法/数据声明已补读；其他来源阅读范围在各项列明。用户批注全文保留当前研究对话，公共补注采用原创学术分析。没有新疾病、树冠、渔业或风电样例计算；新颖性与pilot状态均待评估。原每周任务和发布配置保持。
