---
name: xxd-panel-026
description: "Create XXD Panel 026 artwork from supplied photos in four independently selectable modes that may be combined: photo above/humanist geometry below, photo left/humanist geometry right, transformed design alone, or a four-device wallpaper pack with either independent compositions or anchor-linked visual continuity. Uses an explicit whole-canvas ratio or resolution preflight, complete-canvas generation by default, an approximately equal paired layout target, and an explicit choice for copy, locale, or text-free output. Use for the exact quiet architectural/editorial 026 style; never use it for collages or generic pastel abstraction."
---

# XXD Panel 026 · 温和人文几何

Turn every supplied photograph into finished editorial artwork. Each selected mode may show the source photo above, show it on the left, omit it from one transformed canvas, or expand it into four separately composed device wallpapers while still using it as the sole content source.

Operational rules follow the shared XXD Panel workflow contract: four combinable modes; an explicitly confirmed whole-canvas ratio or exact resolution before generation; single complete-canvas raster generation by default; high-fidelity source reference in paired modes; linked or independent four-device wallpapers; copy and locale preflight; fresh generation jobs; privacy-preserving raster generation; deterministic composition as fallback only; and one fresh task directory per source and mode. Style-specific sections refine aesthetics and copy but never override this contract.

## Non-negotiable contract

- One source photo may be processed in one or more selected modes. Each selected ordinary mode (`top-bottom`, `left-right`, `design-only`) produces one output; selected `wallpaper-pack` produces exactly four separate files. Selecting all four modes therefore produces seven final PNGs per source. Keep every mode in its own task directory and never combine modes or wallpaper files into a grid, collage, contact sheet, or overview.
- Resolve a non-empty ordered set of output modes before generation: `top-bottom` (photo above, geometric design below), `left-right` (photo left, geometric design right), `design-only` (only the transformed design is visible), and/or `wallpaper-pack` (phone, iPad, desktop, and watch wallpapers). Accept one choice, multiple choices separated by `+`, Chinese/English commas or whitespace, natural-language names, or `全部` / `all`. Deduplicate repeated choices and execute in menu order 1→4. If none is specified, ask the concise multi-select question in the workflow and wait; never ask again when the selected set is already clear.
- When the selected set contains `wallpaper-pack`, it has a second required choice: `linked` continuity or `independent` compositions. Ask the two-choice follow-up in the workflow whenever that relationship is not already specified. `linked` uses one approved wallpaper as a visual anchor for the other three; `independent` gives every device only the original source photo. Neither relationship permits mechanical resizing, cropping one wallpaper into another, or returning fewer than four files. Do not ask this follow-up when wallpaper mode is not selected.
- In `top-bottom` and `left-right`, target a visually equal 50/50 relationship inside one coherent generated canvas. Minor generative deviation is acceptable unless the user explicitly requires pixel-exact halves; exact deterministic geometry belongs to fallback composition. In `design-only`, there is no photographic panel and no seam; the transformed design fills the entire final canvas.
- The whole final canvas ratio or exact pixels must be explicitly resolved before generation. Offer the original-prompt 3:4, source aspect as an explicit choice, common ratios, or custom ratio/pixels; never infer explicitly selected final-canvas dimensions silently. Exact pixels take precedence over an explicitly chosen ratio.
- Any visible photographic region remains faithful. Allow only restrained editorial color grading and seamless environmental extension needed to fit its frame. Never stretch, distort, redraw, replace, or structurally alter the subject. In `design-only` and every wallpaper output, use the source only as evidence and render none of it in the final artwork.
- The transformed region is a photo-derived minimal humanist geometric construction: recognizable subject evidence, flat restrained shapes, fine contour or structural lines, generous quiet space, and only a whisper of pressed-paper relief. It is not a trace, realistic illustration, generic pastel wallpaper, or unrelated abstraction.
- Use a restrained 4–6 color palette derived from the source photo and translated toward warm white, sand, pale ochre, dusty pink, mist blue, sage, or nearby low-stimulation hues. These are roles, not a fixed palette.
- Copy has no silent default. Before generation, resolve one explicit choice: source-derived automatic copy, user-supplied exact copy, or text-free output. By default, one source-specific copy package is shared verbatim across all selected modes; accept explicit per-mode copy overrides when the user supplies them. Automatic or direction-led copy contains one main title and 2–4 microtext groups. Custom copy requires an exact main title; user microtext is optional, and supporting microtext may be professionally derived unless the user explicitly requests title-only.
- Resolve copy locale independently from the language used to issue the command. Use this priority for automatic or direction-led copy: explicit target market/audience locale > explicit output language > language of the supplied direction; if none is explicit, ask before generation. Never infer audience language, nationality, or ethnicity from a face, name, clothing, scenery, filename, metadata, or visible signage. Localize by transcreation—native wording, register, rhetoric, punctuation, and line breaking—not literal translation or foreign-looking pseudo-text. Arabic output uses natural Modern Standard Arabic unless the user names a regional variety; preserve connected letterforms, right-to-left reading order, Arabic punctuation, semantic line breaks, and deliberate handling of embedded Latin text or numerals. Do not mirror the artwork indiscriminately: reverse text flow and typographic alignment while keeping source-derived subject direction and composition intentional. Preserve exact finished copy verbatim unless the user explicitly asks to translate/localize it; if exact wording conflicts with an explicitly named target locale and permission is unclear, ask one concise clarification before generation. Do not invent a year; retain one only when explicitly supplied or requested.
- Render no logo, watermark, signature, color swatch, UI chrome, mockup frame, or unrelated explanatory prose.

