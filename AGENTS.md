# Build with Gemini Lightning Talks

Denny Huang's stage talk is in Taiwan Traditional Chinese. Edit `slide.md` and preserve the running order unless the author asks to change it.

## Denny's slide voice

### Slide body

Each slide should first show the thing the audience needs to locate, type, compare, or check. Denny can explain why live.

`README prose -> cue / artifact / command / contrast / expected output / 檢核點`

- One core concept per slide. Give every slide one visible anchor so the audience knows where they are.
- Usually use 0–4 bullets, a short question, an image, a URL, a small table, or a chart. A title-only beat can work between denser slides.
- Use `### 重點` or an equivalent summary cue only after the artifact or demo target is visible.
- Prefer active, direct phrasing. Use short topic titles or questions Denny can say on stage.
- Keep slide text in Taiwan Traditional Chinese. Keep technical terms in English when they are standard in practice, optionally paired with a Traditional Chinese explanation on first use.

Avoid mini articles, marketing tone, motivational filler, inflated claims, and polished documentation voice. Do not replace concrete evidence with abstract summaries, explain away all whitespace, or add text merely because an idea feels important. Avoid definition-first slides when an example works, objective-summary titles such as `建立…` / `說明…` / `提升…` / `確保…`, and `透過…來…` sentences with no concrete decision or evidence.

In this deck, `同一份 diff，閱讀體驗差多少？` gives the audience a question the two screenshots can answer. A demo can pair `git worktree list` with its output. A short transition can leave room for a pause. Keep installation steps and audience exercises out of the stage talk.

### Revision order

1. Delete.
2. Shorten.
3. Replace with words Denny would say live.
4. Turn explanation into a cue, artifact, contrast, decision, or checkpoint.
5. Add explanation only when the audience would be blocked without it.

### Questions to ask while editing

- Does the audience need to see this now, or can it be spoken live?
- Is there a visible anchor, with enough context to interpret it?
- For collaboration slides, is the human/tool boundary visible?

## Editing and verification

- Keep the slide URL and QR code together after the cover. Preserve the speaker's bio, the closing credits and the original sources for third-party media.
- Use real captures for demos. When comparing Git and delta, show the same diff at the same terminal width. Keep demos in `assets/demo/` so they work offline.
- Build with `marp slide.md -o index.html` from the project root. After changing the cover, regenerate its sharing image with `marp slide.md --image jpeg --allow-local-files -o assets/og-image.jpg`.
- Check the rendered slides for Chinese line breaks, legible demos and working links. Verify that the QR code and canonical URL lead to the published deck.
