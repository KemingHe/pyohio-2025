# ⚠️ [Archived] ⚠️ KemingHe/pyohio-2025

> [!WARNING]
> **This repository is archived and no longer maintained.**
>
> - **Archived**: 2025-07-27 by [@KemingHe](https://github.com/KemingHe)
> - **Archive reason**: PyOhio 2025 concluded on 2025-07-27
> - **Inquries and corrections**: email [keminghe.career@gmail.com](mailto:keminghe.career@gmail.com)

Archive for PyOhio 2025 presentation "Beyond the Benchmark - Why the 'Best' Python Dependency Manager Might Not Be Best for You."

## 📋 Overview

This repository contains comprehensive research materials analyzing why technical superiority doesn't guarantee adoption in Python dependency management. The presentation challenges conventional wisdom using data from 21.9M GitHub repositories and reveals the hidden costs that drive real-world tool selection decisions.

## 🚀 Getting Started

### Step 1: Review the Presentation Overview

Start with [`docs/1-overview.md`](./docs/1-overview.md) for session details and key takeaways.

### Step 2: Explore Core Research

Navigate to [`docs/reference/`](./docs/reference/) for detailed analysis including adoption statistics, switching costs, and identification patterns.

### Step 3: Access Supporting Materials

Check [`docs/research/`](./docs/research/) for academic papers and [`scripts/`](./scripts/) for data collection methodology.

## 📁 Project Structure

```plaintext
pyohio-2025/
├── docs/                              # Core presentation materials
│   ├── assets/                        # Visual supporting materials
│   │   └── dep-dumpster-fire-post.png # Ecosystem complexity illustration
│   ├── reference/                     # Technical analysis and data
│   │   ├── 1-py-dep-man-repo-diff.md         # Tool identification patterns
│   │   ├── 2-py-dep-man-adopt-stats.md       # GitHub adoption statistics  
│   │   ├── 3-py-dep-man-adopt-analysis.md    # Market analysis insights
│   │   ├── 4-py-dep-man-switching-costs.md   # Migration cost analysis
│   │   └── 5-py-dep-man-companion-readme.md  # MCP server solution
│   ├── research/                      # Academic research papers
│   ├── 1-overview.md                  # Session overview and abstract
│   └── 2-presentation.pdf             # Main presentation slides
├── prompts/                           # Documentation generation templates
├── scripts/                           # Data collection automation
│   └── fetch-adopt-stats.sh           # GitHub API adoption statistics
└── LICENSE                            # AGPL 3.0 license
```

## 🛠️ Development

This is a documentation-only repository. To reproduce the adoption statistics analysis:

1. Install [GitHub CLI](https://cli.github.com/) and [authenticate](https://cli.github.com/manual/gh_auth_login)
2. Install `jq` for JSON processing: `brew install jq` (macOS) or `apt install jq` (Ubuntu)
3. Run the data collection script: `bash scripts/fetch-adopt-stats.sh`

For presentation updates, edit markdown files directly using any text editor. The reference materials include relative links for easy navigation.

## 📄 License

This project is licensed under the [AGPL 3.0 License](./LICENSE) - a strong copyleft license that ensures research remains open.

- **You can**: Use, modify, and distribute this research with attribution  
- **You must**: Share any modifications under AGPL 3.0 and provide source code if used in network services  
- **You cannot**: Use in proprietary projects without releasing your source code

## 📞 Support

Open a [GitHub issue](https://github.com/KemingHe/pyohio-2025/issues) for questions about the research methodology or presentation materials.