## Aesthetic motive lock

Mode and device constraints may change placement and aspect ratio, never the 026 aesthetic motive. Every transformed frame must visibly express this chain: **this exact photographed subject or inseparable relationship → at least three source-specific identity cues → quiet reduction into simple geometry, fine structural lines, and generous negative space → a source-derived low-stimulation humanist palette → balanced rhythm with slight offsets and restrained positive/negative shape → barely raised or pressed paper depth → sparse editorial typography bound to the image's meaning**.

Reject a result as generic when its source could be replaced by an unrelated photo without materially changing the subject construction, spatial relationship, palette, line logic, or copy. Generic Bauhaus circles, pastel blobs, architecture-diagram decoration, sun-and-wave symbols, stock vector landscapes, or soft-colored wallpaper are not acceptable substitutes for a specific person, object, animal, building, gesture, or relationship. Device safe areas are secondary placement constraints; they must not erase source identity, quiet spatial hierarchy, subtle relief, main title, or editorial typography.

## Raster generation and privacy

### Model priority and credentials

- **Prefer GPT Image 2.** When GPT Image 2 is exposed through the host's built-in image tool or an already configured compatible route, use it before any other model. Preserve the current XXD execution contract: resolve the whole final canvas before generation, use the source as a high-fidelity reference, generate paired modes as one complete canvas, and keep deterministic composition as fallback only.
- Also support **Seedance 5.0 Pro**, **Nano Banana Pro (Gemini Image Pro)**, **Nano Banana 2 (Gemini Image Flash)**, or another compatible bitmap model when it is actually available through a tool or configured route and can satisfy the selected mode. Required capabilities include reference-image generation/editing, source fidelity, the resolved whole-canvas ratio, native target-language text, and multi-image reference input when a linked wallpaper pack needs it.
- Alternative models are secondary routes, not a different workflow. Do not let a model switch silently change the selected modes, final canvas, source-visibility rules, copy, locale, wallpaper relationship, fresh-task boundary, raster-only delivery, or the full-canvas-first strategy. If an alternative cannot satisfy a hard requirement, do not silently degrade that requirement.
- If no suitable route is available, ask the user to enable an image-generation tool or provide an API key. A user may voluntarily provide credentials for the current task. Accept them without echoing, displaying, logging, or reporting their value. Do not persist credentials or modify provider, account, billing, or global route configuration unless the user explicitly asks for that configuration change.
- Determine availability from an actual image-capability check. Do not declare GPT Image 2 or every other route unavailable merely because one tool is absent, one call failed, or one expected environment variable is unset.

