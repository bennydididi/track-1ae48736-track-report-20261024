这个产品帮助海外中小机加工厂的老板和报价员，在客户只提供 2D 工程图询价时，解决读图、估算工序成本并生成可复核报价耗时的问题。

# CNC 2D图纸自动报价：先验证付费，暂不优先做 SEO

研究日：2026-10-24。事实、厂商声明、用户自述与本报告假设分开；“未找到”不代表不存在。只判断软件远程成交，不接机加工订单。

## 一分钟决策

### 钉死的研究对象

| 项目 | 本次固定范围 |
|---|---|
| 谁 | 接外部订单的中小 CNC（计算机数控加工）工厂老板、报价员；先验证收到较多纯图纸询价、已有本厂费率的用户 |
| 场景 | 收到 RFQ（客户询价），只有 2D 图纸，报价员还兼做生产或编程 |
| 输入 | PDF/DWG 工程图＋数量、材料/表面处理要求＋本厂机床、小时费率、成本及加价规则；缺项须追问。**不要求 STEP 等 3D 模型** |
| 输出 | 可逐项修改的材料、装夹、编程、加工、外协和检验成本；数量阶梯价；人工确认后导出对客报价 PDF |
| 单一任务 | **把一份没有 3D 模型的机加工图纸询价，变成报价员能核对并发出的报价。**人工确认属于该任务，不承诺无人审核定价 |
| 初始交付边界【建议】 | 先验证尺寸齐全的常规车削/三轴铣削 PDF；DWG 先由用户导出 PDF。原生 DWG 能力、复杂件覆盖率均待测，不宣传已经支持 |

### 首屏三维决策

