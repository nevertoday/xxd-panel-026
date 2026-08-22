<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 026 project banner" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 026

### Translate photographic facts into quiet, gentle geometry that remains unmistakably recognisable

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-a76f62?style=flat-square)](#four-outputs-one-humanist-geometry)
[![Raster Output](https://img.shields.io/badge/Output-PNG-65766d?style=flat-square)](#boundaries-and-trust)

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a>

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
- a source-bound title and microcopy are present by default.

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

| Mode | Default canvas | Deliverable |
| --- | --- | --- |
| Top–bottom | 3:4 | source photograph above, humanist geometry below, exact equal height |
| Left–right | 3:2 | source photograph left, humanist geometry right, exact equal width |
| Design only | 3:4 | source used as evidence but absent from the final canvas |
| Wallpaper pack | device-specific | four separate PNGs for phone, iPad, desktop, and children's watch |

Exact user-supplied pixels override the default ratios. Top–bottom needs an even total height; left–right needs an even total width. The skill never silently changes an exact requested size.

A wallpaper pack supports two relationships:

- **Linked set:** approve one anchor artwork first, then let the other three reference both the original photo and the same anchor while recomposing for their devices.
- **Four independent works:** every device receives only the original photo and may explore a freer composition.

Linked does not mean cropped. All four wallpapers are generated, composed, and reviewed separately.

## Copy is not a label added afterwards

026 includes copy by default: one main title and two to four microtext groups. Wording is distilled from visible fact, relational tension, and grounded implication, then tested against an unrelated-image swap. If the same line still works on an unrelated photograph, it must be rewritten.

Finished user copy stays verbatim. A direction or editable draft is refined only within the permission given. Text disappears only when the user explicitly requests a text-free result.

Copy language follows the intended audience rather than any guess based on appearance:

**target market or audience locale > specified output language > direction language > request language**

A Japanese edition uses natural Japanese, a Korean edition natural Korean, and a UK edition British English. Every locale is transcreated natively rather than translated literally or decorated with pseudo-foreign text.

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

## About XXD

XXD is the abbreviated brand name of Xiaoxiaodong. This project is created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Support and Membership

### Skills Q&A · CNY 99

This fee covers Q&A support for using the Skills. To purchase or ask a question, contact Xiaoxiaodong through the WeChat QR code below.

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