Prefer GPT Image 2 through Codex's built-in `image_gen` capability when it is exposed, following the available `imagegen` skill for execution details. If a local source image must be used, view it first so it is visible to the built-in edit/generation flow. Issue one built-in call per distinct asset; a four-device wallpaper pack requires four separate calls, not one `n` request. In `linked`, one of those four outputs is the approved visual anchor—it is not an extra fifth master and never becomes a crop source. “Flat geometry,” “fine structural line,” “embossed paper,” or “vector-like edge” describes appearance only; it never authorizes SVG construction. Do not create or return SVG, HTML, CSS, Canvas, diagrams, hand-coded vector markup, or other code-rendered substitutes. Generate bitmap assets, move/copy selected outputs from Codex's generated-images location into the requested output directory, finalize them with `scripts/compose_panel.py`, and deliver PNG files. The script is only for deterministic raster planning, crop/paste, sizing, and audit—not for inventing the artwork.

Judge image-generation readiness by capability, not by a provider name or the presence of one particular environment variable. A missing environment variable is not proof that authentication or bitmap generation is unavailable: the host, an authenticated session, a credential store, a configured SDK, or another compatible route may already provide it. If built-in `image_gen` is not exposed, check only non-secret capability signals for an already configured bitmap route: compatible image model or endpoint, authenticated readiness, and actual PNG/raster output support. Do not hardcode or mention a specific proxy/provider in this policy.

When built-in `image_gen` is unavailable, use the bundled `scripts/configured_imagegen.py`; do not fall back first to a CLI that recognizes only one fixed environment variable. This bridge reuses the active Codex route in-process without changing global configuration:

```bash
# Readiness only: prints sanitized JSON, never route or credential details
python3 scripts/configured_imagegen.py probe

# This skill always has a source reference, so transformed assets use edit
python3 scripts/configured_imagegen.py edit --image source.png \
  --prompt-file /private/job-temp/transform-prompt.txt \
  --out /private/job-temp/design.png --size 1536x1024 --quality high
```

Use `generate` only for an asset that genuinely has no image reference. The bridge normalizes an API generation size when required and writes the requested final PNG dimensions. Keep the prompt file and generated intermediates in a per-job temporary directory outside the finished task directory, then remove the prompt file after the generation step. Do not pass provider settings, credentials, or full prompts as command-line values.

Protect provider identity and credentials throughout discovery and execution. Never display, echo, log, serialize, paste into chat, or include secret values in commands whose output may expose them. Also never report or persist provider names, endpoint URLs, IP addresses, domains, ports, request-header names or values, account identifiers, authentication modes, or credential-store contents. Do not open configuration or credential files for manual inspection or reporting; only the bundled bridge may resolve them internally for the authorized request. Do not run it with shell tracing, verbose HTTP output, environment dumps, `tee`, or process inspection. Its probe/output JSON is the entire allowed diagnostic surface: readiness, sanitized phase/reason, HTTP status, and final artifact path. Do not claim that a key is missing unless a trusted sanitized status explicitly establishes that fact, and never ask the user to paste a key into chat.

An explicit invocation of `/xxd-panel-026` or `$xxd-panel-026`, followed by the source image and requested mode, is the user's explicit confirmation to create the requested PNG deliverable through any already configured, authenticated raster route available to the session. This satisfies the `imagegen` skill's confirmation requirement for switching from an unavailable built-in tool to a compatible configured CLI/API route. Do not ask for a second confirmation merely because the execution route changes. This authorization is limited to the requested image generation: it does not authorize adding or changing credentials, providers, accounts, billing, or global configuration.

