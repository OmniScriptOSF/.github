# OmniScript Format (OSF)

<div align="center">

# 🌟 The Universal Document DSL

**One format to generate documents, slides, sheets, charts, diagrams, and code**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm: parser](https://img.shields.io/npm/v/omniscript-parser.svg?label=parser)](https://www.npmjs.com/package/omniscript-parser)
[![npm: converters](https://img.shields.io/npm/v/omniscript-converters.svg?label=converters)](https://www.npmjs.com/package/omniscript-converters)
[![npm: cli](https://img.shields.io/npm/v/omniscript-cli.svg?label=cli)](https://www.npmjs.com/package/omniscript-cli)
[![Production Ready](https://img.shields.io/badge/status-production%20ready-success.svg)](https://github.com/OmniScriptOSF/omniscript-core/releases/tag/v1.0.0)

[🚀 Quick Start](#-quick-start) • [📦 Packages](#-packages) • [🎯 Features](#-features) • [🔗 Links](#-links)

</div>

---

## 🎉 v1.0.0 Released - Production Ready!

OmniScript Format v1.0 is **complete, tested, and production-ready**:

- ✅ **152/152 tests passing** (100% success rate)
- ✅ **3 npm packages published** and live
- ✅ **v1.0 specification finalized** (charts, diagrams, code blocks)
- ✅ **All formats supported** (PDF, DOCX, PPTX, XLSX)
- ✅ **Interactive playground** with live preview
- ✅ **Zero critical security issues**

**[📖 View Release Notes →](https://github.com/OmniScriptOSF/omniscript-core/releases/tag/v1.0.0)**

---

## 💡 What is OmniScript?

OmniScript Format (OSF) is a **universal document description language** designed for:

- 🤖 **LLM-native workflows** - AI agents can generate structured documents
- 📄 **Multi-format output** - Write once, export to PDF, DOCX, PPTX, XLSX
- 🔄 **Git-friendly** - Plain text format, perfect for version control
- 🚀 **Developer-first** - TypeScript API, CLI tools, VSCode extension
- 📊 **Data visualization** - Built-in charts, diagrams, and code blocks

### Example

```osf
@meta {
  title: "Sales Report Q4 2025";
  author: "Finance Team";
}

@doc {
  content: "# Executive Summary
  
  Revenue increased **35%** this quarter.
  ";
}

@chart {
  type: "bar";
  title: "Quarterly Revenue";
  data: [
    { label: "Q1"; values: [100]; },
    { label: "Q2"; values: [120]; },
    { label: "Q3"; values: [150]; },
    { label: "Q4"; values: [180]; }
  ];
}
```

**Output:** PDF, DOCX, PPTX, or XLSX with charts rendered natively

---

## 🚀 Quick Start

### Install CLI

```bash
npm install -g omniscript-cli
```

### Create a Document

```bash
echo '@meta { title: "Hello World"; }
@doc { content: "# My First Document"; }' > hello.osf

osf export hello.osf --output hello.pdf
```

### Try the Playground

Visit our **[Interactive Playground](https://omniscriptosf.github.io/playground)** to try OSF in your browser with live preview!

---

## 📦 Packages

All packages are published on npm and available for installation:

### Core Packages

| Package | Version | Description | Links |
|---------|---------|-------------|-------|
| **omniscript-parser** | v1.0.0 | Zero-dependency parser for OSF → AST | [npm](https://www.npmjs.com/package/omniscript-parser) • [GitHub](https://github.com/OmniScriptOSF/omniscript-core/tree/main/parser) |
| **omniscript-converters** | v1.0.0 | AST → PDF/DOCX/PPTX/XLSX converters | [npm](https://www.npmjs.com/package/omniscript-converters) • [GitHub](https://github.com/OmniScriptOSF/omniscript-converters) |
| **omniscript-cli** | v1.0.0 | Command-line tools (parse, lint, export) | [npm](https://www.npmjs.com/package/omniscript-cli) • [GitHub](https://github.com/OmniScriptOSF/omniscript-core/tree/main/cli) |

### Installation

```bash
# CLI (includes parser and converters)
npm install -g omniscript-cli

# Libraries for programmatic use
npm install omniscript-parser omniscript-converters
```

---

## 🎯 Features

### v1.0 Block Types

| Block | Purpose | Example Use Cases |
|-------|---------|------------------|
| **@meta** | Document metadata | Title, author, version, tags |
| **@doc** | Markdown content | Articles, reports, documentation |
| **@slide** | Presentation slides | Pitch decks, training materials |
| **@sheet** | Spreadsheet data | Tables, budgets, data exports |
| **@chart** ⭐ | Data visualization | Bar, line, pie, scatter, area charts |
| **@diagram** ⭐ | Visual diagrams | Flowcharts, sequence, Gantt, mindmaps |
| **@code** ⭐ | Syntax-highlighted code | Code examples, tutorials, documentation |

⭐ = New in v1.0

### Output Formats

| Format | Extension | Rendering |
|--------|-----------|-----------|
| **PDF** | `.pdf` | Puppeteer + Chart.js + Mermaid + Prism.js |
| **DOCX** | `.docx` | Microsoft Word (via `docx` library) |
| **PPTX** | `.pptx` | PowerPoint (native charts via PptxGenJS) |
| **XLSX** | `.xlsx` | Excel (via ExcelJS) |

### Advanced Features

- ✅ **Multi-series charts** with customizable colors and legends
- ✅ **Mermaid diagrams** (flowchart, sequence, gantt, mindmap)
- ✅ **Syntax highlighting** for 50+ programming languages
- ✅ **Line numbers** and selective line highlighting in code blocks
- ✅ **TypeScript-first** with full type safety
- ✅ **Zero-configuration** - works out of the box

---

## 🏗️ Repositories

| Repository | Purpose | Status |
|------------|---------|--------|
| [omniscript-core](https://github.com/OmniScriptOSF/omniscript-core) | Parser, CLI, v1.0 spec | ✅ v1.0.0 |
| [omniscript-converters](https://github.com/OmniScriptOSF/omniscript-converters) | Format converters | ✅ v1.0.0 |
| [omniscript-examples](https://github.com/OmniScriptOSF/omniscript-examples) | 25+ example documents | ✅ Active |
| [omniscriptosf.github.io](https://github.com/OmniScriptOSF/omniscriptosf.github.io) | Documentation site | ✅ Live |
| [.github](https://github.com/OmniScriptOSF/.github) | Organization profile | ✅ This repo |

---

## 🔗 Links

### Documentation
- 📖 **[Full Documentation](https://omniscriptosf.github.io/docs)**
- 🎮 **[Interactive Playground](https://omniscriptosf.github.io/playground)**
- 📝 **[v1.0 Specification](https://github.com/OmniScriptOSF/omniscript-core/blob/main/spec/v1.0/osf-spec.md)**
- 🎓 **[Getting Started Guide](https://omniscriptosf.github.io/docs/getting-started/installation)**
- 💡 **[Example Library](https://github.com/OmniScriptOSF/omniscript-examples)**

### Community
- 🐛 **[Report Issues](https://github.com/OmniScriptOSF/omniscript-core/issues)**
- 💬 **[Discussions](https://github.com/OmniScriptOSF/omniscript-core/discussions)**
- 📢 **[Release Notes](https://github.com/OmniScriptOSF/omniscript-core/releases)**

### npm Packages
- 📦 **[omniscript-parser](https://www.npmjs.com/package/omniscript-parser)**
- 📦 **[omniscript-converters](https://www.npmjs.com/package/omniscript-converters)**
- 📦 **[omniscript-cli](https://www.npmjs.com/package/omniscript-cli)**

---

## 📊 Project Stats

- **Total Tests:** 152/152 passing (100%)
- **Code Coverage:** Branch coverage >90%
- **TypeScript:** Strict mode enabled
- **Security:** Zero critical issues
- **Package Size:** 74 kB total (all 3 packages)
- **Dependencies:** Minimal (parser has zero deps)

---

## 🤝 Contributing

We welcome contributions! Please see individual repository README files for contribution guidelines.

---

## 📄 License

All OmniScript OSF packages are released under the **MIT License**.

---

<div align="center">

**Made with ❤️ by the OmniScript OSF Team**

[Website](https://omniscriptosf.github.io) • [GitHub](https://github.com/OmniScriptOSF) • [npm](https://www.npmjs.com/search?q=omniscript)

</div>
