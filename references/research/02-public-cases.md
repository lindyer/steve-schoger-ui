# 本人公开案例与设计过程核验

核验日期：2026-10-15。任务范围：从 Steve Schoger 公开教学中提炼设计判断，服务 FPDF；不分析人格、语气或生平。未获取付费书籍、付费视频课程或付费组件库。

## 资料身份与访问路径

本人官网 [Speaking](https://www.steveschoger.com/speaking/) 直接链接以下三套幻灯片，均位于 `speakerdeck.com/steveschoger`。本次读取页面文字转录，并实际查看下列指定原图；不是只看搜索摘要。页面上名为 Transcript 的区域是**幻灯片文字提取**，不是演讲音频逐字稿。不同页面的转录序号与图片文件名可能不同，故定位同时给出章节标题和原图 URL，避免错误页码。

Steve Schoger 是这些演讲的讲者与公开幻灯片发布者；这不证明每条思想由他独立创作。凡引用 Refactoring UI 的共同成果，应标为 **Adam Wathan 与 Steve Schoger 共同创作**。本人 Book 页也明确两人共同制作该书与课程：[作者身份说明](https://www.steveschoger.com/book/)。

## P1 — How to Think Like a Visual Designer

- 作者/发布者：Steve Schoger。公开发布日期：2019-07-25；本人官网将其列为 Laracon US 2019 演讲资料。
- 精确 URL：[公开幻灯片](https://speakerdeck.com/steveschoger/how-to-think-like-a-visual-designer)。
- 实际访问：网页文字转录；Tuple 布局样例与播客主题比较的原图。未观看完整演讲、未获取演讲字幕。
- 证据定位：多布局探索、颜色与字重对比、深色非反相三个主题；中文为定位概述，不是逐字引语。
- 已核验原始方法：探索多个布局；用颜色与字重建立对比；深色主题不能简单反相。
- 已观察案例：Tuple 同一主张/表单有居中与左右布局；播客主题对照保留顶部较暗、底部较亮的关系。这只证明所示案例，不是所有应用必须如此。
- 可信度：一手公开教学，高；对未出现的桌面行为无证据。

实际查看的图像定位：

- [Tuple 内容区域标记](https://files.speakerdeck.com/presentations/9e5eaff79fa64ae2842d72cc6c2acc8a/slide_12.jpg)
- [Tuple 居中版本](https://files.speakerdeck.com/presentations/9e5eaff79fa64ae2842d72cc6c2acc8a/slide_15.jpg)
- [Tuple 左文右图占位版本](https://files.speakerdeck.com/presentations/9e5eaff79fa64ae2842d72cc6c2acc8a/slide_24.jpg)
- [Tuple 插画版本](https://files.speakerdeck.com/presentations/9e5eaff79fa64ae2842d72cc6c2acc8a/slide_32.jpg)
- [播客浅色层级标注](https://files.speakerdeck.com/presentations/9e5eaff79fa64ae2842d72cc6c2acc8a/slide_135.jpg)
- [播客浅深并排主题比较](https://files.speakerdeck.com/presentations/9e5eaff79fa64ae2842d72cc6c2acc8a/slide_138.jpg)

使用边界：Tuple 是网站首屏，不能据此把巨型标题、大块插画或大留白搬进 FPDF；播客是示例而不是 Qt 色板规范。

## P2 — Practical Solutions to Common UI Design Problems

- 作者/发布者：Steve Schoger。公开发布日期：2019-06-13；本人官网将其链接于 CSS Day 演讲。
- 精确 URL：[公开幻灯片](https://speakerdeck.com/steveschoger/practical-solutions-to-common-ui-design-problems)。
- 实际访问：网页文字转录；航班查询表单中图标深浅比较，以及含行分隔线的表格原图。未观看完整视频。
- 证据定位：视觉重量与对比、少边框、感知亮度、按可读性对齐四个主题；中文为定位概述。
- 已核验原始方法：平衡视觉重量与对比；减少过多边框；明度数值相同未必观感相同；对齐应考虑可读性。
- 已观察案例：一对航班表单改变图标颜色来减弱其视觉重量；“减少边框”章节仍出现有行线的表格，不能解释成禁止全部边框。
- 可信度：一手公开教学，高；没有用户实验效果数据。

实际查看的图像定位：

- [航班表单较重图标版本](https://files.speakerdeck.com/presentations/b2e2444d858e45728c45f2eabe9bfbe8/slide_68.jpg)
- [航班表单减弱图标版本](https://files.speakerdeck.com/presentations/b2e2444d858e45728c45f2eabe9bfbe8/slide_69.jpg)
- [减少边框章节中的表格](https://files.speakerdeck.com/presentations/b2e2444d858e45728c45f2eabe9bfbe8/slide_110.jpg)

使用边界：该表单里的图标多为字段辅助信息；FPDF 的图标按钮本身可能承担操作语义，不能照搬淡化效果导致按钮难辨。此区分是本任务的适配判断。

## P3 — 15 Practical Tips for Cheating at Design

- 作者/发布者：Steve Schoger。公开发布日期：2018-09-22；本人官网链接名为此演讲，Speaker Deck 页面标题为 `fluxible-15m.pdf`。
- 精确 URL：[公开幻灯片](https://speakerdeck.com/steveschoger/fluxible-15m)。
- 实际访问：网页文字转录；联系人对话框边框前后对照；图标大小前后对照原图。不是付费书籍 PDF。
- 证据定位：少边框、字号以外的层级、小图标设计尺寸三个主题；中文为定位概述。
- 已核验原始方法：不只靠字号建立层级；少用冗余边框；避免放大本为小尺寸绘制的图标。
- 已观察案例：联系人对话框用间隔、分区背景替代密集横线；图标案例以小图形加承载背景获得视觉体量。这不是每个桌面图标都加圆底的规定。
- 可信度：一手公开教学，高。

实际查看的图像定位：

- [联系人对话框前后对照](https://files.speakerdeck.com/presentations/ce6f09b0c3814bc0ac573a3b75aa364c/slide_9.jpg)
- [图标尺寸/承载背景对照](https://files.speakerdeck.com/presentations/ce6f09b0c3814bc0ac573a3b75aa364c/slide_49.jpg)

使用边界：图中尺寸与颜色均为该案例的示意值，不是 FPDF 的 token 值，也不是 Windows 桌面控件规范。

## 仅核验入口，未据此提炼内容

以下资料真实存在且是本人官网链接，但当前访问只得到元数据、节目简介或题目，**不计入已阅读内容证据**：

| 资料 | 精确 URL | 本次实际取得 | 禁止声称 |
|---|---|---|---|
| CSS Day 2019: Steve Schoger / Refactoring UI | https://www.youtube.com/watch?v=7Z9rrryIOC4 | 视频页标题；方法内容取自 P2 的公开幻灯片 | 不声称看过视频、听过口述、具有精确时间戳 |
| Refactoring UI YouTube 播放列表 | https://www.youtube.com/playlist?list=PLDVpvW8ghDr9tasku_YvuTy_l0xPUtOHE | 本人官网入口与 YouTube 通用页面 | 不声称看过各重构过程 |
| Full Stack Radio 74 | https://fullstackradio.com/74 | Adam Wathan 主持、Steve Schoger 来宾、2017-10-12；仅官方 show notes | 不能从“讨论灰阶设计”等题目推导他具体如何做 |
| Full Stack Radio 103 | https://fullstackradio.com/103 | Adam Wathan 与 Steve Schoger 设计问答，2018-12-05；仅官方 show notes | 不能编造他们对起步流程、复杂表格、次级动作的回答 |
| Yo! Steve Schoger | https://www.yo.fm/steve | 主持 Rob Hope，2019-05-15；仅简介和空字幕容器 | 不声称取得逐字稿或听过 1 小时访谈 |

## 本任务归纳：可以操作，但不称为 Steve 的原始固定流程

下列是对以上案例组织方式的归纳，证据等级为 **[归纳]**；不是讲者声称的统一步骤。

1. **比较应当有明确变化变量。** P1 把布局变化显示出来，P2 显示图标重量变化，P3 显示分隔方式变化。因此评审时可以保存基线、列出变化维度，以可解释的差别支持选择；不能把所有视觉属性一起改变后把偏好称为事实。
2. **先问元素为何显眼。** 显眼程度不只来自大字号，还来自字重、颜色、边界、背景与图标体量。可以先消除不该强调的竞争元素，再决定是否增强主元素。
3. **把原则理解为带条件的工具。** 多套示例仍采用不同布局、表格分隔和背景，不能将“少边框”升级为“无边框”，也不能将单个对照图宣布为唯一正确方案。

## FPDF 适配建议：全部属于 [适配]，不归为原始规范

- 工具栏：先列出工具角色与频率，再比较紧凑分组和局部突出方案；保持文档画布、最小窗口及已有快捷操作约束。可调整图标墨量，但操作图标不能因“辅助”之名降到近似禁用状态。
- 属性面板：以分组标题、控件和值的角色建立层级；检验层级后再压缩空隙。把“减少线条”理解为比较分隔手段，保留确实帮助密集属性识别的结构线。
- 设置弹窗：比较字段对齐、分组、页脚动作层级；较少边界的版本仍须能区分输入框、选中状态与分组。浅深主题分别检查，并根据现有 Theme 的语义 token 映射色彩。
- 多方案比较的项目验收项：能否辨认当前工具、能否扫描属性、能否找到并解释当前设置、文档可视面积是否受到无谓侵占。指标由项目任务定义，不伪称讲者给出的评分公式。
- 截图只能证明当前可见外观。悬停、按下、禁用、焦点、键盘操作和任务取消等若没有演示、状态图或代码，均记为未知；不从静态对比图推断行为。

## 可供主 Skill 使用的证据标签

- `[原始 P1/P2/P3]`：仅用于上方明确核验的讲授方法与案例事实。
- `[归纳 P1/P2/P3]`：用于“固定基线、分维度比较、解释取舍”等整理后的工作方式。
- `[适配 FPDF]`：用于 Qt/QML、token、画布面积、桌面密度、状态覆盖及具体验收方法。
- 不引用大段正文或复刻幻灯片；本文件用简短摘要与原图链接保持可追溯。