Only report image generation as unavailable after built-in capability and `scripts/configured_imagegen.py probe` both fail to establish a usable bitmap route. State the verified limitation narrowly instead of guessing its cause, and refer only to the “configured bitmap route”—never identify the provider. Never silently substitute SVG or programmatic drawing, and never modify credentials, provider settings, accounts, billing, or global environment variables as a workaround.

## Fresh-task and source boundary

Every invocation is a new generation job unless the user explicitly asks to continue, audit, review, edit, or reuse a named earlier result. Repeating the same source, mode, dimensions, or wording means **generate a fresh result**, not return or re-audit a matching old file. Resolve the next unused task-directory name before generation and write the new deliverable there; an existing result can never satisfy the current job.

Build the source set only from images attached to the current invocation, paths explicitly supplied by the user, or earlier user-supplied source images that the current request explicitly identifies with wording such as “same image” or “again.” A conversation attachment remains the intended source even when it has no usable local filesystem path. Do not replace it with an arbitrary workspace file.

Never scan the Desktop, current workspace, default output root, or unrelated folders broadly to find “some image” when a source is missing. Files under `~/Desktop/xxd/xxd-panel-026/`, task directories created by this skill, and files carrying this skill's output suffixes are historical outputs, not source candidates. Do not inspect or reuse them unless the user explicitly names one as an input or asks for comparison/review. If the intended source cannot actually be accessed, ask for that source or its path; do not improvise from an existing poster.

Do not downgrade a new generation request into validation of an old artifact. If no usable raster route is verified, report only that verified execution limitation; never present an earlier file's dimensions, seam audit, or visual review as completion of the new job.

## Workflow

1. Resolve one or more modes. If missing, ask exactly this as normal multiline chat text and wait:

   ```text
   请选择一个或多个模式（回复序号；多选可用 +、顿号或逗号）：

   1. 上下双联（原图在上＋026 设计在下）
   2. 左右双联（原图在左＋026 设计在右）
   3. 纯设计版（只显示 026 设计画面）
   4. 四端壁纸套装
      手机＋iPad＋电脑＋儿童手表

   示例：1｜1+3｜1、2、4｜全部
   ```

2. Before any ordinary-mode generation, explicitly resolve the **final finished canvas**, not the size of one panel. If the user did not already supply a ratio or exact pixels, ask and wait:

   ```text
   请选择最终成品画幅（回复序号即可；多选模式可共用，也可分别指定）：

   1. 原提示词画幅 3:4
   2. 跟随原图比例
   3. 常用比例
      1:1｜4:5｜2:3｜3:2｜16:9｜9:16
   4. 自定义比例或准确像素

   这里指整张最终成品的比例，不是单个区域。
   示例：1｜3：9:16｜4：2160×3840
   ```

   “跟随原图比例” is valid only when the user explicitly selects it. Never infer a silent canvas from the source dimensions, orientation, archived 3:4 brief, mode, or previous output. In multi-select, ask which mode an ambiguous ratio belongs to. Exact pixels take priority over a chosen ratio. For paired modes, odd split axes are allowed for direct generation; require an even split axis only if deterministic fallback composition is actually triggered.

3. Before generation, resolve copy mode and locale. If missing, ask and wait:

   ```text
   正式做图前，请确认文字设置（回复序号即可）：

   1. 自动文案
      我根据原图与 026 气质创作文案；请同时注明语言或地区
   2. 自定义文案
      请直接输入要呈现的准确文字，并注明语言或地区
   3. 无文字

   示例：1｜日语
   示例：2｜英式英语｜STILL IN BLOOM
   ```

   Automatic copy must be source-specific and native to the resolved locale. Preserve exact custom copy verbatim. Do not infer locale from appearance, clothing, scenery, filenames, metadata, or visible signs.

