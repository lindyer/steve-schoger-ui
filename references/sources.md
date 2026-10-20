# 资料来源与使用范围

核验日期：**2026-10-15**。只使用本次实际取得的公开内容。研究代理分别记录阅读范围；“读过幻灯片文字/指定案例图”不等于观看演讲。这里的 [原始] 表示有直接一手证据，**不表示独创、唯一正确、经过用户实验或适用于所有产品**。

## 归属与证据政策

- Refactoring UI 的作者为 **Adam Wathan 与 Steve Schoger**。联名文章、书籍、课程和共同官方项目不能全部归到 Steve 一人；Steve 的演讲可注明他为讲者，但不由此断言每条思想为其独创。
- 本次没有用户提供的授权付费内容，**未获取或阅读**付费书籍全文、付费视频、组件画廊、色板和字体资源。官网目录只证明主题存在，不能证明已读章节。
- 不使用付费内容的第三方 PDF、泄露副本、来源不明镜像或第三方书摘来补齐原文。产物为简短方法概述与原创项目适配，不复制书页、图集或大量原文。
- 原始方法、案例归纳、桌面适配使用不同标签；不能将来源里的案例值升级为 Qt 规范。更新资料时记录实际访问范围及日期；访问失败保留边界，不用搜索摘要代替正文。

## 一手设计资料

下列“第 N 页”统一指 SpeakerDeck 页面 **Transcript 区域的一基幻灯片条目序号**，不是视频时间戳或口述段落。原图文件名可能采用不同起点，具体案例图以研究记录的原图 URL 定位。

### S01 联名公开文章：七项具体设计策略

