# 📚 STREAMING Learning Content for Africa

**Collaboratively creating, translating, and maintaining open training content for the African continent — powered by Markdown.**

---

## 🌍 Background

This repository is part of the [STREAMING](https://www.2023streaming.eu/) project, which aims to strengthen African food supply chains through capacity building, knowledge sharing, and the adoption of global standards. A key enabler is high-quality, up-to-date training content that can be delivered across diverse contexts — from fully-fledged e-learning platforms to individual self-study.

Rather than locking content into proprietary formats or complex authoring tools, we take a radically simple approach: **plain Markdown files**, collaboratively maintained on GitHub, that can be transformed into multiple output formats with minimal effort.

---

## 🎯 Requirements

Any solution for collaboratively maintaining training content at scale must meet the following criteria:

| # | Requirement | Description |
|---|-------------|-------------|
| 1 | **Multi-channel delivery** | Content must work for learning platforms (e.g. as SCORM packages), for trainers (e.g. as presentation slides), and for individuals (e.g. as readable web pages). |
| 2 | **Multi-language support** | Translations must be managed efficiently — avoiding duplication and ensuring that the same language is translated only once, regardless of how many courses use the content. |
| 3 | **Version control** | Every change must be traceable. Contributors need to see what changed, when, and by whom. |
| 4 | **Up-to-dateness** | The workflow must make it straightforward to keep content current and to retire obsolete material, so learners always access the latest version. |
| 5 | **Open-source ethos** | All training content is intended to be open source, inviting contributions from a global community of domain experts, trainers, and translators. |
| 6 | **Low barrier to entry** | Contributors should not need expensive software licences or advanced technical skills to participate. |
| 7 | **Scalability** | The approach must scale from a handful of modules to hundreds, across multiple languages and regions. |
| 8 | **Offline capability** | Given that network access in parts of Africa can be limited or intermittent, content and tooling should work reliably offline. |
| 9 | **AI readiness** *(exploratory)* | The content format should lend itself to future AI-assisted workflows — e.g. automated translation suggestions, content summarisation, or intelligent tutoring. |

---

## 💡 Solution Approach

### Markdown as the Single Source of Truth

We use **Markdown** — a lightweight markup language that virtually anyone can learn within five minutes. For instance:

- `#` denotes a first-level heading
- `*` creates an unordered list item
- `**bold**` makes text **bold**

That's nearly all you need to know to start contributing.

Each training module is maintained as a single `.md` file (or a small set of files) in this repository. From this single source, multiple output formats are generated:

```
                    ┌──────────────────────────┐
                    │   Markdown Source File    │
                    │  (single source of truth) │
                    └────────┬─────────────────┘
                             │
              ┌──────────────┼──────────────────┐
              ▼              ▼                   ▼
     🌐 HTML Page      📊 PPTX Slides      📦 SCORM Package
    (self-study &      (trainers adapt      (learning platforms
     reference)        look & feel)          e.g. Moodle)
```

### How It Works for Different Audiences

| Audience | Workflow |
|----------|----------|
| **Individuals & self-learners** | Simply view the Markdown file on GitHub — it is automatically rendered as a nicely formatted HTML page. No tools required. |
| **Trainers** | Install the free [Marp](https://marp.app/) extension for Visual Studio Code, then export the Markdown file to PPTX. Adapt colours, fonts, and branding to your own look and feel. |
| **Learning platforms** | Convert Markdown to SCORM-compliant packages for import into platforms such as Moodle, TalentLMS, or similar. |

### The Marp Framework

[Marp](https://marp.app/) (Markdown Presentation Ecosystem) is a free, open-source framework that turns Markdown files into presentation slides. It integrates seamlessly with Visual Studio Code and supports:

- Slide separation via `---` dividers
- Custom themes and styling via CSS
- Export to **PPTX**, **PDF**, and **HTML**
- Speaker notes

> ℹ️ **Note:** All training content in this repository is released as open source. You are free to use, adapt, and redistribute it.

---

## ✅ Why Markdown? Advantages over Alternative Approaches

### Compared to PowerPoint-only Workflows

| Aspect | PPTX-only | Markdown + Marp |
|--------|-----------|-----------------|
| **Version control** | PPTX is a binary format — Git cannot show meaningful diffs. Tracking changes requires manual effort or clunky "track changes" features. | Markdown is plain text. Every change is visible line-by-line in Git, with full history and attribution. |
| **Collaboration** | Simultaneous editing is difficult. Files are typically e-mailed back and forth, leading to `v2_final_FINAL.pptx` chaos. | Contributors open pull requests on GitHub. Changes are reviewed, discussed, and merged in a transparent workflow. |
| **Translation** | Each language requires a separate PPTX file. Updates to the source must be manually propagated to every translation — an error-prone process that rarely stays in sync. | Translations live alongside the source in a structured folder hierarchy. Changes to the source are flagged automatically, making it clear which translations need updating. |
| **Tooling cost** | Requires Microsoft Office or a compatible suite. | Requires only a free text editor (e.g. Visual Studio Code). |
| **Reusability** | Content is trapped inside slides. Extracting text for other purposes (e.g. a website, a chatbot, a printed handbook) is cumbersome. | Markdown is format-agnostic. The same content can be rendered as slides, a web page, a PDF, or fed into an AI pipeline. |
| **File size & bandwidth** | PPTX files with images can be large — a real concern in low-bandwidth environments. | Markdown files are tiny. Images are referenced, not embedded, keeping repositories lean. |

### Compared to Professional E-Learning Authoring Tools (e.g. Articulate Storyline)

| Aspect | Authoring tools | Markdown + Marp |
|--------|----------------|-----------------|
| **Cost** | Commercial licences can run to hundreds of euros per seat per year. | Entirely free and open source. |
| **Learning curve** | Significant — often requiring dedicated training for content authors. | Minimal — Markdown syntax can be learnt in minutes. |
| **Community contributions** | Impractical. Contributors would need the same (paid) software and training. | Anyone with a text editor and a GitHub account can contribute. |
| **Portability** | Content is often locked into proprietary formats. Migrating to a different platform may require rebuilding from scratch. | Markdown is a universal, platform-independent format. |
| **Maintenance** | Updates require opening the authoring tool, navigating complex project structures, and re-publishing. | Updates are a simple text edit, committed via Git. |
| **Suitability** | Ideal for highly interactive, multimedia-rich courses. | Ideal for knowledge-transfer content, reference material, and structured training modules — which is the majority of what we need. |

> 💡 **In short:** We are not building a flashy e-learning product. We are building a **sustainable, community-maintained knowledge base** that can be delivered in whatever format the audience needs. Markdown gives us the simplest possible foundation for that goal.

---

## ✏️ Editing Content

### Getting Started

1. **Install [Visual Studio Code](https://code.visualstudio.com/)** (free, cross-platform).
2. **Clone this repository** to your local machine.
3. **Open any `.md` file** and start editing.

### Previewing Your Changes

VS Code has built-in Markdown preview support — no extensions required:

- **Side-by-side preview:** Open the Command Palette (`Ctrl + Shift + P`), then select `Markdown: Open Preview to the Side`.
- **Full-tab preview:** Press `Ctrl + Shift + V` to open a preview in a new tab.

### Generating Slides (Optional)

1. Install the **[Marp for VS Code](https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode)** extension.
2. Open your Markdown file.
3. Open the Command Palette (`Ctrl + Shift + P`) and select `Marp: Export Slide Deck...`.
4. Choose your desired format (PPTX, PDF, or HTML).

### Contributing Changes

We follow a standard **pull request** workflow:

1. **Fork** this repository (or create a branch if you have write access).
2. Make your changes in a descriptive branch (e.g. `update/module-3-french-translation`).
3. **Commit** with a clear message explaining what you changed and why.
4. Open a **pull request**. A reviewer will check your changes before they are merged.

This ensures quality control, traceability, and a clear audit trail for every change.

---

## 🌐 Multi-Language Strategy

Training content for Africa must support a wide range of languages. Our approach:

```
/content
  /en          ← English (source language)
  /fr          ← French
  /pt          ← Portuguese
  /sw          ← Swahili
  /ar          ← Arabic
  ...
```

- **English serves as the source language.** All modules are first authored in English.
- **Translations are maintained in parallel folders**, mirroring the source structure.
- **GitHub's diff view** makes it easy to see when the English source has changed, so translators know exactly which sections need updating.
- **Each language is translated once.** Whether the content is consumed as a web page, a slide deck, or a SCORM package, it is generated from the same translated Markdown file — eliminating redundant translation effort.

---

## 🤖 Future: AI Readiness

Because Markdown is plain, structured text, it is inherently well-suited for AI-assisted workflows:

- **Automated translation drafts** — LLMs can generate initial translations that human reviewers refine, dramatically accelerating the localisation process.
- **Content summarisation** — AI can produce concise summaries or glossaries from existing modules.
- **Intelligent search & retrieval** — Markdown content can be easily ingested into RAG (Retrieval-Augmented Generation) pipelines, enabling learners to ask questions and receive answers grounded in the training material.
- **Quality checks** — Automated tools can flag outdated references, inconsistent terminology, or incomplete translations.

---

## 🚀 Getting Involved

We welcome contributions from anyone — whether you are a GS1 standards expert, a trainer, a translator, or simply someone who wants to help improve capacity building in Africa.

- 📖 Read the [Contribution Guidelines](CONTRIBUTING.md) *(coming soon)*
- 🐛 [Open an issue](../../issues) if you spot an error or have a suggestion
- 🔀 Submit a pull request with your improvements

---

## 📄 Licence

All training content in this repository is released under an open-source licence. Details are specified in the [LICENSE](LICENSE) file. TBD

---

*This repository is maintained as part of the [STREAMING](https://www.2023streaming.eu/) project.*
