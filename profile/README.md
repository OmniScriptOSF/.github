<div align="center">

<img src="https://img.shields.io/badge/OmniScript-v1.0.0-blue?style=for-the-badge" alt="OmniScript v1.0.0" />

### 🌟 The Universal Document DSL

**One format to generate documents, slides, sheets, charts, diagrams, and code**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm: parser](https://img.shields.io/npm/v/omniscript-parser.svg?label=parser)](https://www.npmjs.com/package/omniscript-parser)
[![npm: converters](https://img.shields.io/npm/v/omniscript-converters.svg?label=converters)](https://www.npmjs.com/package/omniscript-converters)
[![npm: cli](https://img.shields.io/npm/v/omniscript-cli.svg?label=cli)](https://www.npmjs.com/package/omniscript-cli)
[![Production Ready](https://img.shields.io/badge/status-production%20ready-success.svg)](https://github.com/OmniScriptOSF/omniscript-core/releases/tag/v1.0.0)

[🚀 Quick Start](#-quick-start) • [📦 Packages](#-packages) • [🎯 Features](#-features) • [🔗 Links](#-links)

</div>

---

## 🎉 v1.0.0 Released — Production Ready!

OmniScript Format v1.0 is **complete, tested, and production-ready**:

<table>
<tr>
<td width="50%">

✅ **152/152 tests passing** (100% success rate)  
✅ **3 npm packages published** and live  
✅ **v1.0 specification finalized**

</td>
<td width="50%">

✅ **All formats supported** (PDF, DOCX, PPTX, XLSX)  
✅ **Interactive playground** with live preview  
✅ **Zero critical security issues**

</td>
</tr>
</table>

**→ [📖 View Release Notes](https://github.com/OmniScriptOSF/omniscript-core/releases/tag/v1.0.0)**

---

## 💡 What is OmniScript?

OmniScript Format (OSF) is a **universal document description language** designed for:

<table>
<tr>
<td width="50%">

🤖 **LLM-native workflows**  
AI agents can generate structured documents

📄 **Multi-format output**  
Write once, export to PDF, DOCX, PPTX, XLSX

🔄 **Git-friendly**  
Plain text format, perfect for version control

</td>
<td width="50%">

🚀 **Developer-first**  
TypeScript API, CLI tools, VSCode extension

📊 **Data visualization**  
Built-in charts, diagrams, and code blocks

📝 **Simple syntax**  
Human-readable, easy to learn

</td>
</tr>
</table>

### Example OSF Document

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

**1. Install CLI**

```bash
npm install -g omniscript-cli
```

**2. Create a Document**

```bash
echo '@meta { title: "Hello World"; }
@doc { content: "# My First Document"; }' > hello.osf
```

**3. Export to Any Format**

```bash
osf export hello.osf --output hello.pdf
```

**4. Try the Playground**

Visit our **[Interactive Playground →](https://omniscriptosf.github.io/playground)** to try OSF in your browser with live preview!

---

## 📦 Packages

All packages are published on npm and available for installation:

<table>
<thead>
<tr>
<th width="25%">Package</th>
<th width="15%">Version</th>
<th width="40%">Description</th>
<th width="20%">Links</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>omniscript-parser</strong></td>
<td><code>v1.0.0</code></td>
<td>Zero-dependency parser for OSF → AST</td>
<td><a href="https://www.npmjs.com/package/omniscript-parser">npm</a> • <a href="https://github.com/OmniScriptOSF/omniscript-core/tree/main/parser">GitHub</a></td>
</tr>
<tr>
<td><strong>omniscript-converters</strong></td>
<td><code>v1.0.0</code></td>
<td>AST → PDF/DOCX/PPTX/XLSX converters</td>
<td><a href="https://www.npmjs.com/package/omniscript-converters">npm</a> • <a href="https://github.com/OmniScriptOSF/omniscript-converters">GitHub</a></td>
</tr>
<tr>
<td><strong>omniscript-cli</strong></td>
<td><code>v1.0.0</code></td>
<td>Command-line tools (parse, lint, export)</td>
<td><a href="https://www.npmjs.com/package/omniscript-cli">npm</a> • <a href="https://github.com/OmniScriptOSF/omniscript-core/tree/main/cli">GitHub</a></td>
</tr>
</tbody>
</table>

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

<table>
<thead>
<tr>
<th width="20%">Block</th>
<th width="30%">Purpose</th>
<th width="50%">Example Use Cases</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>@meta</code></td>
<td>Document metadata</td>
<td>Title, author, version, tags</td>
</tr>
<tr>
<td><code>@doc</code></td>
<td>Markdown content</td>
<td>Articles, reports, documentation</td>
</tr>
<tr>
<td><code>@slide</code></td>
<td>Presentation slides</td>
<td>Pitch decks, training materials</td>
</tr>
<tr>
<td><code>@sheet</code></td>
<td>Spreadsheet data</td>
<td>Tables, budgets, data exports</td>
</tr>
<tr>
<td><code>@chart</code> ⭐</td>
<td>Data visualization</td>
<td>Bar, line, pie, scatter, area charts</td>
</tr>
<tr>
<td><code>@diagram</code> ⭐</td>
<td>Visual diagrams</td>
<td>Flowcharts, sequence, Gantt, mindmaps</td>
</tr>
<tr>
<td><code>@code</code> ⭐</td>
<td>Syntax-highlighted code</td>
<td>Code examples, tutorials, documentation</td>
</tr>
</tbody>
</table>

<sub>⭐ = New in v1.0</sub>

### Output Formats

<table>
<thead>
<tr>
<th width="20%">Format</th>
<th width="20%">Extension</th>
<th width="60%">Rendering Engine</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>PDF</strong></td>
<td><code>.pdf</code></td>
<td>Puppeteer + Chart.js + Mermaid + Prism.js</td>
</tr>
<tr>
<td><strong>DOCX</strong></td>
<td><code>.docx</code></td>
<td>Microsoft Word (via <code>docx</code> library)</td>
</tr>
<tr>
<td><strong>PPTX</strong></td>
<td><code>.pptx</code></td>
<td>PowerPoint (native charts via PptxGenJS)</td>
</tr>
<tr>
<td><strong>XLSX</strong></td>
<td><code>.xlsx</code></td>
<td>Excel (via ExcelJS)</td>
</tr>
</tbody>
</table>

### Advanced Capabilities

<table>
<tr>
<td width="50%">

✅ Multi-series charts with customizable colors  
✅ Mermaid diagrams (flowchart, sequence, gantt)  
✅ Syntax highlighting for 50+ languages

</td>
<td width="50%">

✅ Line numbers and selective highlighting  
✅ TypeScript-first with full type safety  
✅ Zero-configuration — works out of the box

</td>
</tr>
</table>

---

## 🏗️ Repositories

<table>
<thead>
<tr>
<th width="35%">Repository</th>
<th width="45%">Purpose</th>
<th width="20%">Status</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/OmniScriptOSF/omniscript-core">omniscript-core</a></td>
<td>Parser, CLI, v1.0 spec</td>
<td>✅ v1.0.0</td>
</tr>
<tr>
<td><a href="https://github.com/OmniScriptOSF/omniscript-converters">omniscript-converters</a></td>
<td>Format converters</td>
<td>✅ v1.0.0</td>
</tr>
<tr>
<td><a href="https://github.com/OmniScriptOSF/omniscript-examples">omniscript-examples</a></td>
<td>25+ example documents</td>
<td>✅ Active</td>
</tr>
<tr>
<td><a href="https://github.com/OmniScriptOSF/omniscriptosf.github.io">omniscriptosf.github.io</a></td>
<td>Documentation site</td>
<td>✅ Live</td>
</tr>
<tr>
<td><a href="https://github.com/OmniScriptOSF/.github">.github</a></td>
<td>Organization profile</td>
<td>✅ This repo</td>
</tr>
</tbody>
</table>

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

<table>
<tr>
<td width="50%">

**Total Tests:** 152/152 passing (100%)  
**Code Coverage:** Branch coverage >90%  
**TypeScript:** Strict mode enabled

</td>
<td width="50%">

**Security:** Zero critical issues  
**Package Size:** 74 kB total (all 3 packages)  
**Dependencies:** Minimal (parser has zero deps)

</td>
</tr>
</table>

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
