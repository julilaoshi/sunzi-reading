# Sunzi Reading / 孙子读论文

<p align="center">
  <strong>Papers are not always hard because the ideas are hard.</strong><br />
  Sometimes they are hard because they refuse to speak human.
</p>

<p align="center">
  <a href="./prompts/sunzi_reading_prompt_en.md"><img alt="Copy Prompt" src="https://img.shields.io/badge/Copy-Prompt-d14836?style=for-the-badge" /></a>
  <a href="#install-the-skill"><img alt="Install Skill" src="https://img.shields.io/badge/Install-Skill-2ea44f?style=for-the-badge" /></a>
  <a href="./skill/SKILL.md"><img alt="Read Skill" src="https://img.shields.io/badge/Read-Skill-1f6feb?style=for-the-badge" /></a>
  <a href="https://github.com/julilaoshi/sunzi-reading"><img alt="Star Repo" src="https://img.shields.io/badge/Star-Repo-f6c343?style=for-the-badge&logo=github&logoColor=111111" /></a>
  <a href="#two-ways-to-use-it"><img alt="Start Here" src="https://img.shields.io/badge/Start-Here-111111?style=for-the-badge" /></a>
</p>

<p align="center">
  Public <code>v1.0</code> now. The stronger versions shown in my own workflow may use more examples, upstream research judgment, and other linked skills.
</p>

[简体中文](./README.md) | English

**Sunzi Reading** is a copyable prompt and public-safe skill that turns dense academic papers into short, accurate, gently funny explanations for beginners: like a patient elder explaining a paper to a beloved grandchild.

## Start Here

- [Copy the English prompt](./prompts/sunzi_reading_prompt_en.md)
- [Copy the Chinese prompt](./prompts/sunzi_reading_prompt.md)
- [Install into Codex](#install-the-skill)
- [Read the public skill file](./skill/SKILL.md)
- [Star the repository](https://github.com/julilaoshi/sunzi-reading)

## Install The Skill

If you only want to try this in ChatGPT, Claude, DeepSeek, or Doubao, copy the prompt. No installation is needed.

If you use Codex, open a new Codex chat, paste the text below, and press Enter:

```text
Please install this Codex Skill from GitHub:
https://github.com/julilaoshi/sunzi-reading/tree/main/skill

After installing it, tell me whether I need to restart Codex.
```

Restart Codex after installation. Then ask Codex to use Sunzi Reading on a paper.

If you prefer manual terminal installation:

```bash
mkdir -p "$HOME/.codex/skills"
test ! -e "$HOME/.codex/skills/sunzi-reading" || { echo "sunzi-reading already exists; not overwriting"; exit 1; }
tmpdir="$(mktemp -d)"
git clone --depth 1 https://github.com/julilaoshi/sunzi-reading.git "$tmpdir/sunzi-reading"
cp -R "$tmpdir/sunzi-reading/skill" "$HOME/.codex/skills/sunzi-reading"
```

## Two Ways To Use It

This is not an npm package. You do not need `npm install`. You can either copy the prompt or install the Skill into Codex.

### 1. Beginner mode: copy the prompt

- [`prompts/sunzi_reading_prompt_en.md`](./prompts/sunzi_reading_prompt_en.md)

Paste it into ChatGPT, Claude, DeepSeek, Doubao, or another model that can read your paper text, abstract, screenshots, or PDF content.

Then send a paper and ask it to explain.

This is the fastest way to try Sunzi Reading.

### 2. Stable mode: use the Skill

- [`skill/SKILL.md`](./skill/SKILL.md)

Use the Skill when you want Sunzi Reading to behave like a repeatable workflow, not just a one-time prompt.

The Skill is better than the prompt when you need:

- the same output structure every time
- clearer boundaries around what the paper proves and does not prove
- fewer long, drifting answers
- safer public examples without copyrighted full-text papers
- a reusable method that a coding agent can apply across files, READMEs, examples, and release checks

The prompt is for quick use.

The Skill is for repeatable work.

## What It Does

- Explains a paper in plain language.
- Keeps the answer short and accurate.
- Translates scary terms into human words.
- Adds light talk-show rhythm without turning the paper into a joke.
- Gives emotional support: "don't panic, this paper is written weirdly."
- Marks what the paper proves, what it does not prove, and where beginners may misread it.

## Included

```text
agents/
  openai.yaml
prompts/
  sunzi_reading_prompt.md
  sunzi_reading_prompt_en.md
skill/
  SKILL.md
examples/
  microplastics_tetracycline_demo.md
```

## Not Included

- No paper downloader.
- No PDF parser.
- No private datasets.
- No copyrighted full-text papers.
- No promise that the model is always correct.

Use it as a reading assistant, not as a substitute for checking the paper.

## Why The Social Media Version May Look Stronger

This public repository focuses on the reusable prompt and public Skill.

In my own workflow, the stronger version may also use:

- more paper-reading context
- more examples and prompt tests
- upstream research judgment
- video writing and publishing skills
- more internal notes and intermediate assets

So the public version is real, but it is intentionally light.

It gives you the method, not my entire private workflow.

## Structure

- `prompts/sunzi_reading_prompt_en.md` - copyable English prompt
- `prompts/sunzi_reading_prompt.md` - copyable Chinese prompt
- `skill/SKILL.md` - public Skill file
- `agents/openai.yaml` - skill UI metadata
- `examples/` - public-safe examples
- `GITHUB_ABOUT_SUGGESTION.md` - suggested GitHub About text and topics
- `PUBLIC_RELEASE_CHECKLIST.md` - pre-publish checklist

## Language Strategy

- English README is optimized for GitHub visitors.
- Chinese README keeps fuller context and platform information.
- The project name keeps the Chinese joke, because that is the strongest signal.

## License And Brand Boundary

The reusable prompt, docs, and framework are released under the MIT License.

Brand-facing identity and endorsement implications are not automatically transferred with that license. See [`BRAND_NOTICE.md`](./BRAND_NOTICE.md).

## Internal vs Public Boundary

The public version keeps:

- method
- prompt
- public Skill
- reusable explanation structure
- public-safe demo

The public version does not keep:

- private paper libraries
- private workflow traces
- full copyrighted papers
- internal prompt chains
- social media production drafts

## License

Code and public text are released under the MIT License.

The project name, creator identity, and brand presentation are covered by [`BRAND_NOTICE.md`](./BRAND_NOTICE.md).

## Find Juli

<p align="center">
  <a href="https://github.com/julilaoshi"><img alt="Follow Juli on GitHub" src="https://img.shields.io/badge/Follow%20Juli-on%20GitHub-111111?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://github.com/julilaoshi/sunzi-reading"><img alt="Star Sunzi Reading" src="https://img.shields.io/badge/Star-Sunzi%20Reading-f6c343?style=for-the-badge&logo=github&logoColor=111111" /></a>
</p>

| Platform | Identity |
| --- | --- |
| X / Twitter | [@julilaoshi](https://x.com/julilaoshi?s=21) |
| Instagram | [@julilaoshi](https://www.instagram.com/julilaoshi?igsh=d2lhZmhoMzNlOTlk&utm_source=qr) |
| YouTube | [@julilaoshi](https://www.youtube.com/@julilaoshi) |
| Red Book | [居里老师](https://xhslink.com/m/ArTQH4nAado) |

## Release Helpers

- [`GITHUB_ABOUT_SUGGESTION.md`](./GITHUB_ABOUT_SUGGESTION.md)
- [`PUBLIC_RELEASE_CHECKLIST.md`](./PUBLIC_RELEASE_CHECKLIST.md)
