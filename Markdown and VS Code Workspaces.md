# **Markdown**


Markdown is a lightweight plain-text formatting language that lets you add formatting elements (headers, bold, lists, links, etc.) using simple punctuation characters, which then get converted into formatted HTML or other output.

### Brief History


2004 — Created by John Gruber (of Daring Fireball) in collaboration with Aaron Swartz. The goal was simple: let people write in easy-to-read, easy-to-write plain text that could be converted to valid HTML. The name was a play on “markup” — instead of marking up text with tags, you mark it down with minimal symbols.
2009–2012 — Fragmentation era. No formal specification existed, so different platforms implemented Markdown differently, causing inconsistencies across tools.
2014 — CommonMark was proposed by Jeff Atwood (co-founder of Stack Overflow) and others — a standardized, unambiguous spec for Markdown to resolve the fragmentation problem.
2016 — GitHub Flavored Markdown (GFM) became one of the most widely used variants, adding features like tables, task lists, and syntax-highlighted code blocks.

### **How It’s Used Today**


**Markdown is now ubiquitous across the web and software development:**
	∙	Documentation — README files on GitHub/GitLab are almost universally written in Markdown
	∙	Note-taking apps — Obsidian, Notion, Bear, and Typora all use it
	∙	Static site generators — Jekyll, Hugo, and Gatsby render Markdown into full websites
	∙	Communication tools — Slack, Discord, and Microsoft Teams support Markdown-like formatting
	∙	AI & chat interfaces — including this one; Claude and ChatGPT both render Markdown responses
	∙	Academic & technical writing — tools like Pandoc convert Markdown to PDF, Word, LaTeX, and more
	∙	Wikis & knowledge bases — Confluence, GitHub Wikis, and many CMS platforms support it


Its enduring appeal is that the source text is readable as-is, even without rendering — making it both human- and machine-friendly.

### Markdown in the Age of AI


**Markdown has become arguably more important with the rise of AI, not less. Here’s why:**

1. **It’s the Native Language of AI Communication**
   Large language models like Claude and GPT were trained on enormous amounts of Markdown-formatted text (GitHub, Stack Overflow, documentation sites, Reddit, etc.). As a result, AI models think and structure output naturally in Markdown — headers, bullets, code blocks, and emphasis come out cleanly because the model has seen billions of examples of it.
   When you read a well-structured AI response, Markdown is almost certainly what’s making it look that way under the hood.