4. Only when `wallpaper-pack` is selected, resolve its relationship and device sizes. Ask for `1. 连贯套装` or `2. 四张独立` when missing. A linked set approves one iPad anchor by default; the other three outputs each reference the original plus that same anchor and are independently recomposed. An independent set gives every device only the original. Then ask for either the common preset—phone `1440×3200`, iPad `2048×2732`, desktop `3840×2160`, watch `1024×1024`—or labelled custom pixels. Never crop one wallpaper into another or chain derivatives.

5. Start a fresh job and reserve collision-safe output directories before generation. Use only the current invocation's explicit source or theme. Read `references/xxd-panel-026-prompt.en.md` or `references/xxd-panel-026-prompt.zh-CN.md` immediately before building the generation request.
6. Privately lock the principal subject or inseparable relationship, at least three source-specific recognition cues, the style's complete aesthetic motive, composition logic, materials, palette, typography, exact copy, and locale. The source photograph is the factual and identity anchor; do not borrow content from samples or old outputs.
7. Use **single complete-canvas generation as the default for every mode**:
   - `top-bottom`: supply the source as a high-fidelity edit/reference input and generate one finished image containing the faithful source in the upper half and the 026 transformation in the lower half.
   - `left-right`: supply the source as a high-fidelity edit/reference input and generate one finished image containing the faithful source on the left and the 026 transformation on the right.
   - `design-only`: generate the 026 transformation across the whole canvas; the source is reference-only and not visible.
   - `wallpaper-pack`: generate four separate complete canvases, one per device, following the resolved independent or linked relationship.
8. Append the complete-canvas payload below to the full local style prompt. Keep all 026-specific aesthetic and typography instructions active across the entire composition. For paired modes, ask for approximately equal regions while prioritising a coherent finished artwork: colour, light, rhythm, typography, meaning, and any cross-panel echo must feel intentionally unified.
9. Generate each distinct output as a fresh raster image job. Do not request two separate half-images, a contact sheet, a mockup, an empty reserved panel, or a code-rendered substitute.
10. Inspect the actual bitmap at full size and thumbnail size. Check, in order: whole-poster integration; 026 aesthetic fidelity; source identity and structure; visual and semantic correspondence between regions; typography and locale; mode, ratio/pixels, count, and PNG format; then approximate 50/50 geometry.
11. If a paired result fails a hard requirement, retry the **complete canvas once**, changing only the failed constraint. Use `scripts/compose_panel.py` only after that retry still fails, or when the user explicitly requires pixel-identical source preservation, the active image route cannot realise the selected canvas, the requested ratio exceeds route limits, or final lossless pixel calibration is necessary. The script is a fallback utility, never the default creative path and never an aesthetic judge.
12. Reopen every final PNG, apply the acceptance gate, and return absolute paths in source order and mode order 1→4. Wallpaper order is phone, iPad, desktop, watch.

## Complete-canvas generation payload

Append one resolved block to the style prompt for each output:

```text
OUTPUT MODE: TOP_BOTTOM | LEFT_RIGHT | DESIGN_ONLY | WALLPAPER_PACK
DEVICE PROFILE: NONE | PHONE | IPAD | DESKTOP | WATCH
FINAL CANVAS: <whole finished ratio and/or exact WIDTHxHEIGHT>
GENERATION STRATEGY: SINGLE COMPLETE CANVAS
REFERENCE ROLE: SOURCE — HIGH-FIDELITY CONTENT AND IDENTITY ANCHOR
SOURCE VISIBILITY: UPPER 50% | LEFT 50% | REFERENCE ONLY — NOT VISIBLE
LAYOUT RULE:
- Produce one finished poster in one image.
- TOP_BOTTOM keeps a faithful photographic source in the upper half and creates the transformed design in the lower half.
- LEFT_RIGHT keeps a faithful photographic source in the left half and creates the transformed design in the right half.
- DESIGN_ONLY and WALLPAPER_PACK use the whole canvas for the transformed design and show no source photograph or reserved panel.
- Keep paired regions approximately equal while unifying colour, light, rhythm, typography, and meaning.
- Do not output separate panels, a contact sheet, a mockup, or an empty placeholder.
WALLPAPER RELATIONSHIP: NONE | INDEPENDENT | LINKED
ANCHOR DEVICE: NONE | IPAD
```

