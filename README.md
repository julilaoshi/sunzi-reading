# 孙子读论文 / Sunzi Reading

<p align="center">
  <strong>论文不一定是你读不懂。</strong><br />
  有时候是它明明能说人话，但它偏不。
</p>

<p align="center">
  <a href="./prompts/sunzi_reading_prompt.md"><img alt="复制提示词" src="https://img.shields.io/badge/复制-提示词-d14836?style=for-the-badge" /></a>
  <a href="./skill/SKILL.md"><img alt="阅读 Skill" src="https://img.shields.io/badge/阅读-Skill-1f6feb?style=for-the-badge" /></a>
  <a href="https://github.com/julilaoshi/sunzi-reading"><img alt="给仓库点星" src="https://img.shields.io/badge/给仓库-点星-f6c343?style=for-the-badge&logo=github&logoColor=111111" /></a>
  <a href="#两种用法"><img alt="从这里开始" src="https://img.shields.io/badge/从这里-开始-111111?style=for-the-badge" /></a>
</p>

<p align="center">
  当前公开的是 <code>v1.0</code>。我自己工作流里更强的版本，可能还会用到更多样张、上游研究判断和其他联动 Skill。
</p>

简体中文 | [English](./README.en.md)

**孙子读论文** 是一个可复制 Prompt 和 public 版 Skill：把复杂论文讲成短、准、有人味的解释，像一个有学问、有耐心、还会哄人的长辈，在给小孙子讲论文。

## 快速开始

- [复制提示词](./prompts/sunzi_reading_prompt.md)
- [阅读公开版 Skill 文件](./skill/SKILL.md)
- [给仓库点星](https://github.com/julilaoshi/sunzi-reading)

## 两种用法

这不是 npm 包，不需要安装。

### 1. 初级用法：直接复制提示词

- [`prompts/sunzi_reading_prompt.md`](./prompts/sunzi_reading_prompt.md)

把它粘贴到 ChatGPT、Claude、DeepSeek、豆包，或者任何能读论文内容的模型里。

然后发论文摘要、论文截图、PDF 内容或学术段落，让它解释。

这是最快的用法，复制就能试。

### 2. 稳定用法：使用这个 Skill

- [`skill/SKILL.md`](./skill/SKILL.md)

如果你只是偶尔读一篇论文，用提示词就够了。

如果你希望它每次都稳定地按同一个方法读论文，就用 Skill。

Skill 比单独提示词更好的地方是：

- 输出结构更稳定，不容易跑成普通论文摘要。
- 会固定检查“作者证明了什么 / 没证明什么”。
- 会固定提醒哪里容易误读。
- 更适合反复处理多篇论文、多个示例和 GitHub 发布材料。
- 更容易约束公开边界，不把论文全文、私有材料或不该公开的内容带出去。

提示词适合立刻用。

Skill 适合长期复用。

## 它能帮你做什么

- 把论文讲成人话。
- 保持短、准，不写成长篇综述。
- 把吓人的术语拆开。
- 加一点脱口秀节奏，但不为了搞笑乱说。
- 加一点“乖，别怕”的情绪价值，但不油腻。
- 标出作者证明了什么、没证明什么、哪里最容易误读。

## 仓库包含什么

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

## 仓库不包含什么

- 不包含论文下载器。
- 不包含 PDF 解析器。
- 不包含私有数据集。
- 不包含受版权保护的论文全文。
- 不保证模型永远正确。

它是阅读辅助，不是替代你核对论文。

## 为什么我自媒体里的版本可能更强

这个 public 仓主要公开的是可复制提示词和公开版 Skill。

我自己工作流里更强的版本，可能还会用到：

- 更多论文阅读上下文
- 更多样张和 Prompt 测试
- 上游研究判断
- 视频写作和发布 Skill
- 更多内部笔记和中间资产

所以公开版是真的，但它是轻量版。

它给你方法，不等于把我的整套私有工作流都打包出来。

## 仓库结构

- `prompts/sunzi_reading_prompt.md`：可复制提示词
- `prompts/sunzi_reading_prompt_en.md`：英文版可复制提示词
- `skill/SKILL.md`：公开版 Skill 文件
- `agents/openai.yaml`：Skill 展示元数据
- `examples/`：公开安全示例
- `GITHUB_ABOUT_SUGGESTION.md`：GitHub About 和 topics 建议
- `PUBLIC_RELEASE_CHECKLIST.md`：推送前检查表

## 语言策略

- 英文 README 更适合给 GitHub 公共访客快速理解。
- 中文 README 保留更完整的语境和平台信息。
- 项目名保留中文梗，因为这是最强识别点。

## 许可与品牌边界

可复用提示词、文档和框架按 MIT License 发布。

但作者身份、品牌呈现和背书关系不会随 MIT License 自动转让，详见 [`BRAND_NOTICE.md`](./BRAND_NOTICE.md)。

## 内部版与公开版边界

公开版保留：

- 方法
- 提示词
- 公开版 Skill
- 可复用解释结构
- 公开安全样例

公开版不保留：

- 私有论文库
- 私有工作流痕迹
- 受版权保护的论文全文
- 内部提示词链
- 自媒体生产草稿

## 许可

公开文本与代码按 MIT License 发布。

项目名称、作者身份和品牌展示边界见 [`BRAND_NOTICE.md`](./BRAND_NOTICE.md)。

## 找到居里老师

<p align="center">
  <a href="https://github.com/julilaoshi"><img alt="关注 GitHub" src="https://img.shields.io/badge/关注-GitHub-111111?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://github.com/julilaoshi/sunzi-reading"><img alt="给仓库点星" src="https://img.shields.io/badge/给仓库-点星-f6c343?style=for-the-badge&logo=github&logoColor=111111" /></a>
</p>

| 平台 | 账号 / 入口 |
| --- | --- |
| 推特 / X | [@julilaoshi](https://x.com/julilaoshi?s=21) |
| Instagram / INS | [@julilaoshi](https://www.instagram.com/julilaoshi?igsh=d2lhZmhoMzNlOTlk&utm_source=qr) |
| YouTube | [@julilaoshi](https://www.youtube.com/@julilaoshi) |
| B站 | [居里老师](https://space.bilibili.com/522623529) |
| Red Book | [居里老师](https://xhslink.com/m/ArTQH4nAado) |
| 公众号 | `居里生成` |
| 视频号 | `居里老师` |

## 发布辅助文件

- [`GITHUB_ABOUT_SUGGESTION.md`](./GITHUB_ABOUT_SUGGESTION.md)
- [`PUBLIC_RELEASE_CHECKLIST.md`](./PUBLIC_RELEASE_CHECKLIST.md)