2. **AI-Generated Code Lives in Markdown**
   When AI writes code, it wraps it in fenced code blocks (```). This isn’t cosmetic — it signals:
   ∙	What programming language is being used (for syntax highlighting)
   ∙	Where the code starts and ends (so it can be copy-pasted cleanly)
   ∙	Separation between explanation and executable content
   Without Markdown, AI-generated code would be indistinguishable walls of text.
3. **Prompts and Context Are Often Written in Markdown**
   Developers increasingly write system prompts, AI instructions, and context documents in Markdown because it gives the model clear structural signals — it knows a ## heading is a section boundary, a - is a list item, and a code block is something to reason about differently than prose.
   Structure in → structure out.
4. **Documentation Automation**
   AI tools like GitHub Copilot, Cursor, and Claude can now auto-generate entire README files, API docs, and wikis in Markdown. This means:
   ∙	Codebases stay documented with far less manual effort
   ∙	Docs live alongside code in version control
   ∙	Teams can prompt an AI to update or expand docs as code changes
5. **AI Tools Are Built Around It**
   Nearly every major AI-adjacent tool has Markdown at its core:
   ∙	Cursor / VS Code + AI extensions — inline docs and explanations render as Markdown
   ∙	Jupyter Notebooks — mix code and Markdown prose, increasingly AI-generated
   ∙	LLM APIs — responses are returned as Markdown strings for apps to render
   ∙	RAG pipelines — documents chunked and stored for AI retrieval are often Markdown files
   ∙	MCP servers and AI agents — tool outputs, memory, and reasoning traces are logged in Markdown
6. **Human-AI Collaboration Needs a Common Format**
   As humans and AI increasingly co-author code, documentation, and knowledge bases, both sides need a format they can read and write reliably. Markdown is:
   ∙	Simple enough for humans to write quickly
   ∙	Structured enough for AI to parse and generate consistently
   ∙	Renderable in virtually every modern tool
   It has quietly become the lingua franca of the human-AI interface — the shared medium through which ideas, instructions, and code flow back and forth.

In short, Markdown was already important before AI. The AI era has made it foundational.


### Markdown for IBM i / RPG Developers Using VS Code

Traditional RPG programmers are often coming from an environment (green screen, SEU, RDi) where documentation was an afterthought and formatting was essentially nonexistent. VS Code and the modern IBM i toolchain change that dramatically — and Markdown sits at the center of it.

1. **README Files for IBM i Projects**
   With tools like Source Orbit and bob (Better Object Builder), your IBM i projects are now version-controlled in Git repositories. Every serious Git repo has a README.md — and that file is:
   ∙	The first thing a teammate sees when they open the project
   ∙	Where you document what the project does, dependencies, and build instructions
   ∙	Rendered automatically and beautifully by GitHub, GitLab, or Azure DevOps
   RPG developers new to Git-based workflows need to understand Markdown just to write basic project documentation.
2. **The IBM i Extension Pack and VS Code Render Markdown Natively**
   VS Code has built-in Markdown preview — you can write a .md file and see it rendered side-by-side in real time. For IBM i developers this means:
   ∙	Documenting programs, service programs, and modules right alongside the source
   ∙	Writing deployment notes or runbooks that live in the same repo as the RPG source
   ∙	Creating onboarding guides for new team members familiar with the codebase
3. **Source Orbit and bob Use Markdown-Adjacent Formats**
   Source Orbit generates dependency graphs and build metadata. The output and documentation around those workflows — including Rules.mk explanations, impact analysis reports, and project notes — are increasingly written or rendered in Markdown. Understanding Markdown helps you:
   ∙	Document which modules depend on what
   ∙	Annotate impact analysis findings for your team
   ∙	Write change notes that travel with the source in version control
4. **AI Coding Assistants in VS Code Speak Markdown**
   If you’re using GitHub Copilot, Continue, or Claude inside VS Code to help write or explain RPG code, every response comes back formatted in Markdown. Understanding it means you can:
   ∙	Read AI-generated explanations of legacy RPG logic clearly
   ∙	Copy AI-suggested free-format RPG code cleanly from code blocks
   ∙	Write better prompts by structuring your questions with Markdown formatting
   This is especially valuable when modernizing fixed-format RPG to free-format ILE RPG — a task AI can help with heavily, and one where structured explanations really matter.
5. **Documenting RPG Programs Properly for the First Time**
   Many legacy RPG shops have zero documentation — logic lives only in the heads of senior developers or buried in cryptic comments. Markdown gives teams a lightweight way to finally document:
   ∙	What a program or service program does
   ∙	Input/export parameters for procedures
   ∙	Business rules embedded in legacy code
   ∙	Known issues and technical debt
   A simple CUSTINQ.md sitting next to CUSTINQ.rpgle in the repo is infinitely better than nothing — and Markdown makes writing it fast and painless.
6. **GitHub / Azure DevOps Wiki and Issue Tracking**
   IBM i shops adopting modern DevOps practices use GitHub or Azure DevOps for issue tracking and wikis. Both render Markdown everywhere — in issues, pull requests, wikis, and comments. RPG developers participating in code reviews or filing bugs need basic Markdown literacy to communicate effectively in those tools.

## The Bottom Line for RPG Developers


Traditional RPG programmers were experts in a world where the code was the documentation and everything lived on the iron. The modern IBM i stack — VS Code, ILEastic, NOXDB, Source Orbit, bob, Git — is a collaborative, open, documented world. Markdown is the low-friction glue that makes documentation actually happen in that world, and AI tools make writing it even easier. Learning Markdown is a small investment with an outsized return for any RPG developer modernizing their workflow.


---



## VS Code Workspaces

A **workspace** in VS Code is essentially a configured context for your work — it defines *which folders are open* and *how VS Code should behave* within that context.

### What Is a Workspace?

At its simplest, opening a single folder in VS Code creates an  **implicit single-folder workspace** . But you can also create a **named workspace** (saved as a `.code-workspace` file) that can contain multiple folders and explicit configuration. This file is just JSON and can be committed to source control.

### What a Workspace Controls

**Settings** — Workspaces have their own `settings.json` that overrides your user-level settings. The precedence chain is:

> Default → User settings → Workspace settings → Folder settings (in multi-root)

So you can, for example, enforce a specific formatter for one project without affecting others.

**Tasks & Launch Configs** — `tasks.json` and `launch.json` live inside `.vscode/` within the workspace, so your run/debug configs are project-specific.

**Recommended Extensions** — You can add an `extensions.json` file inside `.vscode/` to suggest (or even require) specific extensions for anyone who opens that workspace:

```json
{
  "recommendations": ["esbenp.prettier-vscode", "dbaeumer.vscode-eslint"]
}
```

VS Code will prompt collaborators to install them. This is **not** enforcement, just a recommendation.

---

### How Workspaces Relate to Profiles

**Profiles** are a separate, higher-level concept introduced more recently. A profile bundles together:

* Extensions
* Settings
* Keybindings
* Snippets
* UI state

The relationship is:

* A **profile** is like a persona (e.g., "Python Dev", "Frontend", "Writing")
* A **workspace** is a specific project or folder context

You can  **associate a profile with a workspace** , so that when you open that workspace, VS Code automatically switches to the right profile — giving you only the extensions and settings relevant to that work. You do this via  **File → Preferences → Profiles → Apply Profile to Workspace** .

---

### The Key Distinction

|                       | Workspace                                                     | Profile                                                  |
| --------------------- | ------------------------------------------------------------- | -------------------------------------------------------- |
| **Scope**       | A project/folder                                              | A full VS Code environment                               |
| **Controls**    | Settings, tasks, launch configs, extension*recommendations* | Extensions, settings, keybindings, snippets              |
| **Portability** | `.code-workspace`file or `.vscode/`folder                 | Synced via Settings Sync or exported                     |
| **Switching**   | Open a different folder                                       | Manually switch or auto-switch via workspace association |

---

### Practical Tips

* Use **workspace settings** for project-specific things like linting rules, tab size, or file associations.
* Use **profiles** to avoid having 50 extensions loaded at all times — a "Data Science" profile with Jupyter/Python tools and a "Web" profile with ESLint/Prettier keeps VS Code fast and focused.
* Commit your `.vscode/extensions.json` and `.vscode/settings.json` to git so teammates get a consistent environment automatically.
