<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 026 项目介绍" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 026

### 把照片中的事实，转译成安静、温和、仍能一眼认出的几何秩序

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-a76f62?style=flat-square)](#四种输出共享同一种人文几何)
[![Raster Output](https://img.shields.io/badge/Output-PNG-65766d?style=flat-square)](#边界与信任)

<strong>简体中文</strong> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> RECOGNISE QUIETLY · REDUCE GENTLY · LET THE PAPER BREATHE

XXD Panel 026 是一个面向 Codex 与兼容 Agent 的图像生成 Skill。它先读懂照片中的主体、轮廓、姿态、结构轴线、距离和叙事关系，再把这些事实转译为极简几何、细线、柔和色组与浅浅纸面浮雕。

它不是给照片套一层“莫兰迪滤镜”。它要留下照片为什么值得被看见。

## 为什么需要它

很多“照片转极简海报”最终只剩通用圆形、柔和色块和几根建筑线：看起来安静，却与原照片几乎无关。主体的动作消失了，关系被模板替代，换一张照片仍能继续使用同一套图形与标题。

026 把“安静”当成一种有证据的设计秩序：

- 至少保留三个源图专属身份线索；
- 用几何形、轮廓线、结构线和留白重新组织，而不是抹掉主体；
- 从源图转译 4–6 个低刺激色彩角色，而不是套固定色卡；
- 只使用含蓄的压印或微微隆起感，不做明显 3D；
- 生图前明确选择原始提示词生成文字、用户准确文字或无文字；原始提示词生成文字才会生成与画面语义高度绑定的标题和微型文字。

## 从照片事实到人文几何

026 的内部方法是：

**观察 → 识别 → 删减 → 人文化 → 浅浮雕 → 排版 → 验收**

主体始终是唯一视觉核心。构图偏居中，但不会僵硬对称；它通过正负形、疏密、轻微错动和大面积留白建立节奏。形体像从高级纸张中轻微压出，而不是悬浮在界面中的卡片。

色彩可能靠近米白、暖白、浅灰、沙色、灰粉、浅赭、雾蓝或鼠尾草绿，但这些只是转译方向。真正的主色、辅助色和结构色必须能从当前照片的光线、材质或气氛中解释。

## 样张 · 来自 X

> [小小东（@xiaoxiaodong01）](https://x.com/xiaoxiaodong01/status/2090433161096581434) · 2026 年 8 月 20 日<br>
> GPT2 × 浮雕 × 裁剪 × 冷静 × 美学提示词 × VOL.026<br>
> 它不是把照片再画一遍，而是抓住最有意思的部分重新表达：慢慢减到几根线和几个色块，仍然一眼能够认出。

<table>
  <tr>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090433161096581434"><img src="./assets/examples/sample-01.jpg" alt="XXD Panel 026 样张 1"></a></td>
    <td width="50%"><a href="https://x.com/xiaoxiaodong01/status/2090433161096581434"><img src="./assets/examples/sample-02.jpg" alt="XXD Panel 026 样张 2"></a></td>
  </tr>
</table>

<p align="center"><a href="https://x.com/xiaoxiaodong01/status/2090433161096581434">查看原推文与完整提示词 →</a></p>

这些样张用于展示 026 的美学动机，不会把推文中的旧画幅写成当前 Skill 的默认尺寸；当前四种模式仍遵循下方的生成前明确画幅与自定义尺寸逻辑。

## 原始提示词优先，而不是二次导演

`references/026-source.md` 是本项目唯一的创作与审美权威。Skill 不再额外总结或扩写它，也不会统一规划颜色、色板、美学动机、标题或微文案。原始提示词要求怎样处理颜色、材料、构图、留白与文字，GPT Image 2 就按那套逻辑执行。

模式与尺寸只覆盖原始提示词旧有的 3:4 上下双联容器：左右模式表达原图与设计转译之间的左右视觉关系，但不预设两块半幅或裁切框；在只要设计图和壁纸模式中，下方设计审美扩展到完整画布。除此之外，原始提示词全部保持有效。

## 四种可组合输出模式

模式可以单选或多选：`top-bottom`、`left-right`、`design-only`、`wallpaper-pack`。双联默认把原图、原始提示词、视觉关系和最终尺寸一次交给图像模型，由它直接生成完整画布；只有用户明确要求像素级分区或原片逐像素不变时，才使用确定性拼合。

上下或左右是视觉关系，不是固定的等分容器。区域比例、尺度、留白、交叠、裁切或环境延展由图像模型结合原图与最终画布自主判断，不做分界线、中线百分比或像素坐标检测。

普通成品尺寸同样可以多选：自动适配、跟随原图、1:1、3:4、4:3、4:5、5:4、2:3、3:2、9:16、16:9、21:9、5:7、7:5，或自定义比例／准确像素。没有静默默认尺寸；每个不同比例都会基于同一份原始提示词独立重构。

壁纸套装可选“连贯”或“四张独立”。连贯模式先生成一张定调图，其余设备同时参考原图与定调图重新构图；不会把一张图机械裁成四种尺寸。

## 文字方式

正式生图前只确认三种选择：

1. **模型根据原始提示词生成文字**：用户只指定语言或地区，文字内容、数量、气质与排版由 GPT Image 2 按原始提示词生成；所有文字都从当前图片的内容、气质或隐喻中自然生长。
2. **使用我的准确文字**：逐字传给图像模型，不改写、不翻译、不补标题；排版仍遵循原始提示词。
3. **不要文字**：严格禁止文字与伪文字。

外层 Skill 不再预编标题、微文案或文案包。文字语言与操作语言分开确认，不根据人物、场景或文件名猜测国家与受众。

## 能力自适应问询与快捷参数

同一个 Skill 会根据宿主真正提供的交互能力选择界面，不会把文本符号伪装成可点击控件：

- **Claude Code 提供 `AskUserQuestion + multiSelect: true` 时**：模式和尺寸使用真正的 checkbox；文字方式与壁纸关系使用单选。常用尺寸会按方形、竖版、横版分组展示，并累计多组选项；自定义尺寸进入自由输入。
- **Codex 只提供 `request_user_input` 时**：它只用于文字方式、壁纸关系等互斥单选，不拿来伪装模式或尺寸多选。模式与尺寸改用清楚的组合输入。
- **没有交互工具时**：使用两轮文字问询。第一轮选择一个或多个模式；第二轮填写尺寸与文字方式。Skill 不显示假的 `- [ ]`，也不会为了获得表单要求用户切换 Plan mode。

默认第二轮只展示“智能推荐／跟随原图／常用比例／自定义”四个入口；只有选择常用比例时，才展开完整比例库：方形 `1:1`，竖版 `3:4、4:5、2:3、9:16、5:7`，横版 `4:3、5:4、3:2、16:9、21:9、7:5`。所有比例都可组合，也可直接输入准确像素。

全部设置都可以直接作为参数传入：

```text
/xxd-panel-026 photo.jpg --mode top-bottom,design-only --size auto,3:4,9:16 --text prompt --locale ja-JP
```

支持 `--mode`、可重复或逗号分隔的 `--size`、`--text prompt|exact|none`、`--locale`、`--copy`、`--wallpaper linked|independent`、`--wallpaper-size` 和 `--out`。参数齐全时跳过全部问询；参数不完整时只询问缺失项。

## 生图模型优先级

GPT Image 2 是默认首选，并继续执行本项目现有的高保真垫图、生成前确认整张画幅、双联一次生成完整画布、脚本仅作条件式兜底等逻辑。

当当前工具或已配置兼容通道确实可用，并能满足原图保真、整张成品比例、目标语言文字和连贯壁纸多图参考等要求时，也支持 Seedance 5.0 Pro、Nano Banana Pro（Gemini Image Pro）、Nano Banana 2（Gemini Image Flash）或其他兼容位图模型。备用模型只替换生成通道，不得改变模式、画幅、文案、语言、壁纸关系和完整画布优先策略。

如果没有合适的生图通道，Skill 会请用户启用生图工具或提供 API Key。用户主动提供的凭据可以用于当前任务，但不得在回复或日志中回显、展示或泄露；未经用户明确要求，不会长期保存凭据或修改供应商、账户、计费及全局路由配置。

## 开始使用

### 安装

```bash
git clone https://github.com/nevertoday/xxd-panel-026.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-026" ~/.codex/skills/xxd-panel-026
```

Claude Code 用户可将同一目录链接到 `~/.claude/skills/xxd-panel-026`。安装后重新开启 Agent 会话。

### 调用

```text
$xxd-panel-026
请把这张照片做成上下双联，主标题使用日语。
```

只上传照片并调用也可以；Skill 会先用分行编号菜单询问一个或多个模式。壁纸模式未说明关系时，再询问“连贯套装”或“四张独立”。

完整规范：

- [Skill 工作流](SKILL.md)
- [中文运行适配器](references/xxd-panel-026-prompt.zh-CN.md)
- [English runtime adapter](references/xxd-panel-026-prompt.en.md)
- [原始风格说明](references/026-source.md)

## 边界与信任

- 当前照片是当前任务唯一的内容来源，不借用其他输入、旧成品或样张内容。
- 每次调用都会新建任务子文件夹；相同照片和参数也必须重新生成。
- 双联中的摄影区域保持真实，只允许克制调色和必要的环境延展。
- 纯设计版与壁纸不显示原照片，也不会用 SVG、HTML 或程序化绘图冒充生图。
- 位图可用性按实际能力判断，不会因为缺少某一个环境变量就武断认定无法生成。
- 安全位图桥接器只返回脱敏状态，不展示 provider、端点、请求头、凭据、Prompt 或服务端正文。
- 每个所选普通模式各返回一张；若选择 `wallpaper-pack`，再返回四张独立壁纸。选择 `全部` 时每张原图共返回 7 个 PNG，分处四个同级模式文件夹，绝不生成拼贴总览。

本地合成需要 Python 3 与 Pillow；安全位图桥接器使用 Python 3.11+ 的 `tomllib`。实际生成需要宿主 Agent 的内置位图能力，或已配置好的兼容位图路径。

## 完整画布优先与位图边界

图像模型负责整张成品的审美重构，双联也默认一次直出完整画布。`scripts/compose_panel.py` 只保留为条件明确的兜底、无创尺寸校准和只读审计工具，不再预先规划每次任务，也不评价审美是否成功。

全部交付为 PNG 位图。每次调用都在 `~/Desktop/xxd/` 下创建新任务；已配置图像通道只返回脱敏状态，不公开供应商、端点、凭据、请求头、提示词、响应或账户信息。SVG、HTML、Canvas、图表和程序绘图不能替代最终作品。

## 关于 XXD

XXD 是小小东的品牌名缩写。本项目由 [@xiaoxiaodong01](https://x.com/xiaoxiaodong01) 创作与维护。

## 支持与会员权益

### 深度咨询｜299 元/小时

按小时提供一对一 Skills 深度咨询，每小时 299 元。如需预约，请扫描下方微信二维码联系小小东。

### 小小东 Skills 用户交流群｜入群 99 元

一次付费加入用户交流群，用于 Skills 使用经验分享、作品交流与成员互助；不包含按小时的一对一深度咨询。入群请扫描下方微信二维码，备注「Skills 用户群」。

### 知识星球＋成员提示词库｜699 元/年

知识星球与 [XXD 成员提示词库](https://vip.xiaoxiaodong.ai/)属于同一项会员权益：**支付一次年费，两项同时开通，不需要重复付费。**

任选一种开通方式：

1. 在[知识星球](https://wx.zsxq.com/group/15554814142882)开通后，微信联系小小东，领取成员提示词库兑换码。
2. 在[成员提示词库](https://vip.xiaoxiaodong.ai/)自助开通后，微信联系小小东，由小小东邀请进入知识星球。

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD 付费社群微信二维码" width="320"></a>
</p>

<div align="center">

**让安静来自照片，而不是来自模板。**

</div>

---

<div align="center">
  <h2>⚡ 算力赞助</h2>
  <p>如果这个项目为你节省了时间，欢迎点亮 Star、分享给朋友，或自愿赞助项目算力。</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://colors.xiaoxiaodong.ai/docs/images/wechat-reward-qr.png"><img src="https://colors.xiaoxiaodong.ai/docs/images/wechat-reward-qr.png" alt="XXD 算力赞助微信收款码" height="220"></a><br>
        <strong>微信</strong><br>
        <sub>扫描二维码赞助算力</sub>
      </td>
      <td align="center" width="240">
        <a href="https://colors.xiaoxiaodong.ai/docs/images/alipay-reward-qr.png"><img src="https://colors.xiaoxiaodong.ai/docs/images/alipay-reward-qr.png" alt="XXD 算力赞助支付宝收款码" height="220"></a><br>
        <strong>支付宝</strong><br>
        <sub>扫描二维码赞助算力</sub>
      </td>
    </tr>
  </table>
  <p><sub>算力赞助完全自愿，用于支持生成测试与项目持续维护，不影响项目的免费使用。</sub></p>
</div>