For text output append:

```text
COPY MODE: REQUIRED
COPY ORIGIN: USER_EXACT | USER_DIRECTION | SOURCE_DERIVED
COPY LOCALE: <resolved locale>
COPY PAYLOAD: <the exact 026-specific title and supporting-text package resolved under the local production prompt>
COPY RULE: Render only the populated strings in COPY PAYLOAD, each exactly once. Do not rewrite, translate, spell-correct, duplicate, or add text. Use native shaping, direction, punctuation, spacing, and semantic line breaks. Preserve the 026-specific hierarchy, amount of supporting text, placement, material, and typographic role instead of applying a generic overlay.
```

For text-free output append only `COPY MODE: NONE — render no text or pseudo-text anywhere.`

## Composition fallback only

`scripts/compose_panel.py` remains available for deterministic recovery and audit. Trigger it only under step 11. When used, generate a same-aspect design asset from the full 026 prompt, preserve the source without destructive crop or stretch, and document which fallback condition applied. A direct complete-canvas success must not be split and recomposed again.

```bash
# Read-only audit after direct generation
python3 scripts/compose_panel.py --audit final.png --layout top-bottom --size WIDTHxHEIGHT

# Deterministic fallback after the complete-canvas retry has failed
python3 scripts/compose_panel.py --source photo.png --design design.png \
  --out final.png --layout top-bottom --size WIDTHxHEIGHT
```

## Output location

Save every generated poster under `~/Desktop/xxd/xxd-panel-026/`. Create the shared `~/Desktop/xxd/` wrapper, the skill root, and the task directory if they do not exist.

- Wrap each source-and-mode result in one task directory: `<source-stem>-top-bottom/`, `<source-stem>-left-right/`, `<source-stem>-design-only/`, or `<source-stem>-wallpaper-pack/`. A batch or multi-select creates one sibling task directory per source and selected mode; never mix different sources in one directory.
- Inside an ordinary-mode task directory, name the single final PNG after the source (`IMG_4821.png`), append `-lr` for `left-right`, or append `-design` for `design-only`.
- Inside a wallpaper-pack task directory, keep exactly four finished PNGs named with `-wallpaper-phone`, `-wallpaper-ipad`, `-wallpaper-desktop`, and `-wallpaper-watch`. Do not create four device subdirectories and do not mix another source's files into the pack.
- When the source has no usable name, use the short title slug as `<source-stem>`.
- Never overwrite an existing task directory. On collision append `-2`, `-3`, and so on to the task-directory name; keep filenames inside unchanged.
- Keep temporary generations, plans, audits, and source copies out of the finished task directory. It contains final deliverable PNGs only.
- An explicit user file path overrides this default exactly. When the user supplies only a destination directory, create the same per-source-and-mode task directories inside it unless the user explicitly requests a flat directory.

## Acceptance gate

Before accepting each result, verify all of the following:

