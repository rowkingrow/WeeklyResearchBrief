# 研究背景与证据边界

更新于2026-10-22。本文件供“近期研究周报”及其独立定时运行使用；现行筛选以config/BRIEFING_RULES.md为准。

## 用户提供的研究条件

用户研究关注极端天气与海上运行，特别是船舶能耗与排放、交通空间重组、多船交互，以及恢复与适应。周报优先帮助掌握核心领域的直接先例、证据边界与近期进展，保留少量有明确连接的拓展阅读。

现行问题结构为：暴露与约束、个体船舶行为、系统空间重组与相遇压力、运行后果、恢复与适应。AIS、遥感、因果推断和深度学习是跨问题的方法/数据标签。健康、城市热风险、树冠、服务可达性等旧拓展主题，仅在与上述主线存在实质连接时纳入，不再按独立热点并列筛选。

以公开资料和可核实的数据/代码入口评估可行性，不因公开论文使用某类数据就假定用户或课题组具备相同资料、许可和合作。私有项目进度、内部任务号和未发表结果不进入本公开仓库。

## 导师已公开的研究主题

[HKU地理系主页](https://geog.hku.hk/b-huang)与[HKU Scholars Hub](https://hub.hku.hk/cris/rp/rp03146)一致列出时空数据分析、卫星影像融合、环境监测和综合空间规划；主页介绍其GTWR相关工作，以及土地利用空间统计、环境监测影像融合和可持续规划空间优化。这些为公开研究主题依据。

[Google Scholar指定页面](https://scholar.google.com/citations?user=UCzVB4MAAAAJ&hl=en)于本轮访问返回内部错误，无法据此完整核对近年发表或引用信息。HKU主页的条目有跨年度重复，同一DOI合并处理。作者归属以姓名、HKU地理系机构及论文原文结合核实，主页列表不被视作逐条完成身份核验。

## 已核实的近年相关成果

| 成果 | 原文核实与日期 | 研究联系与边界 |
|---|---|---|
| Lin等，Addressing urban tree loss and inequality in the USA: the need for targeted policies；Science Bulletin | DOI [10.1016/j.scib.2024.12.024](https://doi.org/10.1016/j.scib.2024.12.024)。出版社网页访问受限；读取格罗宁根大学托管且注明Version of record的[出版社PDF](https://pure.rug.nl/ws/portalfiles/portal/1325762458/Addressing_urban_tree_loss_and_inequality_in_the_USA_the_need_for_targeted_policies.pdf)，类型Short Communication，首次在线2024-12-21，卷期70(8), 1235–1238，2025-04。原文列黄波及HKU地理系。 | 美国470城2011—2021年树冠、人口与社会脆弱性，比较树木项目参与与公平性。关联设计限制政策因果解释。主题衔接城市树木损失与不平等。 |
| Qi、Huang、Webster，Rising Global Elderly Health Inequalities in the Face of Temperature Extremes；Earth’s Future | [出版社原文](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2025EF006000)，Research Article，首次在线2025-07-04，13(7), e2025EF006000。正文核实黄波为通讯作者。 | ERA5、CMIP6、人口和经济资料构造EMRI，讨论年龄与地区不平等。EMRI为风险指标，论文承认横截面流行病学部分的因果局限。与第三篇脆弱群体定义相关。 |
| Cai、Huang、Liu，Fusing Sentinel-1 and Sentinel-2 data with diffusion models for cloud removal；Remote Sensing of Environment | [出版社页面](https://www.sciencedirect.com/science/article/pii/S0034425725004535)，DOI [10.1016/j.rse.2025.115049](https://doi.org/10.1016/j.rse.2025.115049)，331, 115049，卷期2025-12；HKU列明作者与标题，Crossref核对标题、期刊、DOI与卷期。出版社检索摘要可读，首次在线精确日与全文方法仍待补核。 | 摘要描述EDM-CR融合S1/S2进行去云。可为环境监测提供方法线索；灾后变化保真和模型生成结果的独立真值验证需针对任务检验。 |

核验结论对应上述阅读范围。本轮未对导师全部论文、当前在研项目和实际合作条件作完整调查。

## 我们推测的方法适配性

时空统计可用于分层暴露、恢复轨迹和空间异质性；网络与空间规划可用于生活服务可达性；影像融合可辅助多云灾后环境监测。这些属于方法适配推论。具体科学问题仍需真实观测、比较单位、竞争解释和独立贡献支持。

遥感树冠损失与遮阴、地表温度与近地气温、热应激指标与健康结局分别定义。公开论文中的医学合作、商业资料或独有观测未被视为课题组已拥有资源。HPC可用支持计算可行性，数据许可和验证资料仍需逐项确认。

## 研究判断与执行边界

每项新建议先核查关键时段真实观测、比较单位、竞争解释与独立贡献。新颖性未建立时标注待查新。周报中的“支持/修正/挑战/无直接影响”仅对应可公开的一般研究问题，不披露或评判用户未发表的具体主张。文献周报提供线索与证据；科研立项和计算任务另行决定。

## 授权范围

目标为[WeeklyResearchBrief](https://github.com/rowkingrow/WeeklyResearchBrief)，固定main发布。2026-10-07核实为公开仓库，当前连接具有pull/push权限。授权内容为原创简报、文献索引、背景与配置及必要轻量证据。附加仓库、分支、Issue、PR、GitHub Actions和外部服务须按用户授权规则办理；现有仓库要求PR时遵循，合并由用户决定。凭据在官方或私有入口配置。

