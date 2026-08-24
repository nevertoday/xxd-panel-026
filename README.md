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
- 生图前明确选择自动文案、自定义文案或无文字；自动文案才会生成与画面语义高度绑定的标题和微型文字。

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

## 四种可组合输出模式

可用 `1`、`1+3`、`1、2、4` 或 `全部` 选择一个或多个模式；`全部` 每张源图输出 7 个独立 PNG。模式确定后，Skill 会在生图前继续询问整张最终成品的画幅：`3:4` 原提示词画幅、明确跟随原图、常用比例，或自定义比例／准确像素。不会再静默套用源图尺寸。

| 模式 | 画幅逻辑 | 成品 |
| --- | --- | --- |
| `top-bottom` | 用户确认的整张成品画幅 | 一次生成完整画布：高保真原图在上，026 设计在下，约 50/50 |
| `left-right` | 用户确认的整张成品画幅 | 一次生成完整画布：高保真原图在左，026 设计在右，约 50/50 |
| `design-only` | 用户确认的整张成品画幅 | 026 设计铺满画布，不显示原照片 |
| `wallpaper-pack` | 逐设备确认 | 手机、iPad、电脑、儿童手表四张独立 PNG |

双联默认把原图作为高保真垫图／编辑参考，用一套完整提示词直接生成一张整体成品，让摄影、设计、色彩、光线、文字与含义自然呼应。只有完整画布针对性重试仍失败、用户要求原片逐像素不变、当前通道无法实现目标画幅，或需要无创像素校准时，才启用确定性拼合兜底。

壁纸可选连贯或独立。连贯套装先批准一张 iPad 定调图，另外三张分别参考原图＋同一定调图重新构图；独立套装的四张都只参考原图。两者都不会裁切其他设备成品或串联衍生图。

## 文字不是后贴标签

026 在生图前先确认文字方式。选择自动文案时，生成一个主标题和 2–4 组微型文字；标题从可见事实、关系张力和有依据的潜台词中提炼，并通过“换图测试”——如果换一张无关照片仍然成立，就必须重写。

选择自定义文案时，用户可直接输入主标题和可选微型文字，最终成稿逐字保留；提供方向或草稿时，在允许范围内专业深化。选择无文字时完全关闭文字。

文案语言按目标受众决定，而不是按人物外貌猜测：

**目标市场／受众地区 > 指定成品语言 > 方向语言；以上均未明确时，生图前询问**

日本版使用自然日语，韩国版使用自然韩语，英国版使用英式英语，阿拉伯语版使用自然的现代标准阿拉伯语与从右到左排版。所有地区都做母语转创，而不是机械翻译或伪外文装饰。

## 勾选式选择与快捷参数

当运行环境提供真正的交互控件时，Skill 会优先使用卡片式选择：成品模式和普通成品尺寸均可多选，文字方式与壁纸关系为单选。尺寸提供自动适配、跟随原图、1:1、3:4、4:3、4:5、5:4、2:3、3:2、9:16、16:9、21:9、5:7、7:5 和自定义比例／像素。没有交互控件时，会自动改用清楚的多行编号菜单，不显示无法点击的假复选框。

所有设置也可以作为变量直接跟在调用指令后：

```text
/xxd-panel-026 photo.jpg --mode top-bottom,design-only --size auto,3:4,9:16 --text auto --locale ja-JP
```

可使用 `--mode`、可重复或逗号分隔的 `--size`、`--text auto|custom|none`、`--locale`、`--copy`、`--wallpaper linked|independent`、`--wallpaper-size` 和 `--out`。参数齐全时跳过全部问询并直接生成；参数不完整时只补问缺失项。不同比例会分别重新构图，四端壁纸仍是独立设备分支，不与普通尺寸机械相乘。

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
- [中文完整提示词](references/xxd-panel-026-prompt.zh-CN.md)
- [English full prompt](references/xxd-panel-026-prompt.en.md)
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
