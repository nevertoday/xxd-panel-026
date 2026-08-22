<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 026 项目介绍" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 026

### 把照片中的事实，转译成安静、温和、仍能一眼认出的几何秩序

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-a76f62?style=flat-square)](#四种输出共享同一种人文几何)
[![Raster Output](https://img.shields.io/badge/Output-PNG-65766d?style=flat-square)](#边界与信任)

<strong>简体中文</strong> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a>

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
- 默认生成与画面语义高度绑定的标题和微型文字。

## 从照片事实到人文几何

026 的内部方法是：

**观察 → 识别 → 删减 → 人文化 → 浅浮雕 → 排版 → 验收**

主体始终是唯一视觉核心。构图偏居中，但不会僵硬对称；它通过正负形、疏密、轻微错动和大面积留白建立节奏。形体像从高级纸张中轻微压出，而不是悬浮在界面中的卡片。

色彩可能靠近米白、暖白、浅灰、沙色、灰粉、浅赭、雾蓝或鼠尾草绿，但这些只是转译方向。真正的主色、辅助色和结构色必须能从当前照片的光线、材质或气氛中解释。

## 样张

样张正在制作中。以下区域已经为四种模式预留，后续可直接替换为 `assets/examples/` 中的正式作品。

<table>
  <tr>
    <td align="center" width="50%"><strong>上下双联</strong><br><br><em>样张制作中</em><br><br></td>
    <td align="center" width="50%"><strong>左右双联</strong><br><br><em>样张制作中</em><br><br></td>
  </tr>
  <tr>
    <td align="center"><strong>纯设计版</strong><br><br><em>样张制作中</em><br><br></td>
    <td align="center"><strong>四端壁纸套装</strong><br><br><em>样张制作中</em><br><br></td>
  </tr>
</table>

## 四种输出共享同一种人文几何

| 模式 | 默认画布 | 成品 |
| --- | --- | --- |
| 上下双联 | 3:4 | 原照片在上，人文几何设计在下，严格等高 |
| 左右双联 | 3:2 | 原照片在左，人文几何设计在右，严格等宽 |
| 纯设计版 | 3:4 | 原照片只作为依据，不出现在最终画面 |
| 四端壁纸套装 | 按设备 | 手机、iPad、电脑、儿童手表四张独立 PNG |

用户给出的精确像素优先于默认比例。上下双联要求总高度为偶数，左右双联要求总宽度为偶数；Skill 不会偷偷修改精确尺寸。

壁纸套装有两种关系：

- **连贯套装**：先生成并验收一张定调图，另外三张同时参考原照片与同一定调图，重新求解各自画幅。
- **四张独立**：每张只参考原照片，构图变化更自由。

连贯不等于裁切。四张壁纸始终分别生成、分别构图、分别验收。

## 文字不是后贴标签

026 默认有文字：一个主标题和 2–4 组微型文字。标题从可见事实、关系张力和有依据的潜台词中提炼，并通过“换图测试”——如果换一张无关照片仍然成立，就必须重写。

用户提供最终文案时逐字保留；提供方向或草稿时，在允许范围内专业深化；明确要求无字时才完全关闭文字。

文案语言按目标受众决定，而不是按人物外貌猜测：

**目标市场／受众地区 > 指定成品语言 > 方向语言 > 当前请求语言**

日本版使用自然日语，韩国版使用自然韩语，英国版使用英式英语。所有地区都做母语转创，而不是机械翻译或伪外文装饰。

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

只上传照片并调用也可以；Skill 会先用分行编号菜单询问模式。壁纸模式未说明关系时，再询问“连贯套装”或“四张独立”。

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
- 普通模式每张源图输出一张；壁纸模式严格输出四张独立文件，不做拼贴总览。

本地合成需要 Python 3 与 Pillow；安全位图桥接器使用 Python 3.11+ 的 `tomllib`。实际生成需要宿主 Agent 的内置位图能力，或已配置好的兼容位图路径。

## 仓库结构

```text
xxd-panel-026/
├── SKILL.md
├── README.md / README.en.md / README.ja.md
├── agents/openai.yaml
├── assets/
│   ├── banner.svg
│   └── examples/
├── scripts/
│   ├── compose_panel.py
│   └── configured_imagegen.py
└── references/
    ├── xxd-panel-026-prompt.zh-CN.md
    ├── xxd-panel-026-prompt.en.md
    └── 026-source.md
```

## 关于 XXD

XXD 是小小东的品牌名缩写。本项目由 [@xiaoxiaodong01](https://x.com/xiaoxiaodong01) 创作与维护。

## 支持与会员权益

### Skills 答疑｜99 元

费用用于 Skills 使用答疑。如需购买或咨询，请扫描下方微信二维码联系小小东。

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
