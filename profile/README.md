# OmniScript Format (OSF)

<div align="center">

<img src="https://raw.githubusercontent.com/OmniScriptOSF/omniscript-core/main/assets/osf-icon-512px.png" alt="OmniScript Logo" width="200" height="200" />

# 🌟 The Universal Document DSL

**Write once, export everywhere - Documents, Slides, Sheets, Charts, Tables & More**

[![v1.2.0](https://img.shields.io/badge/version-1.2.0-blue.svg)](https://github.com/OmniScriptOSF/omniscript-core/blob/main/RELEASE_NOTES_v1.2.0.md)
[![Tests](https://img.shields.io/badge/tests-203%2F203%20passing-brightgreen.svg)](https://github.com/OmniScriptOSF/omniscript-core)
[![Security](https://img.shields.io/badge/security-A+-brightgreen.svg)](https://github.com/OmniScriptOSF/omniscript-core/blob/main/P%23_REVIEW_V1.2.0_FINAL_CLEAN.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[🚀 Get Started](https://github.com/OmniScriptOSF/omniscript-core) • [📖 Documentation](https://omniscript.dev/docs) • [🧪 Playground](https://omniscript.dev/playground) • [💬 Discussions](https://github.com/OmniScriptOSF/omniscript-core/discussions)

</div>

---

## 🎉 v1.2.0 - Tables, Includes & Enterprise Security!

**NEW in v1.2.0**:
- ✨ **@table blocks** - Markdown-style tables with captions, alignment, and styling
- ✨ **@include directive** - Modular documents with file composition and security
- 🔒 **Security Grade A+** - Path traversal protection, ReDoS prevention, strict validation
- 📊 **203 tests** - 130 core + 73 converters, 100% passing with 19 security tests
- 🏗️ **Refactored** - 85-91% code reduction, highly modular architecture (46 focused files)
- ✅ **Zero breaking changes** - Fully backward compatible with v1.1

---

## 💡 What is OmniScript?

OmniScript Format (OSF) is a **universal document DSL** that lets you write structured content once and export to multiple formats:

```osf
@meta { title: "Sales Report"; date: "2025-10-16"; }

@doc {
  # Q4 Sales Report
  **Outstanding performance** across all regions!
}

@table {
  caption: "Regional Performance";
  style: "bordered";
  alignment: ["left", "right", "center"];
  
  | Region | Revenue | Status |
  | --- | --- | --- |
  | North | $120K | ✓ Growth |
  | South | $95K | → Stable |
  | East | $145K | ✓ Growth |
}

@chart {
  type: "bar";
  title: "Revenue by Region";
  data: [
    { label: "North"; values: [120]; },
    { label: "South"; values: [95]; },
    { label: "East"; values: [145]; }
  ];
}

@include { path: "./sections/recommendations.osf"; }
```

**Export to**: PDF 📄 • DOCX 📝 • PPTX 🎞️ • XLSX 📊 • HTML 🌐 • Markdown 📃

---

## 🚀 Quick Start

### Install

```bash
# CLI tools (v1.2.1)
npm install -g omniscript-cli@1.2.1

# Libraries (v1.2.0)
npm install omniscript-parser@1.2.0
npm install omniscript-converters@1.2.0
```

### Use

```bash
# Create document
echo '@doc { # Hello World }' > hello.osf

# Export to PDF
osf render hello.osf --format pdf --output hello.pdf

# Parse and validate
osf parse hello.osf

# Format code
osf format hello.osf
```

---

## 📦 Official Packages

| Package | Version | Description | Tests | Status |
|---------|---------|-------------|-------|--------|
| [**omniscript-parser**](https://www.npmjs.com/package/omniscript-parser) | 1.2.0 | Zero-dependency TypeScript parser | 83/83 | ✅ [NPM](https://www.npmjs.com/package/omniscript-parser) |
| [**omniscript-cli**](https://www.npmjs.com/package/omniscript-cli) | 1.2.1 | Command-line tools | 47/47 | ✅ [NPM](https://www.npmjs.com/package/omniscript-cli) |
| [**omniscript-converters**](https://www.npmjs.com/package/omniscript-converters) | 1.2.0 | PDF, DOCX, PPTX, XLSX converters | 73/73 | ✅ [NPM](https://www.npmjs.com/package/omniscript-converters) |
| [**omniscript-vscode**](https://github.com/OmniScriptOSF/omniscript-vscode) | 0.1.0 | VSCode extension with IntelliSense | - | ✅ Stable |
| [**omniscript-examples**](https://github.com/OmniScriptOSF/omniscript-examples) | - | 25+ professional examples | All ✓ | ✅ Complete |

---

## ✨ Features

### Block Types

- **@meta** - Document metadata
- **@doc** - Markdown content with rich formatting
- **@slide** - Presentation slides
- **@sheet** - Spreadsheets with formulas
- **@table** - *NEW v1.2* Markdown-style tables
- **@chart** - Bar, line, pie charts
- **@diagram** - Flowcharts, sequences (Mermaid/Graphviz)
- **@code** - Syntax-highlighted code blocks

### Directives

- **@include** - *NEW v1.2* File composition and modular documents

### Export Formats

- PDF with charts and diagrams
- DOCX with tables and formatting
- PPTX with native charts
- XLSX with formulas
- HTML with live rendering
- Markdown with formatting

---

## 🏆 Why OmniScript?

✅ **Git-Friendly** - Plain text format perfect for version control  
✅ **AI-Friendly** - Easy for AI to generate and understand  
✅ **Developer-First** - Designed for technical writers and developers  
✅ **Type-Safe** - Full TypeScript support with 0 'any' types  
✅ **Secure** - Grade A+ security with comprehensive testing  
✅ **Fast** - Zero-dependency parser, blazing performance  
✅ **Modular** - Compose documents from reusable sections  
✅ **Extensible** - Easy to add custom blocks and renderers

---

## 🔒 Security

OmniScript v1.2.0 achieves **Security Grade A+**:

- ✅ Path traversal protection (prevents directory escape)
- ✅ ReDoS prevention (bounded regex quantifiers)
- ✅ XSS protection (multi-layer sanitization)
- ✅ Strict input validation (all inputs validated)
- ✅ Defense-in-depth architecture
- ✅ 19 comprehensive security tests

[View Security Review →](https://github.com/OmniScriptOSF/omniscript-core/blob/main/P%23_REVIEW_CLEAN_SUMMARY.md)

---

## 📊 Stats

| Metric | Value |
|--------|-------|
| **Tests** | 203/203 passing (100%) |
| **Core Tests** | 130 (parser + CLI) |
| **Converter Tests** | 73 (all formats) |
| **Security Tests** | 19 comprehensive |
| **Security Grade** | A+ |
| **Lines of Code** | 3,059 (highly modular) |
| **Dependencies** | 0 (parser) |
| **Block Types** | 8 |
| **Export Formats** | 6 |
| **Examples** | 25+ |

---

## 🎯 Use Cases

- 📚 **Technical Documentation** - Write once, export to multiple formats
- 🎓 **Education** - Create worksheets, slides, and exercises
- 💼 **Business Reports** - Generate reports with charts and tables
- 📊 **Data Visualization** - Build dashboards and analytics
- 🎨 **Presentations** - Professional slides with code and diagrams
- 📝 **API Documentation** - Version-controlled documentation
- 🔬 **Research Papers** - Academic papers with citations and tables

---

## 🌍 Community

- **GitHub**: [OmniScriptOSF](https://github.com/OmniScriptOSF)
- **Website**: [omniscript.dev](https://omniscript.dev)
- **Playground**: [omniscript.dev/playground](https://omniscript.dev/playground)
- **Discussions**: [GitHub Discussions](https://github.com/OmniScriptOSF/omniscript-core/discussions)
- **NPM**: [omniscript packages](https://www.npmjs.com/search?q=omniscript)

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](https://github.com/OmniScriptOSF/omniscript-core/blob/main/CONTRIBUTING.md) for guidelines.

Ways to contribute:
- 🐛 Report bugs
- 💡 Suggest features
- 📝 Improve docs
- 🔧 Submit PRs
- 🎨 Create themes
- 📚 Add examples

---

## 📄 License

MIT License - See [LICENSE](https://github.com/OmniScriptOSF/omniscript-core/blob/main/LICENSE)

---

<div align="center">

**Built with ❤️ by the OmniScript community**

[⭐ Star us on GitHub](https://github.com/OmniScriptOSF/omniscript-core) • [📖 Read the Docs](https://omniscript.dev/docs) • [🧪 Try the Playground](https://omniscript.dev/playground)

</div>
