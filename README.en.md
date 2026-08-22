<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 026 project banner" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 026

### Translate photographic facts into quiet, gentle geometry that remains unmistakably recognisable

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-a76f62?style=flat-square)](#four-outputs-one-humanist-geometry)
[![Raster Output](https://img.shields.io/badge/Output-PNG-65766d?style=flat-square)](#boundaries-and-trust)

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a> · <a href="README.ar.md">العربية</a>

</div>

> RECOGNISE QUIETLY · REDUCE GENTLY · LET THE PAPER BREATHE

XXD Panel 026 is an image-generation skill for Codex and compatible agents. It reads the subject, contour, posture, structural axes, distance, and narrative relationships in a photograph, then translates that evidence into minimal geometry, fine lines, a soft colour family, and barely raised paper relief.

It does not place a muted-colour filter over a photo. It preserves why that particular photograph deserves attention.

## Why it exists

Many “photo to minimal poster” workflows end with the same circles, pastel blocks, and architectural lines. The result may look calm, yet have almost nothing to do with the source. Gesture disappears, relationships are replaced by a template, and the same title could survive a completely different image.

026 treats quietness as evidence-based design:

- at least three source-specific identity cues must remain;
- geometry, contour, structure, and negative space reorganise the subject rather than erase it;
- four to six low-stimulation colour roles are translated from the source instead of selected from a fixed palette;
- depth is limited to pressed or gently raised paper, never overt 3D;
- before generation, choose automatic copy, custom copy, or text-free output; automatic copy produces a source-bound title and microcopy.

## From photographic fact to humanist geometry

The internal method is:

**Observe → Identify → Reduce → Humanise → Relief → Typeset → Check**

The subject remains the sole visual core. The composition tends towards the centre without becoming rigidly symmetrical; positive and negative shape, measured density, small offsets, and generous quiet space create the rhythm. Forms should feel lightly pressed out of fine paper, not like cards floating inside an interface.

Colours may move towards ivory, warm white, pale grey, sand, dusty pink, pale ochre, mist blue, or sage. These are directions, not presets. The principal, supporting, and structural colours must remain explainable through the current photograph's light, material, or atmosphere.

## Samples

Samples are in production. The four mode slots below are ready to be replaced with finished work from `assets/examples/`.

<table>
  <tr>
    <td align="center" width="50%"><strong>Top–bottom</strong><br><br><em>Sample in production</em><br><br></td>
    <td align="center" width="50%"><strong>Left–right</strong><br><br><em>Sample in production</em><br><br></td>
  </tr>
  <tr>
    <td align="center"><strong>Design only</strong><br><br><em>Sample in production</em><br><br></td>
    <td align="center"><strong>Four-device wallpaper pack</strong><br><br><em>Sample in production</em><br><br></td>
  </tr>
</table>

## Four outputs, one humanist geometry

| Mode | Sizing logic | Deliverable |
| --- | --- | --- |
| Top–bottom | source-adaptive | source photograph above, humanist geometry below, each panel retains the complete source size; exact equal height |
| Left–right | source-adaptive | source photograph left, humanist geometry right, each panel retains the complete source size; exact equal width |
| Design only | source-adaptive | source used as evidence but absent from the final canvas; retains the source ratio and dimensions |
| Wallpaper pack | device-specific | four separate PNGs for phone, iPad, desktop, and children's watch |

Exact user-supplied pixels take priority; otherwise ordinary modes adapt to the source instead of imposing stock ratios. Top–bottom needs an even user-specified total height; left–right needs an even user-specified total width. The skill never silently changes an exact requested size.

Wallpaper-pack also has no silent size default: choose the common device preset—phone `1440×3200`, iPad `2048×2732`, desktop `3840×2160`, watch `1024×1024`—or provide labeled custom resolutions.

A wallpaper pack supports two relationships:

- **Linked set:** approve one anchor artwork first, then let the other three reference both the original photo and the same anchor while recomposing for their devices.
- **Four independent works:** every device receives only the original photo and may explore a freer composition.

Linked does not mean cropped. All four wallpapers are generated, composed, and reviewed separately.

## Copy is not a label added afterwards

Before generation, 026 asks for automatic copy, custom copy, or text-free output. Automatic copy uses one main title and two to four microtext groups, distilled from visible fact, relational tension, and grounded implication, then tested against an unrelated-image swap.

In custom-copy mode, the user may supply an exact main title and optional microtext; finished wording stays verbatim. A direction or editable draft is refined only within the permission given. Text-free mode removes all text.

Copy language follows the intended audience rather than any guess based on appearance:

**target market or audience locale > specified output language > direction language; if none is explicit, ask before generation**

A Japanese edition uses natural Japanese, a Korean edition natural Korean, a UK edition British English, and an Arabic edition natural Modern Standard Arabic with correct shaping and right-to-left composition. Every locale is transcreated natively rather than translated literally or decorated with pseudo-foreign text.

## Get started

```bash
git clone https://github.com/nevertoday/xxd-panel-026.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-026" ~/.codex/skills/xxd-panel-026
```

Claude Code users may link the same directory to `~/.claude/skills/xxd-panel-026`. Restart the agent session after installation.

```text
$xxd-panel-026
Turn this photograph into a top–bottom composition. Use Japanese for the main title.
```

Invoking the skill with only a photograph also works. It first asks for the mode in a numbered multiline menu; when wallpaper relationship is unspecified, it follows with linked or independent.

Full specifications:

- [Skill workflow](SKILL.md)
- [Chinese full prompt](references/xxd-panel-026-prompt.zh-CN.md)
- [English full prompt](references/xxd-panel-026-prompt.en.md)
- [Original style brief](references/026-source.md)

## Boundaries and trust

- The current photograph is the current task's only content source; no other input, old output, or sample subject is borrowed.
- Every invocation opens a fresh task directory, even when source and parameters are identical.
- Photography in paired modes stays photographic, with only restrained grading and necessary environmental extension.
- Design-only and wallpaper modes do not show the source and never substitute SVG, HTML, or programmatic drawing for bitmap generation.
- Raster readiness is judged by actual capability, not the absence of one environment variable.
- The safe bitmap bridge returns sanitised status only; it does not expose provider, endpoint, headers, credentials, prompts, or server response bodies.
- Ordinary modes return one file per source. Wallpaper mode returns exactly four separate files, never a collage overview.

Local composition needs Python 3 and Pillow. The safe bitmap bridge uses Python 3.11+ `tomllib`. Generation requires either the host agent's built-in raster capability or an already configured compatible raster route.

## Repository

```text
xxd-panel-026/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ar.md
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

## About XXD

XXD is the abbreviated brand name of Xiaoxiaodong. This project is created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Support and Membership

### In-depth Consultation · CNY 299/hour

One-to-one in-depth consultation for using the Skills is billed at CNY 299 per hour. To book a session, contact Xiaoxiaodong through the WeChat QR code below.

### Xiaoxiaodong Skills User Community · CNY 99 to join

A one-time CNY 99 fee joins the user community for sharing workflows, discussing work, and peer support. It does not include hourly one-to-one in-depth consultation. Scan the WeChat QR code below and include “Skills User Community” in your message.

### Knowledge Planet + Member Prompt Library · CNY 699/year

The Knowledge Planet community and the [XXD Member Prompt Library](https://vip.xiaoxiaodong.ai/) are one membership: **one annual payment unlocks both, with no second purchase required.**

Choose either activation route:

1. Subscribe through [Knowledge Planet](https://wx.zsxq.com/group/15554814142882), then contact Xiaoxiaodong on WeChat for a Member Prompt Library redemption code.
2. Subscribe directly through the [Member Prompt Library](https://vip.xiaoxiaodong.ai/), then contact Xiaoxiaodong on WeChat for an invitation to Knowledge Planet.

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD paid community WeChat QR code" width="320"></a>
</p>

<div align="center">

**Let quietness come from the photograph, not the template.**

</div>

---

<div align="center">
  <h2>☕ Support this open-source project</h2>
  <p>If this project saved you time, a Star, a share, or a coffee helps keep it moving.</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Support Xiaoxiaodong through Buy Me a Coffee" width="180"></a><br>
        <strong>Buy me a coffee</strong><br>
        <sub>Scan or open the QR code to support Xiaoxiaodong</sub>
      </td>
    </tr>
  </table>
  <p><sub>Support is entirely optional and never changes access to this open-source project.</sub></p>
</div>