- **标题/作者**：*7 Practical Tips for Cheating at Design*；Adam Wathan & Steve Schoger；2018-02-20。
- **链接**：[Medium / Refactoring UI 公开正文](https://medium.com/refactoring-ui/7-practical-tips-for-cheating-at-design-40c736799886)。
- **访问范围**：实际读取引言和七节正文；未把评论当作者材料。
- **定位与可支持结论**：§1 字重/颜色层级；§2 彩底文字；§3 有方向的阴影；§4 比较分隔方式；§5 图标原定尺寸；§6 强调色边；§7 行动主次。
- **范围限制**：Web 设计策略；不是工具栏高度、Qt 字重映射或所有状态的规范。正文提到的示例尺寸、数量和颜色不作为 FPDF 默认值。行动主次也不能直接变成“整个编辑器只能有一个主要命令”。
- **使用处**：M1/M3/M4/M5、R01–R03、R06、R08；只取有关任务的策略，不复刻全文。

### S02 本人演讲：如何进行视觉设计判断

- **标题/发布者**：*How to Think Like a Visual Designer*；Steve Schoger，本人 SpeakerDeck 账户；发布于 2019-07-25。
- **链接**：[公开幻灯片](https://speakerdeck.com/steveschoger/how-to-think-like-a-visual-designer)，由 [本人 Speaking 页](https://www.steveschoger.com/speaking/) 链接。
- **访问范围**：逐页可提取文字；另实际查看 Tuple 布局与播客主题的六张指定图。未观看视频或获取口述字幕。
- **定位**：页面文字第12页多个布局、第51页颜色/字重、第75页彩底文字、第87页图标尺度、第133–140页深色主题。图像链接及编号差异见 [案例研究 P1](research/02-public-cases.md)。
- **可支持结论**：探索备选布局；对比不只靠大小；深色不能简单反相。案例证明存在这些处理，不证明桌面效率改善幅度。
- **范围限制**：Tuple 是网站首屏，其大标题、插画和留白不适配本项目。播客层级不是通用主题配方；本次没有 Steve 对 FPDF、QML 或完整交互状态的原始规范。
- **使用处**：M2/M5、R05/R09；方案比较的具体约束与验收方法仍为归纳/适配。

### S03 本人演讲：界面的局部细节

- **标题/发布者**：*The Little Details of UI Design*；Steve Schoger；2018-02-07，页面说明对应 Laracon Online 2018。
- **链接**：[公开幻灯片](https://speakerdeck.com/steveschoger/the-little-details-of-ui-design)。
- **访问范围**：可提取的逐页文字和修改标注；未完整检查案例图、未观看口述。
- **定位与可支持结论**：第29–40页搜索框、圆角与图标；第66–84页文字、侧栏和次要内容；第87–88页信息主次。可支持检查不一致和过强的视觉元素。
- **范围限制**：从局部异常到修改再比较的工作循环，是本 Skill 对案例的归纳；不是作者命名的固定程序。演示值不用于项目硬编码。
- **使用处**：M2/M4、R05/R06；适用与失效条件另由本 Skill 明示。

### S04 本人演讲：常见 UI 视觉问题的具体处理

- **标题/发布者**：*Practical Solutions to Common UI Design Problems*；Steve Schoger；2019-06-13。
- **链接**：[公开幻灯片](https://speakerdeck.com/steveschoger/practical-solutions-to-common-ui-design-problems)，本人 Speaking 页列为 CSS Day 演讲资料。
- **访问范围**：可提取逐页文字；实际查看两张航班表单图标比较和一张表格图。未看完整演讲。
- **定位**：第11页文字对比、48–54页感知亮度、58页间距、68页重量与对比、104–109页对齐/数字、110页少边框、139页背景分隔；具体原图见 [案例研究 P2](research/02-public-cases.md)。
- **可支持结论**：平衡视觉重量、比较对齐与分隔；数字明度一致不保证相同观感。少边框不等于消除所有结构线。
- **范围限制**：辅助图标变淡的案例，不支持将所有操作图标淡化。间距主题不能覆盖桌面画布要求；数字特性主题不证明某个 QML 属性或字体可用。
- **使用处**：M3/M4、R03/R04/R07。

### S05 Refactoring UI 官方公开页面

- **归属/链接**：Adam Wathan 与 Steve Schoger；[Refactoring UI 官网](https://refactoringui.com/)。
- **访问范围**：公开介绍、边框示例、目录与 FAQ。**未读目录指向的付费章节**。
- **可支持结论**：共同创作；项目原始语境为 Web；公开边框例子可作为问题与策略的说明。组件示例用于启发，不能代替具体产品判断。
- **范围限制**：不从销售页推导付费资料的完整内容，不转述未读视频或资源包。仅作身份/范围确认和有限的公开方法交叉核验。

### S06 本人对共同作品的说明

- **作者/链接**：Steve Schoger；[本人 Book 页](https://www.steveschoger.com/book/)。
- **访问范围**：页面全部简短公开说明。
- **可支持结论**：Refactoring UI 的书、视频和资源由他与 Adam Wathan 共同制作，面向 Web 设计教学。
- **范围限制**：该页不提供 Qt 状态、尺寸、品牌切换或桌面密度规范。

### S07 本人演讲：十五项实用设计提示

- **标题/发布者**：本人官网列为 *15 Practical Tips for Cheating at Design*；Steve Schoger；2018-09-22。SpeakerDeck 页面的文件标题为 `fluxible-15m.pdf`，与 S04 是不同资料。
- **链接**：[公开幻灯片](https://speakerdeck.com/steveschoger/fluxible-15m)。
- **访问范围**：可提取文字；实际查看联系人弹窗分隔对照与图标尺度对照。原图见 [案例研究 P3](research/02-public-cases.md)。
- **可支持结论**：以间距/背景比较密集分隔线；层级不只靠字号；不要机械放大小图标。
- **范围限制**：给图标加承载背景只是案例做法，不是桌面按钮必须有圆底。不是付费书 PDF，也没有阅读视频。
- **使用处**：为 M1/M3/M4 的跨案例归纳提供交叉证据。

## Qt 官方技术资料：只支持适配层

以下资料作者/发布者为 The Qt Company 与文档贡献者；不是 Steve/Adam 的观点。本次在线 `qt-6` 页面显示 Qt 6.12/6.12.0，**不表示 FPDF 的实际版本**。实施时核对项目 Qt 次版本与 style；不要求升级。

| 编号 | 官方链接与实际读取定位 | 支持范围 / 不支持的推论 |
| --- | --- | --- |
| Q01 | [定制 Qt Quick Controls](https://doc.qt.io/qt-6/qtquickcontrols-customize.html)：单控件、可复用组件、style 定义与 Customization Reference | 定制具有不同层次，部分原生 style 不适合覆盖。不能据示例给产品设固定颜色、半径、透明度或尺寸。 |
| Q02 | [Controls style 选择](https://doc.qt.io/qt-6/qtquickcontrols-styles.html)：编译期/运行期与混用；[QQuickStyle](https://doc.qt.io/qt-6/qquickstyle.html)：初始化限制 | style 需在相关 QML 类型注册前配置，不能承诺已创建控件后随意切换。主题/品牌角色变更是另一件事。 |
| Q03 | [AbstractButton](https://doc.qt.io/qt-6/qml-qtquick-controls-abstractbutton.html)：checked/checkable、pressed/down、text | 区分持续选中与瞬时按下；图标按钮需要文字描述。不证明 FPDF 某按钮实际可切换或属于互斥组。 |
| Q04 | [Control](https://doc.qt.io/qt-6/qml-qtquick-controls-control.html)：hovered/hoverEnabled、visualFocus、内容隐式尺寸 | 分别核验悬停、键盘焦点和内容尺寸。不能把所有焦点需求都替换成一种视觉规则。 |
| Q05 | [Palette](https://doc.qt.io/qt-6/qml-qtquick-palette.html)：三组颜色与 style 注意事项 | active/inactive/disabled 含义不同，部分 style 使用独立颜色。仅改根 palette 不能保证所有组件和弹出层被覆盖。 |
| Q06 | [Qt Quick Controls 图标](https://doc.qt.io/qt-6/qtquickcontrols-icons.html)：Using Icons | 平台主题图标的优先级、颜色和尺寸需核验；icon.source 不保证就是最终资源。 |
| Q07 | [High DPI](https://doc.qt.io/qt-6/highdpi.html)：坐标模型、绘图与坐标参考 | 常规 UI 几何使用设备无关坐标，原始图像缓冲不同；截图物理像素不能直接变成 QML 逻辑尺寸。未执行 DPI 测试。 |

## 不能用作正文证据的材料

| 材料 | 本次状态及边界 |
| --- | --- |
| 付费 Refactoring UI 书、screencasts、组件库和设计资产 | 用户未提供，未取得、未读、未下载；未来只处理用户明确提供并许可的范围。 |
| [CSS Day 视频](https://www.youtube.com/watch?v=7Z9rrryIOC4)、[官方播放列表](https://www.youtube.com/playlist?list=PLDVpvW8ghDr9tasku_YvuTy_l0xPUtOHE) | 仅入口/元数据；没有完整视频或字幕，不提供虚构时间戳。对应方法只从已读幻灯片提取。 |
| [Full Stack Radio 74](https://fullstackradio.com/74)、[103](https://fullstackradio.com/103)、[Yo 访谈](https://www.yo.fm/steve) | 仅简介/show notes，不推导来宾回答。详见案例研究。 |
| 猜测的 refactoringui.com `/previews/7-practical-tips-for-cheating-at-design` 与 adamwathan.me 同名路径 | 本次不可访问，采用 S01 可读联名原文；不声称读过不可访问页面。 |
| 第三方 Skill、转载、社交聚合与书摘 | 仅查重/发现线索；不作为本人方法证据，不复制其规则。未使用未验证推文正文。 |

## 资料与产物的关系

- 直接方法见 S01–S04/S07；共同归属由 S05/S06 交叉确认。有限的案例阅读足以构建条件性策略，不能还原完整作者直觉。
- “保存基线、控制主要变量、给最小与较大方案、用任务指标评估”是本 Skill 的**案例归纳**，不是声称作者原始步骤。
- Theme/tokens 架构、桌面密度、画布预算、状态矩阵、DPI/键盘验证、保存/多选/进度边界均为**FPDF 适配**。
- 研究记录：[一手文字范围](research/01-primary-methods.md)、[指定案例图及访问限制](research/02-public-cases.md)、[桌面技术适配与查重](research/03-desktop-adaptation.md)。研究内的 P 编号是各文件局部编号；对外引用统一使用本文件 S/Q 编号。
