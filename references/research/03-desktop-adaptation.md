# 桌面适配研究与已有 Skill 检索

核验日期：2026-10-15。此文件由主执行代理整理。以下 Qt 资料是技术依据，不是 Steve Schoger 的观点；所有 FPDF 布局、主题、验证建议均属于项目适配。未访问实际 FPDF 仓库、截图或可运行程序。

## Qt 官方文档

本次 `qt-6` 在线入口显示 Qt 6.12/6.12.0。该标签只是所读网页版本，不表示 FPDF 使用此版本。实施时先核对项目实际 Qt 次版本、导入、Controls style 和组件 API。

| 文档及 URL | 实际读取范围、定位 | 可用结论及边界 |
| --- | --- | --- |
| [Customizing Qt Quick Controls](https://doc.qt.io/qt-6/qtquickcontrols-customize.html) | 正文 Customizing a Control、Definition of a Style、Customization Reference | 定制可复用控件有不同层次；部分原生 style 不适合覆盖外观。只支持“先检查现有 style 的定制边界”，不要求迁移整个项目。示例中的尺寸、色值、透明度不作为产品规范。 |
| [Styling Qt Quick Controls](https://doc.qt.io/qt-6/qtquickcontrols-styles.html) | Using Styles、Compile-Time/Run-Time Style Selection、Mixing Style Selection | Controls style 选择有初始化与导入约束。“换主题色”不可直接等同于“已创建控件后切换整个 style”。不建议为本任务添加未经核验的新版本 API。 |
| [AbstractButton](https://doc.qt.io/qt-6/qml-qtquick-controls-abstractbutton.html) | checkable、checked、down、pressed、text | 持续选中与瞬时按下有不同属性；只有业务确认可切换时才映射 checked。图标按钮仍需文字描述。不能从控件类型猜测 FPDF 的实际动作或互斥逻辑。 |
| [Control](https://doc.qt.io/qt-6/qml-qtquick-controls-control.html) | hovered、hoverEnabled、visualFocus、font、implicit size | 悬停与键盘焦点应分别检查；自定义外观须考虑内容尺寸。不能仅从静态图确认焦点、命中区或字体实际渲染。 |
| [Palette](https://doc.qt.io/qt-6/qml-qtquick-palette.html) | Detailed Description、active、disabled、inactive；末尾 style 注意事项 | Palette 有活动、禁用、非活动组；部分 style 的颜色独立于 palette。不能承诺只改 ApplicationWindow.palette 即可覆盖所有自定义绘制与弹出层。 |
| [Icons in Qt Quick Controls](https://doc.qt.io/qt-6/qtquickcontrols-icons.html) | Using Icons | 平台主题图标可能优先于 source；着色、尺寸需核验。跨平台一致性应检查真实资源解析，而非凭 icon.source 推断最终图标。 |
| [High DPI](https://doc.qt.io/qt-6/highdpi.html) | Conceptual Model、Drawing、Coordinate Systems Reference | Qt 常规 UI 几何使用设备无关坐标；图像缓冲和底层渲染需区分。截图物理像素不直接作为 QML 逻辑尺寸。未做 DPI 实测。 |

## 形成的项目建议（适配，非作者原始规范）

- 先查已有 Theme、tokens、图标、按钮、字段、弹窗和 Controls style，再提出修改；不存在时仅提议最小角色集。
- 基础值 → 语义角色 → 组件状态的映射是本 Skill 的适配结构。名字只是示意，不代表仓库已有接口。
- 浅色、深色与品牌色按同一语义角色提供不同取值；页面纸色、文档内容、批注原色与应用装饰色分开决策。
- 持续状态、瞬时指针反馈、键盘焦点、业务错误相互独立；用组合状态样例检查遮盖问题。
- 缩放比例、窗口、文档、面板展开情况必须一致，才能比较可视画布和密度。
- 桌面验收计划可包含 Windows 100%、125%、150%、200% 缩放、混合 DPI、长中文/英文、键盘遍历及目标跨平台；这些是建议样本，不是已执行测试或 Steve 的规范。

## 已有 Skill 检索

- 检索本机 `.codex/skills` 与 `.agents/skills` 内 SKILL.md，未找到同名 Steve Schoger 专用 Skill。未把相近的通用 UI Skill 当作一手资料。
- 远程检索词包含 `"SKILL.md" "Steve Schoger"`，打开 [mikeoptimax/refactoring-ui/SKILL.md](https://github.com/mikeoptimax/refactoring-ui/blob/main/SKILL.md)。它是第三方通用规则集，存在宽松留白和固定示例值等 Web 倾向；未采用其内容作为 Steve 的原始方法，也未安装或复制。
- 结论：按用户明确要求新建 `steve-schoger-ui`，从一手材料重新整理证据，同时加入可区分的桌面适配。

## 流程裁剪

女娲的资料核验、方法提炼、边界声明、独立自检保留。人物生平、语气 DNA、第一人称身份与人物立场预测不适用；用户已明确排除模仿。研究聚焦方法与公开案例，不为凑来源数量加入第三方书摘或传记。