- The output mode and dimensions match the resolved explicit selection or explicit final-canvas ratio or pixels. `--size` is reproduced pixel-for-pixel. When the user explicitly chooses source aspect, the source is never cropped and the generated asset either matches the planned frame natively or is proportionally resampled from the same aspect with no crop.
- `top-bottom` has a clean near-central horizontal relationship; `left-right` has a clean near-central vertical relationship; `design-only` and all wallpaper files contain no seam or visible source photo.
- In paired modes, the photographic panel remains recognizably the original source, appears in the correct upper/left position, and contains no deformation or typography.
- The transformed region depicts the same key subject and relationship through simplified silhouette, gentle geometric planes, fine contour/structural lines, and source-specific spacing.
- Automatic or direction-led copy expresses a visible fact plus a grounded relational or latent meaning, passes the unrelated-photo swap test, and earns its emotional turn without a forced pun or invented backstory. Its language matches the resolved target locale rather than the command language or presumed identity: Arabic reads as native Arabic with connected shaping and RTL composition, Japanese as native Japanese, Korean as native Korean, and UK English uses British conventions. Exact user copy remains verbatim and its hierarchy, script shaping, punctuation, line breaks, and placement preserve the intended emphasis; editable user direction is transcreated only within the permission given.
- The transformed construction feels balanced, quiet, and human rather than rigidly symmetric: one clear core, generous negative space, measured density, slight offsets, and only shallow pressed-paper or low-relief depth.
- The palette contains 4–6 source-derived low-stimulation colors translated toward warm white, sand, dusty pink, pale ochre, mist blue, sage, or adjacent hues; it avoids neon, dirty grey distortion, cold tech color, complex gradients, and cheap commercial styling.
- In automatic or direction-led copy mode, the transformed design contains the locked main title and all 2–4 locked microtext strings. In custom-copy mode, it contains the exact title plus every populated or derived microtext string, or the exact title alone when title-only was explicitly requested. All rendered wording is accurate, with no substitution, misspelling, gibberish, extra wording, or invented year; the main title is visually unmistakable and at least three times the microtext scale. In text-free mode, no letters, numbers, captions, or pseudo-text appear anywhere.
- Typography follows contours, structural axes, or quiet margins and participates in the geometry without becoming a UI panel, commercial title bar, or template.
- The artwork was reopened and visually inspected. It preserves at least three source-specific identity cues and the principal relationship; generic pastel blobs, Bauhaus decorations, architecture-diagram marks, or stock vector scenery cannot substitute for the actual source content.
- Each wallpaper has its requested exact dimensions, its own aspect-specific composition, usable safe regions, no baked-in system UI, and no evidence of being mechanically cropped from another device output.
- In `independent`, all four wallpapers derive directly from the original source and may explore freer compositions without borrowing a generated wallpaper. In `linked`, the anchor passed its gate before fan-out, the other three all reference the original source plus that same anchor, and the four preserve one recognizable family of soft palette, geometric reduction, line grammar, paper relief, typography, and copy without becoming resized duplicates.
- The final count per source equals one file for each selected ordinary mode plus four files when `wallpaper-pack` is selected. `all` / `全部` therefore means seven finished PNGs across four sibling task directories, with no content borrowed from other inputs.
- Every delivered file was newly generated or composed for this invocation and lives in the fresh task directory reserved for it; no historical output was returned as the current result.

## Override policy

Preserve user-specified subject wording, output count, target locale, and language. Copy priority is explicit text-free request > exact supplied wording > supplied creative direction > automatic source-derived copy. Target-locale priority is explicit audience/market > explicit output language > direction language; if none is explicit, ask before generation. Treat exact wording as immutable unless the user asks for rewriting or localization. Apply a shared creative direction across a batch when requested, but still write a distinct source-aware copy package for each photo unless the user explicitly requests identical wording.

A user-forced mode set and per-mode exact pixel sizes are always honored. Exact size takes precedence over an explicitly chosen ratio; neither may be inferred silently. Canvas orientation never changes any selected mode: `top-bottom` always stacks vertically, `left-right` always places source left and design right, and source-hidden modes never reintroduce the photograph. In `wallpaper-pack`, a labeled device size overrides only that device. If a paired frame fights the source orientation, protect the subject with seamless environmental extension rather than stretching it.

Do not relax the one-photo-per-selected-ordinary-mode rule, exact four-output rule in `wallpaper-pack`, the paired-mode relationship and any explicitly requested exact split, absence of the photo in source-hidden modes, faithful visible photography, or the photo-derived humanist geometry unless the user explicitly asks to leave the 026 style.

## Provenance boundary

The original user style brief is archived at [references/026-source.md](references/026-source.md). Use [assets/examples](assets/examples) only as visual examples; never borrow their subjects, colors, copy, or composition unless the user supplies that exact image. The operative visual specification is the local 026 reference prompt.
