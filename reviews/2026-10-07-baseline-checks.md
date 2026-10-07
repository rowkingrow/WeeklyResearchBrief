# 首期基线轻量核验记录

核验日期2026-10-07；资料截止锚定09:20:57（Asia/Singapore）。内容整理完成记录见最终发布回执。本记录覆盖本期原创简报、元数据、索引、背景和配置。

## 仓库与动作

目标rowkingrow/WeeklyResearchBrief真实存在，仓库ID1408089089，public；当前GitHub连接身份rowkingrow，有pull/push权限。get_repo成功；初次contents返回空仓库，main初始未有提交；rulesets返回空数组。使用默认分支写入README后返回提交af80facd4f8a9ca99f4618c681f0d0bad7e138dd，随后fetch_file读回相同内容。分支main已存在，protected=false。可用工具包括create_file、create_tree、create_commit及update_ref。

正式内容以本期文件集提交，提交后回读所有更新文件；实际提交与字节结果写入独立发布回执。无新增附加分支、Issue、PR或Actions。

## 文献检索与元数据

采用主题检索、出版社追溯、Crossref逐DOI核对及作者数据代码入口。academic-search MCP未暴露，使用网页工具和直接公开REST回退；连通性测试显示PubMed E-utilities、Crossref REST与arXiv API可达。本期PubMed/arXiv未开展完整系统检索。

代表检索式包括“2026 hurricane heat power outage health”“2026 urban tree loss heat inequality”“2026 extreme heat labour health mortality”“2026 marine heatwaves fisheries livelihoods”“2026 flood drinking water”，并对Nature、Science、PNAS和Lancet域名检索。方法论文与导师成果沿准确题名、DOI追溯。检索发现优先在出版社回读；检索摘要的抓取日期未用于纳入判断。

15篇入选、12篇核心窗、3篇回溯、5篇重点；标准化DOI无重复。所有入选题名、DOI、期刊、首次在线日均从出版社页面或元数据核实。Crossref对B11返回429，B15尚未补核Crossref，已按出版社元数据记录。其余已取得Crossref记录未见update-to/updated-by关系。全文补充材料尚未逐项阅读，未执行论文模型复算。

Science、PNAS、Lancet的主题检索质量与可读性不均，本期入选明显偏Nature体系；后续需扩大公共健康、交通与水安全检索。该覆盖限制已在正文披露。

Google Scholar指定页面访问失败，HKU主页和Scholars Hub可读。导师树木论文读取大学托管的出版社正式PDF，首页核实类型Short Communication及首次在线2024-12-21；导师RSE论文取得出版社摘要与Crossref元数据，精确在线日待补核。

## 日期与版本

| 条目 | 首次在线 | Version of record | 核验依据 |
|---|---|---|---|
| B01 | 2026-07-20 | 2026-08-21 | 出版社About this article及citation_online_date；Crossref |
| B02 | 2026-02-10 | 2026-03-18 | 同上 |
| B10 | 2026-05-04 | 2026-07-09 | 同上 |
| B11 | 2026-05-31 | 2026-08-11 | 出版社页面；Crossref请求限流 |

首次在线、卷期、正式版本与更正分字段。上述时间差未被归类为已发布的独立更正。页面日期精度为日，时区未给出；本期无贴近12个月下界的入选条目。其他日期见papers.json。

B03沿出版社及作者页面关联arXiv:2412.08079；B05、B12的预印本关系来自Crossref。版本去重以正式论文为主记录。B12归档概念DOI15012708解析至版本15012709。

## 数据入口与样例

- B02：Zenodo九城数据页可读；香港ZIP在网页下载遇429后，通过公开下载URL读取成功。大小1,588,179字节，SHA256为596e7a85769bef497755572803c50da83fd9f6bf5a6046020a0bd08f8ecb583d。ZIP完整读取，含shp/dbf/shx/prj/cpg；DBF头显示129记录、14字段，字段含Average sh、Cumulative、stpug_eng和人口收入变量；PRJ为Hong Kong 1980 Grid。此为邻里汇总样例，数值分析与地图视觉检查尚未执行。字段缩写的完整含义待对照数据说明。数据下载地址https://zenodo.org/records/17972371/files/Hong%20Kong.zip?download=1。
- B02代码：Slim Shady公开README成功读取。数据页和软件源明确关联。
- B03：GenFocal公开README与Zenodo软件API读取成功；归档文件swirl-dynamics-GenFocal-Stable.zip约19.2MB。权重与训练/输出数据为原文公开声明，本轮未取样和推理。
- B05：Dryad DOI跳转和初次API路径失败，后续公开数据页面成功。目录给出约1.38GB主包与README，R/Python/GEE、i-Tree配置明确。已核实入口，数据样例未取得。
- B09：Zenodo API成功，归档coruubc/CompoundExtremes-v1.0.1.zip约9.6MB，未下载代码包和输入数据。论文摘要写6659条时间序列、方法写6569，正文未引用该总数；进一步复现时须向来源核对。
- B12：Zenodo API成功，解析至10.5281/zenodo.15012709，MATLAB包约208KB。原始电网输入完整性待确认。
- B01：代码仓库页面可读；西班牙日死亡数据需要审批。B13原始停电记录需购买，公开汇总的时间粒度有限。
- B04：CDS ERA5-HEAT入口可读；代码按原文需合理请求。
- B15：阅读停留在摘要与元数据，原始健康数据与代码分享条件待查。

已取得样例仅指B02香港ZIP；读取README、数据目录和API元数据归为“已核实入口”。其余条目状态逐项列于正文及JSON。

## 检查结果与边界

读取检查完成至上述范围；元数据完整性、DOI去重、日期窗口及Markdown相对链接作程序核查。数值核查包含文献数量、窗口分类和香港DBF记录/字段数。论文效应值的原始数据复算尚未执行。字节核查包括香港样例SHA256与正式发布文件回读。视觉检查未进行；本期交付为Markdown与JSON，论文图表和样例地图未作视觉认证。

原始论文HTML、受版权保护PDF及下载的研究数据保留为阅读中间材料；远端本期文件集包含原创评述、元数据、来源链接与轻量核验说明。
