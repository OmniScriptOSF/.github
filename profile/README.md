# OmniScript (.osf) Project

<div align="center">

<img src="https://raw.githubusercontent.com/OmniScriptOSF/omniscript-core/main/assets/osf-icon-512px.png" alt="OmniScript Logo" width="160" height="160" />

# 🚀 The Future of Document Processing

**OmniScript Format (OSF) - Universal Document DSL for LLMs, Agentic AI, and Git-Native Workflows**

[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Organization](https://img.shields.io/badge/GitHub-OmniScriptOSF-181717?logo=github)](https://github.com/OmniScriptOSF)
[![Discord](https://img.shields.io/badge/Discord-Join%20Us-7289DA?logo=discord)](https://discord.gg/omniscript)
[![Twitter](https://img.shields.io/badge/Twitter-@OmniScriptOSF-1DA1F2?logo=twitter)](https://twitter.com/OmniScriptOSF)

[🚀 Get Started](#-get-started) • [📦 Packages](#-our-ecosystem) • [💡 Examples](#-quick-examples) • [🤝 Contributing](#-contributing) • [🗺️ Roadmap](#-roadmap)

</div>

---

## ✨ What is OmniScript?

**OmniScript Format (OSF)** is revolutionizing how we create, manage, and process documents by unifying the best features of multiple formats into a single, AI-friendly syntax. Think of it as **Markdown meets LaTeX meets Excel meets PowerPoint** - all in one universal format.

<table>
<tr>
<td width="25%">

### 📝 **Rich Documents**
Like Markdown & LaTeX
- Expressive prose & math
- Structured content  
- Beautiful typography
- Git-friendly diffs

</td>
<td width="25%">

### 🎯 **Dynamic Presentations**
Like PowerPoint & Keynote
- Rich layouts & themes
- Smooth transitions
- Interactive elements
- Automatic slide generation

</td>
<td width="25%">

### 📊 **Live Spreadsheets**
Like Excel & Google Sheets
- Data tables & formulas
- Real-time calculations
- Dynamic charts
- Formula engine built-in

</td>
<td width="25%">

### 🤖 **AI-Native**
Built for the Future
- LLM-friendly syntax
- Semantic structure
- Version control ready
- Perfect for automation

</td>
</tr>
</table>

---

## 🌟 Why Choose OmniScript?

<div align="center">

| Challenge | Traditional Approach | OmniScript Solution |
|-----------|---------------------|-------------------|
| **🔄 Version Control** | Binary files, merge conflicts | ✅ **Git-native text format** with meaningful diffs |
| **🤖 AI Integration** | Complex parsing, format chaos | ✅ **LLM-optimized syntax** for seamless AI workflows |
| **📱 Multi-format Output** | One format = one tool | ✅ **Single source** → Export to DOCX, PPTX, XLSX, PDF, HTML |
| **🔗 Interoperability** | Format silos and vendor lock-in | ✅ **Universal format** that works everywhere |
| **⚡ Dynamic Content** | Static documents only | ✅ **Live formulas** and real-time calculations |
| **🎨 Consistent Styling** | Manual formatting headaches | ✅ **Theme system** with automatic styling |

</div>

---

## 📦 Our Ecosystem

<div align="center">

### 🎯 Core Packages

[![omniscript-parser](https://img.shields.io/npm/v/omniscript-parser?label=omniscript-parser&logo=npm&color=CB3837)](https://www.npmjs.com/package/omniscript-parser)
[![omniscript-cli](https://img.shields.io/npm/v/omniscript-cli?label=omniscript-cli&logo=npm&color=CB3837)](https://www.npmjs.com/package/omniscript-cli)
[![omniscript-converters](https://img.shields.io/npm/v/omniscript-converters?label=omniscript-converters&logo=npm&color=CB3837)](https://www.npmjs.com/package/omniscript-converters)

</div>

### 🏗️ Repository Structure

| Repository | Description | Status | Key Features |
|------------|-------------|--------|--------------|
| **[omniscript-core](https://github.com/OmniScriptOSF/omniscript-core)** | 🔥 Core engine with parser, CLI & specs | ![Build](https://img.shields.io/github/actions/workflow/status/OmniScriptOSF/omniscript-core/ci.yml) | Parser, CLI tools, specifications |
| **[omniscript-converters](https://github.com/OmniScriptOSF/omniscript-converters)** | 🔄 Professional format converters | ✅ **Published** | PDF, DOCX, PPTX, XLSX export |
| **[omniscript-examples](https://github.com/OmniScriptOSF/omniscript-examples)** | 💡 Real-world examples & templates | ![Examples](https://img.shields.io/badge/examples-50+-green) | Business docs, presentations, reports |
| **[omniscript-vscode](https://github.com/OmniScriptOSF/omniscript-vscode)** | 🎨 VS Code extension | ![Planned](https://img.shields.io/badge/status-planned-blue) | Syntax highlighting, IntelliSense |
| **[omniscript-site](https://github.com/OmniScriptOSF/omniscript-site)** | 🌐 Official website & documentation | ![Planned](https://img.shields.io/badge/status-planned-blue) | Interactive docs, playground |

### 📊 Package Details

| Package | Purpose | Version | Downloads | Dependencies |
|---------|---------|---------|-----------|--------------|
| **omniscript-parser** | TypeScript parsing engine | ![npm](https://img.shields.io/npm/v/omniscript-parser) | ![downloads](https://img.shields.io/npm/dm/omniscript-parser) | Zero deps |
| **omniscript-cli** | Command-line tools | ![npm](https://img.shields.io/npm/v/omniscript-cli) | ![downloads](https://img.shields.io/npm/dm/omniscript-cli) | Parser + converters |
| **omniscript-converters** | Professional converters | ![npm](https://img.shields.io/npm/v/omniscript-converters) | ![downloads](https://img.shields.io/npm/dm/omniscript-converters) | Parser + formats |

---

## 🚀 Get Started

### ⚡ Quick Installation

<table>
<tr>
<td width="50%">

**🔧 For Developers**
```bash
# Core parsing library
npm install omniscript-parser

# Professional format converters
npm install omniscript-converters

# Both together
npm install omniscript-parser omniscript-converters
```

</td>
<td width="50%">

**⚡ For Users**
```bash
# Global CLI tools
npm install -g omniscript-cli

# Quick start
osf --help
```

</td>
</tr>
</table>

### 🏃 30-Second Demo

```bash
# Create a sample document
echo '@meta { title: "Hello OSF"; }
@doc { # Welcome
This is **your first** OSF document! }' > hello.osf

# Parse and validate
osf parse hello.osf

# Render to HTML
osf render hello.osf --output hello.html

# Convert to multiple formats
osf render hello.osf --format docx --output hello.docx
osf render hello.osf --format pptx --output hello.pptx
osf render hello.osf --format xlsx --output hello.xlsx
osf render hello.osf --format pdf --output hello.pdf
```

---

## 💡 Quick Examples

<details>
<summary><b>📋 Business Report</b></summary>

```osf
@meta {
  title: "Q2 Business Review";
  author: "Jane Smith";
  date: "2025-06-28";
  theme: "CorporateBlue";
}

@doc {
  # Executive Summary
  
  Our Q2 performance exceeded expectations with **15% revenue growth** 
  and significant improvements in customer retention.
  
  ## Key Achievements
  - Revenue: $2.3M (+15%)
  - Customer Churn: 3% (-2%)
  - Team Growth: 45 employees (+8)
}

@sheet {
  name: "Regional Performance";
  cols: [Region, Q1_Revenue, Q2_Revenue, Growth_Percent];
  data {
    (2,1)="North America"; (2,2)=850000; (2,3)=975000;
    (3,1)="Europe"; (3,2)=650000; (3,3)=748000;
    (4,1)="Asia Pacific"; (4,2)=400000; (4,3)=477000;
  }
  formula (2,4): "=(C2-B2)/B2*100";
  formula (3,4): "=(C3-B3)/B3*100";
  formula (4,4): "=(C4-B4)/B4*100";
}
```

</details>

<details>
<summary><b>🎯 Product Presentation</b></summary>

```osf
@meta {
  title: "Product Launch 2025";
  author: "Product Team";
  theme: "ModernTech";
}

@slide {
  title: "Introducing OmniScript";
  layout: "TitleAndContent";
  content: "The future of document processing is here.";
}

@slide {
  title: "Key Features";
  layout: "TitleAndBullets";
  bullets {
    "🚀 Universal document format";
    "🤖 AI-native syntax design";
    "🔄 Git-friendly version control";
    "📊 Multi-format export capabilities";
  }
}
```

</details>

<details>
<summary><b>📊 Data Analysis</b></summary>

```osf
@meta {
  title: "Sales Analysis Dashboard";
  author: "Analytics Team";
  theme: "DataViz";
}

@sheet {
  name: "Monthly Sales";
  cols: [Month, Sales, Target, Performance];
  data {
    (1,1)="Jan"; (1,2)=85000; (1,3)=80000;
    (2,1)="Feb"; (2,2)=92000; (2,3)=85000;
    (3,1)="Mar"; (3,2)=78000; (3,3)=90000;
  }
  formula (1,4): "=B1/C1*100";
  formula (2,4): "=B2/C2*100";
  formula (3,4): "=B3/C3*100";
}
```

</details>

---

## 🗺️ Roadmap

<div align="center">

### 📅 Version Timeline

| Version | Status | Key Features | ETA |
|---------|--------|--------------|-----|
| **v0.5** | ✅ **Released** | Core parsing, CLI tools, basic rendering | **Current** |
| **v0.6** | 🚧 **In Progress** | Converter improvements, enhanced themes | **Q3 2025** |
| **v1.0** | 📋 **Planned** | Advanced exports, diagram support, VS Code extension | **Q4 2025** |
| **v1.1** | 💭 **Future** | Real-time collaboration, plugin system | **Q1 2026** |
| **v2.0** | 🌟 **Vision** | Visual editor, cloud integration, enterprise features | **2026** |

</div>

### 🔥 Coming Soon

- 🎨 **Visual Editor** - WYSIWYG editing experience with live preview
- 📊 **Advanced Charts** - Interactive data visualizations and dashboards  
- 🔗 **Real-time Collaboration** - Multi-user editing with conflict resolution
- 🧩 **Plugin System** - Extensible architecture for custom functionality
- ☁️ **Cloud Integration** - Seamless sync across devices and platforms

---

## 🤝 Contributing

<div align="center">

**We ❤️ contributions from developers, designers, writers, and users of all skill levels!**

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](http://makeapullrequest.com)
[![First Timers Only](https://img.shields.io/badge/first--timers--only-friendly-blue.svg?style=for-the-badge)](https://www.firsttimersonly.com/)
[![Good First Issues](https://img.shields.io/github/issues/OmniScriptOSF/omniscript-core/good%20first%20issue?style=for-the-badge)](https://github.com/OmniScriptOSF/omniscript-core/labels/good%20first%20issue)

</div>

### 🚀 Quick Start for Contributors

```bash
# 1. Fork and clone any repo
git clone https://github.com/YOUR_USERNAME/REPO_NAME.git

# 2. Install dependencies
pnpm install

# 3. Create a feature branch
git checkout -b feature/amazing-feature

# 4. Make your changes and test
pnpm run build && pnpm test

# 5. Submit a PR
git push origin feature/amazing-feature
```

### 📚 Resources & Support

- 📖 [Complete Documentation](https://github.com/OmniScriptOSF/omniscript-core/tree/main/docs)
- 💡 [Example Gallery](https://github.com/OmniScriptOSF/omniscript-examples)
- 🤝 [Contributing Guide](https://github.com/OmniScriptOSF/omniscript-core/blob/main/CONTRIBUTING.md)
- 🐛 [Bug Reports](https://github.com/OmniScriptOSF/omniscript-core/issues/new?template=bug_report.md)
- 💡 [Feature Requests](https://github.com/OmniScriptOSF/omniscript-core/issues/new?template=feature_request.md)

---

## 📄 License & Community

<div align="center">

**MIT License** © 2025 [OmniScript Organization](https://github.com/OmniScriptOSF)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

**🔗 Connect with us:**
[GitHub](https://github.com/OmniScriptOSF) • [Discord](https://discord.gg/omniscript) • [Twitter](https://twitter.com/OmniScriptOSF)

---

### 🌟 **"The future of documents is universal, AI-native, and Git-friendly."**

*Made with ❤️ by the global OmniScript community*

</div>