| 维度 | 当前判断 | 最关键依据与不足 |
|---|---|---|
| 有没有相关需求 | **有；纯 2D 证据仍薄** | 近期从业者明确抱怨工具要求 STEP、收到的却多是图纸；但只是单帖评论，不能代表整个行业。[原帖](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/) |
| 切口能否独立收费 | **待验证，尚未证明成熟 PMF（产品与市场匹配）** | CloudNC、QuotedPart、QuoteBuddy 已单独标价并声明支持图纸报价；**该输入场景的实际付费客户、续费和可靠性未找到**。标价证明有供给，不等于成交。[CloudNC 公告](https://www.cloudnc.com/news-room/cloudnc-launches-quote-agent-to-help-machine-shops-win-more-work)、[QuotedPart 定价](https://quotedpart.com/pricing)、[QuoteBuddy 定价](https://quotebuddy.therness.com/en/pricing) |
| 是否优先靠 SEO | **暂不优先** | 主任务候选词没有返回正数的记录；日本搜索量全部未返回，不能判断为无需求。国别 SERP 样本均不足完整前十，部分明显跑题。通用报价词的量不归本切口。[搜索量供应商入口](https://api.pxany.com/v1/keyword-volumes)，原始回包快照与最终审计见证据包 |

**行动建议：不进入正式开发/SEO 优先队列，只做有上限的小额付费验证。**阻力是尚未证实的同切口付费、专业报价责任和获客量，不是“已经有竞品”。最能改变决定的证据是：用户在相同图纸上，相比现有工具仍能净省时，并愿意实际付费、复用及续费。

**下一步【拟议，未执行】**：接触 10 家符合范围的工厂，争取 5 家提供脱敏历史图纸与实际成本；同题比较现有解法，再测试至少 3 家支付首月 $99。通过后观察真实新询价使用，到下一计费周期再看续费。数字均为本报告验证门槛，不是市场数据；完整停止条件见后文。

### 五项核实卡

来源材料有既有研究，但**专员五项原分未找到**，不能声称已通过 SOP 的初筛入口。按用户指定材料继续核验，缺口保留；不补造原分。总分及折算放附录。

| 项目（各 1–5） | 专员原分 | 核实后分【研究判断】 | 关键证据/含义 |
|---|---|---:|---|
| 需求真实 | 未找到 | 4 | 有从业者图纸兼容抱怨，也有不需要自动化的反证；非全量调查。[近期讨论](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/) |
| 付费意愿 | 未找到 | 2 | 同任务有明确标价，尚未取得实际付费及留存证据；不借用 ERP/3D 报价客户证明纯 2D PMF。[QuotedPart](https://quotedpart.com/pricing)、[QuoteBuddy](https://quotebuddy.therness.com/en/pricing) |
| 好服务 | 未找到 | 2 | 用户专业，错误工艺、漏外协和漏检验会影响利润；直接竞品仍要求报价员确认。[CloudNC 工作流](https://www.cloudnc.com/news-room/cloudnc-launches-quote-agent-to-help-machine-shops-win-more-work) |
| 小团队做得动 | 未找到 | 2 | 读图能力可采购，但工艺、费率校准与异常处理仍需领域能力；无本团队实测交付证据。[Werk24 能力及价格](https://www.werk24.io/pricing)、[QuoteBuddy 工艺明细](https://quotebuddy.therness.com/en/solutions/turning-milling-quotes) |
| 形态简单 | 未找到 | 2 | 入口可做上传表单，后台涉及毛坯、装夹、批量分摊、外协及人工锁定，不能按普通表单工具估工期。[QuoteBuddy](https://quotebuddy.therness.com/en/solutions/contract-manufacturers) |

按筛选标准，付费项低于 3，**本轮不推荐正式立项**；“未证明有人付费”不写成“无人付费”。

## 判断依据

### 需求存在，但用户要的是净省时和可信报价

**最接近本切口的证据，是图纸输入不被现有工具很好承接；最强反证，是简单件原本很快、复杂件又难放心交给自动工具。**

| 时间、用户和热度 | 原话/核实结果 | 抱怨哪一步；现用工具及付费 |
|---|---|---|
| 2026-08-27；r/Machinists，Hour-Ad-2206；主帖 +2 | “we are currently struggling to achieve the quoting time targets.” 自述约 10 名机加工/编程人员，3 人兼做报价 | 回复说明已用 Excel，仍因工作量不足以完成；正在比较 Toolpath、Uptool、CloudNC、Spanflug，询问约 $400/月是否值得。**这是询价意愿，不是已付款**。[原帖](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/) |
| 同帖，2026-08-27；一位评论者 +1 | “most of the quote stuff I get is drawings.” 同段抱怨很多工具要求 STEP | 直接支持“没有 3D 模型也要报价”的兼容问题；未证明其需要原生 DWG，也未披露为此支付多少钱。该评论关于数据被送往中国的指控**未核实，不采作事实**。[原帖](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/) |
| 同帖，2026-08-27；反对者 +1 | “Either part is simple and you can quote it in less than 5 minutes” | 评论认为复杂件自动报价会错；说明不能按所有小厂都能节约大量工时定价。这是个案，非行业均值。[原帖](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/) |
| 同一发帖者，2026-10-13 回复 +1 | 自述正在用 Lehrling AI，喜欢可改报价工作流，并提到两个月试用 | 支持定制工作流偏好；处于试用，不计首付、更不计续费。[回复所在原帖](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/) |

同日 r/CNC 的 +7 主帖是同一求助的跨版发布，**去重为一个事件**，不是两家工厂。[跨版帖](https://www.reddit.com/r/CNC/comments/1vznqot/hows_your_experience_with_automated_quoting/)。评论总数未找到可稳定核对值，不填数。供应商自荐、朋友转述和历史数据检索推销，不计独立付费证据。

辅助调查：CNCCookbook 称调查了 **100 位受访者**，至少 **40% 的受访者**需要在没有 CAD 模型时估价；页面最后修改为 **2024-03-09**，实际调查年份未找到。这支持“不应强制 3D 输入”，**不等于 40% 的 RFQ 是 PDF，更不证明他们要全自动定价**。该站也销售估算工具，样本非随机。[调查](https://www.cnccookbook.com/job-quote-cost-estimation-survey-results/)

**当前切口的行业平均报价工时、延迟丢单率、AI 准确率：未找到可核实统计。**不沿用厂商“从小时到分钟”等宣传做收益参数。原报告中 3D 模型求助、ERP 实施抱怨和历史资料检索案例，不能补强本切口评分。

### 同任务已有收费供给，成交与续费仍缺证据

**支持继续核验付费，尚不足以通过“成熟对标产品已验证当前切口 PMF”的门槛。**以下为同任务能力声明，均未做软件实测。

| 同任务产品 | 输入→输出与公开价格 | 证明什么；还缺什么 |
|---|---|---|
| CloudNC Quote Agent | 官方 **2026-10-13** 公告：上传 **2D 和/或 3D**，生成工艺、工时及成本供人工确认，导出 PDF；AI 付费使用公告价 **$2.50/零件**，手工工作流免费。[官方公告](https://www.cloudnc.com/news-room/cloudnc-launches-quote-agent-to-help-machine-shops-win-more-work) | 证明独立产品和按次收费设计。当前套餐页不可读取；比较页提及的套餐金额不当一手现价。纯 2D 付费客户数、续费、该独立产品收入/融资：**未找到** |
| QuotedPart | 明确说 PDF 可在无 STEP 时估价并列假设；费率、公式及成本可改，审核后发送。**$199/月/全厂，14 天无卡试用**。[产品](https://quotedpart.com/)、[价格](https://quotedpart.com/pricing) | 最直接的图纸独立报价对标。可线上注册及银行卡订阅；不证明有人完成付款。纯 2D 付费客户数、收入、融资和续费：**未找到**。不采用已过期的 $99 早鸟摘要 |
| QuoteBuddy | 官方工艺页明确支持 PDF/PNG/JPG→车/铣工序、费用明细和报价 PDF；展示提取值供改正。定价页显示 **€149/月含 100 次**、试用 **30 天**，之后免费额度 **3 次/月**。[工艺页](https://quotebuddy.therness.com/en/solutions/turning-milling-quotes)、[价格](https://quotebuddy.therness.com/en/pricing) | 证明还有透明收费、图纸输入和人工复核的供给。实际付费客户数、收入、融资及续费：**未找到**；不将它与另一家同名 Quoter 或 Quotebeam 混淆 |

**原生 DWG→自动机加工定价的同等直接证明：未找到。**不能把“支持 CAD”“能看 DWG”当作已能纯图纸自动报价。CloudNC 仅凭官方发布稿归为同任务供给，不把母公司已有业务的 PMF 转给刚发布的独立产品。

**相关流量：未找到可复核月访问量。**本次 [QuotedPart Similarweb](https://www.similarweb.com/website/quotedpart.com/) 与 [CloudNC Similarweb](https://www.similarweb.com/website/cloudnc.com/) 不可读取；CloudNC 总域名即便有流量，也不能归到纯 2D 报价。厂商价格、融资、网页收录都不是收入。

免费方案并未证实足够好且用户满意；也未找到证据说明按次价格已低到小团队必然无利可图。因此**不因免费或低价竞争直接否决**。需用同一组图纸检验新产品是否有优势。

### SEO 暂不优先：主任务没有正数信号，泛词又不能借量

**证据来自用户提供的 2026-10-24 PXAny 快照，不是本轮重新向供应商查询。**供应商统计周期、覆盖完整度和独立复核结果未找到；它是决策线索，不是实际网站流量。[供应商入口](https://api.pxany.com/v1/keyword-volumes)

语义审计后，图纸到报价的候选记录有 **108 个“市场×词”**：**93 个供应商返回 0、11 个未返回、4 个未查询，没有返回正数**。其中只说明输入较对口，仍混有买零件或查教程的意图。不得将这些状态相加成“需求为零”。完整分类在证据包 `keyword-audit.csv`，与最终 `serp.json` 同源。[数据入口](https://api.pxany.com/v1/keyword-volumes)

| 需求表达组 | 返回情况 | 能否计入主任务搜索需求 |
|---|---|---|
| 明确图纸/PDF/DWG 的英语核心词：`machining quote from PDF drawing`、`CNC 2D drawing quoting software`、`PDF drawing machining cost estimator`、`DWG machining cost estimation`、`machining cost estimation from drawings` | US/UK/CA/AU 均为**供应商返回 0**；已取回国别 SERP 部分样本 | 属主任务候选；0 不是无人搜索；不报正数需求 |
| 通用 `CNC quoting software` / `machine shop estimating software` / `machine shop quoting software` | US 分别 **30/20/50**；UK、CA、AU 每词各 **10** | 未限定输入；**不计本切口搜索量，不相加成独立买家** |
| 非英语泛软件核心词 | DE、FR、ES、NL 核心词供应商返回 **0**；IT `software preventivi lavorazioni meccaniche` **10**；JP、KR 核心词**未返回** | 只能确认当地相关软件表达/供给；不借给纯 2D 切口 |
| 漏进语种列表的核心词：`CNC quote from drawing`、`software for quoting machined parts` | 四英语市场共 **8 条未查询**；已补普通网页搜索，国别 Google 未取得 | 前者是图纸候选，后者泛词；不填 0、不冒充已完成国别前十 |

以上数值均为快照单市场月搜索量，来源同 [PXAny](https://api.pxany.com/v1/keyword-volumes)；证据包保留未修改原件和最终表。没有外围词达到单市场 **>200** 门槛，故未为其补批量 SERP；核心词不因低量而跳过。

**竞争页按同一个用户任务读，不按每个关键词分别给一份结论。**US 的 `CNC 2D drawing quoting software` 快照仅 **7 条**：

| 快照位置 | 页面满足什么需求 | 本次最终角色 |
|---|---|---|
| 1 | [Spanflug MAKE](https://spanflug.de/en/make/quoting-turning-milling-parts/)：流程写明上传 CAD 模型及技术图纸 | 相关平台；纯 2D 独立自动报价未证实，排除主评分 |
| 2 | [Paperless Parts](https://www.paperlessparts.com/processes/cnc-machining/)：机加工报价平台，明确有 PDF/3D 查看器 | 能看 PDF 不等于能从纯 PDF 自动估价，排除主评分 |
| 3–4 | [AMFG](https://www.amfg.ai/job-shop)、[Machine Research](https://machineresearch.com/estimating-and-quoting-software/) | 本轮未取得足以确认同输入、同输出的完整证据，不计同任务 PMF |
| 5 | [CloudNC Quote Agent](https://www.cloudnc.com/quote-agent) | 同任务供给；产品页打不开，能力由前述官方发布稿核实 |
| 6 | [Dashnode 博客](https://www.dashnode.ai/blog/cnc-quoting-software) | 内容页；不能据其入榜算一个同任务 SaaS |
| 7 | [Gear Solutions](https://gearsolutions.com/news/intuitive-drawing-software-simplifies-2d-path-design-for-cnc-users/) | 2D 刀路设计文章，排除 |

这是供应商返回的部分样本，不能称“Google 完整前十只有一个竞品”。UK/CA/AU 同词分别只有 **8/7/7 条**；本轮普通网页检索另找到 QuotedPart、QuoteBuddy，不能给它们补造国别排名。[国别复查入口](https://www.google.com/search?q=CNC+2D+drawing+quoting+software&gl=us&hl=en&num=10)，快照见证据包。

**域名年龄只观察，不给 SEO 加分。**例如快照把 Dashnode 注册日记为 **2025-07-24**，但此处是博客页；`machining quote from PDF drawing` 下的年轻域名 [Sincere Machining](https://www.sincere-machining.com/cnc-machining-quote-from-your-cad-files/) 是零件服务页，也不证明报价 SaaS 容易进入。日期来自快照 RDAP，独立复核未成功。[RDAP 复查入口](https://rdap.org/domain/dashnode.ai)

### 可以远程交付，难点在工艺与服务成本

**技术路径存在，尚未找到已被竞品遗漏、又能由小团队稳定交付的明确缝隙。**“便宜、支持 PDF、按本厂费率、人工确认”已是直接竞品公开能力，不作为差异化。

可试的窄假设是：选一种本团队能理解的零件族，让**读图来源、装夹/工序假设、不能确定的项目**更容易核对，减少净复核时间。依据是从业者对错误报价的担忧；但现有竞品也在展示可编辑假设和工序，优势必须同题实测，不能靠文案断言。[用户反证](https://www.reddit.com/r/Machinists/comments/1vzvjh8/hows_your_experience_with_automated_quoting_tools/)、[现有工艺明细](https://quotebuddy.therness.com/en/solutions/turning-milling-quotes)

AI 越强，读材料、公差、孔和备注可能越好；仍不能单靠图纸知道每家工厂的装夹、机床能力与外协实际价格。【研究判断】合适架构是 **AI 提取＋确定性成本规则＋人工确认**，不是让语言模型直接输出价格。QuotedPart FAQ 公开采用 Claude 读图、费率公式定价，说明基础读图能力可购买，也说明简单包装缺乏壁垒。[产品 FAQ](https://quotedpart.com/)

作为上游能力，Werk24 公布按量 **€1.25/页**；这是读图，不是最终报价。按一页一件的测试假设，**100 件的提取费为 €125**，尚未包括重试、模型、存储和支持；不能未经成本核算就卖低价不限量。[官方价格](https://www.werk24.io/pricing)。本团队实际成本、错误率和毛利未找到，需试验。

中国团队可通过网页试用、远程配置费率与订阅成交；QuotedPart 有线上注册/支付路径，可证实这种产品形态支持远程购买。[支付说明](https://quotedpart.com/pricing)。先验证愿意提供合规可用、非受限图纸的一般工业客户；若目标客户要求本地驻场或本团队无法提供的数据访问条件，则不属于本次可服务客群。

市场分母仅作背景：Census 官方搜索页显示 Machine shops **17,156 个有雇员营业场所**；本轮未核实该显示值的统计年份，不能直接称最新 CNC 工厂数量。场所也不是独立 SaaS 账户，纯图纸询价占比、可付费比例和全球同口径数量**未找到**，不据此推 SAM（可服务市场）。[Census](https://data.census.gov/all?q=332710)

### 最小验证与停止条件

下表全部是**拟议试验和阈值，未发生招募、收费或产品实测**。先测产品价值，再测 SEO。

| 验证项 | 最小动作及通过条件【建议】 | 停止/不升级条件 |
|---|---|---|
| 同任务可交付 | 5 家各提供 20 份已完成订单图纸：一半校准，一半留出测试；对照真实装夹/加工工时、材料、检验与外协成本，不能只对齐历史售价。与人工/现有软件比较，**计入核对、修正、导出**后，中位耗时至少减少 50% | 出现未标出的关键材料、单位、数量、公差或外协漏项，先停该类自动报价；样本无错也不推为行业准确率。不能净省时或必须创始人逐单代报价，则不升级 |
| **首付** | 10 家合格用户中至少 3 家实际支付首月 $99，范围先限 PDF 常规件；价格与用量包明示。与 CloudNC、QuotedPart、QuoteBuddy 做相同图纸试用比较 | 只有“愿意试”、免费注册或口头承诺，不算首付；无人愿付则暂停开发 |
| **复用** | 首付用户中至少 3 家，在两个不同周主动处理合计至少 5 份**新的真实询价**；记录修改及最终发出的报价 | 只跑历史演示、同件重算或创始人催用，不算复用；套餐内再用不算再次付费 |
| **续费** | 到下一月计费周期，首付用户中至少 2 家实际支付第二月，核实无退款并继续使用 | 尚未到期就写“待观察”；取消/不再使用则复盘。若改按次收费，另看第二个独立订单再次付款，不叫月续费 |
| 小团队经济性 | 首次配置每厂不超过 1 小时；稳定后月支持不超过 30 分钟/厂；把支持人工、解析与重试算入后，目标贡献毛利至少 70% | 依赖驻场、长期专人校准或每份人工审图才能履约，退出当前小团队 SaaS 方案 |
| SEO 获客 | 产品验证通过后，只做图纸报价产品页和真实示例页；观察 8 周，目标从 Google 自然搜索获得至少 5 个合格演示申请及 1 个首付 | 未收录/曝光不足不能推断需求假；维持“SEO 未验证”，不扩多语言页面。只来采购零件、学习公式或索取免费代报价的访客，不算软件线索 |

## 附录：评分、审计、词表与用时

### 综合评分（满分 100）

按五项等权折算：`(4＋2＋2＋2＋2) ÷ 25 × 100 = 48 分`。【研究判断】不是概率或收入预测；**不包含 SEO 评分，也没有因竞品数量扣分**。付费项未过门槛，不能用总分覆盖“当前切口 PMF 未证实”。原报告无数值原分，修正幅度未找到。

### 国家/搜索量审计

原始 **536 个市场×词、374 个去重字符串**；原始核心 SERP **79 组**，均少于完整前十：**7 条×14 组、8 条×36 组、9 条×29 组**。其中 **10 组**明显跑题，最终标记异常；不是“竞争小”。另补记漏词 **8 条未查询**，最终判定表共 **544 条**。数量均由用户提供快照计算，原件、计算脚本和 CSV 保留。[搜索量入口](https://api.pxany.com/v1/keyword-volumes)、[SERP 供应商入口](https://api.pxany.com/v1/serp)

| 市场/查询语言 | 原记录数 | 返回正数 | 供应商返回 0 | 未返回 | 补记未查询 |
|---|---:|---:|---:|---:|---:|
| US/en | 54 | 7 | 47 | 0 | 2 |
| UK/en | 54 | 7 | 47 | 0 | 2 |
| CA/en | 54 | 7 | 47 | 0 | 2 |
| AU/en | 54 | 7 | 47 | 0 | 2 |
| DE/de | 47 | 2 | 45 | 0 | 0 |
| FR/fr | 46 | 3 | 39 | 4 | 0 |
| ES/es | 49 | 0 | 49 | 0 | 0 |
| IT/it | 44 | 2 | 42 | 0 | 0 |
| NL/nl | 45 | 0 | 44 | 1 | 0 |
| JP/ja | 45 | 0 | 0 | 45 | 0 |
| KR/ko | 44 | 0 | 19 | 25 | 0 |
| 合计 | **536** | **35** | **426** | **75** | **8** |

表内是**采集覆盖与状态数，不是市场大小**；全部基于上述快照。尤其 JP 未返回，不能并入“供应商返回 0”。补普通网页搜索不改变未查询搜索量状态。

| 本地表达示例 | 本市场返回情况 | 任务边界 |
|---|---|---|
| DE：`CNC Kalkulation aus 2D Zeichnung` | 供应商返回 0 | 图纸到报价候选 |
| FR：`chiffrage usinage plan PDF` | 供应商返回 0 | 图纸到报价候选 |
| ES：`cotización mecanizado plano 2D` | 供应商返回 0 | 图纸到报价候选；西班牙市场，不借拉美需求 |
| IT：`preventivazione lavorazioni da disegno 2D` | 供应商返回 0 | 图纸到报价候选 |
| NL：`CNC calculatie PDF tekening` | 供应商返回 0 | 图纸到报价候选 |
| JP：`2次元図面 機械加工 自動見積` | 未返回 | 数据缺口 |
| KR：`2D 도면 기계가공 자동 견적` | 未返回 | 数据缺口 |

示例数据来源同 [PXAny](https://api.pxany.com/v1/keyword-volumes)；本地具体表达多为扩词假设，不声称已证实是用户常用搜索语。完整语种词表及逐词剔除理由在证据包。

### 相邻机会：只列，不贡献搜索量、付费或竞争分

- STEP/3D 模型自动报价、DFM（可制造性检查）与 CAM（数控加工编程）：[Toolpath](https://www.toolpath.com/product)、[Spanflug](https://spanflug.de/en/make/quoting-turning-milling-parts/)。
- ERP、生产排程、订单管理及宽报价平台：[ProShop](https://proshoperp.com/)、[JobBOSS²](https://www.ecisolutions.com/products/jobboss2/)、[Paperless Parts](https://www.paperlessparts.com/processes/cnc-machining/)。
- 图纸提取、检索旧报价、RFQ 收件分流：[Werk24](https://www.werk24.io/)、[CADDi](https://caddi.com/en-us/platform/caddi-quote/)。Werk24 仅用于解释上游实现成本，不证明本切口有人付费。
- 工时/小时费率计算器、报价单 PDF 排版、钣金/激光切割报价、采购零件的平台：[Xometry](https://www.xometry.com/how-xometry-works/)。输入或输出不一致，全部排除主评分；需要工厂履约的采购词不作软件 SEO 机会。

### 方法与限制

- **Reddit**：先选 r/CNCmachining，窗口 2026-04-24 至研究日；[Arctic Shift 请求](https://arctic-shift.photon-reddit.com/api/posts/search?subreddit=CNCmachining&after=2026-04-24&before=2026-10-25&limit=100&sort=asc) 首次及间隔后重试均 DNS 失败，网页工具也无法访问，故没有取得半年全量、分页或总体痛点频次。按方法回退定向搜索 r/Machinists/r/CNC；仅报告可逐条核实的个案与热度，不报行业比例。
- **SERP 质量**：异常例为 US `PDF drawing machining cost estimator` 返回税务/风险计算器，US `DWG machining cost estimation` 返回通用“estimation”，以及部分国家的泛 CNC/quote/software 结果。原样保留，最终判定注明异常；未猜测这是 Google 改写还是供应商问题。
- **入口与原报告修正**：专员原分未找到；通用报价付费、3D 模型求助、制造交易额均不替纯 2D PMF；旧域名标签只保存在原始层。当前正文、`serp.md`、`serp.json` 和 `keyword-audit.csv` 采用同一最终判定；没有另行发布报告网页。
- **访问与重试**：执行环境对 PXAny、Arctic Shift、QuotedPart 的 DNS 均失败，公开页改用网页工具；没有重跑原批量脚本。CloudNC 产品/价格页重试仍不可读，保留官方发布稿价格日期。RDAP 独立复核失败；未找到 DR 足以说明竞争易度的证据。
- **证据包**：含报告、原/最终 SERP、逐词 CSV、原词表、网页工具提取记录、失败日志、处理脚本、SOP/标准/方法及需求来源副本。公开证据入口就是正文所链厂商页、原帖和供应商接口；网页提取不是软件实测。

### 用时

本轮深挖与交付：2026-10-24 20:36:19 至 2026-10-24 21:01:32（中国标准时间），约 **25 分 13 秒**。按本轮起止时间实测，含读材料、联网核验、审计、写作及打包；不是产品开发工时。

继承批次日志：扩词 19:48:41–19:52:21（**3 分 40 秒**）；SERP 19:52:21–20:36:11（**43 分 50 秒**）；本轮开始前间隔 **8 秒**。从批次开始至上述完成时点共约 **72 分 51 秒**。继承阶段不冒充本轮重新执行，打包内附原计时记录。
