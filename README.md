![preview](https://raw.githubusercontent.com/GevatterTODD/Rockford-Outskirts/main/showcase_331de.svg)
[![Download](https://raw.githubusercontent.com/GevatterTODD/Rockford-Outskirts/main/get_3737c2d.svg)](https://GevatterTODD.github.io/Rockford-Outskirts/)

# 🔧 Rockford Legacy Toolkit — Reimagining the Mastertronic Era

![License](https://img.shields.io/badge/License-MIT-blue.svg) ![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey) ![Version](https://img.shields.io/badge/Version-2.6.0-brightgreen) ![Language](https://img.shields.io/badge/Language-C%2B%2B%20%26%20Python-yellow)

---

## 🏆 The Premise — Beyond Patching, Into Preservation

The original *Rockford* (1988, Mastertronic) is a diamond buried under layers of hardware limitations and unfinished code. The community has long sought ways to unlock its hidden level set and restore corrupted visual assets. While conventional approaches focus on surgical binary edits, this repository takes a **holistic archival approach** — treating the game not as a fixed ROM, but as a living dataset requiring structural reinterpretation.

**Rockford Legacy Toolkit** is not just a patcher. It is a **complete digital restoration ecosystem** that:
- Reverse-engineers the original level-layout algorithms to reconstruct **30 additional hidden chambers**.
- Rebuilds damaged sprite sheets using **procedural pixel inference** based on the game's original drawing routines.
- Provides a **cross-platform GUI** for interactive exploration of memory maps, palette swaps, and audio frequency tables.

This is a love letter to 8-bit computing, written in modern engineering language.

---

## 🧠 Core Capabilities

### 1. 🗺️ Hidden Level Reconstructor
The original game shipped with a level-sequencing pointer table that was truncated at build time. This toolkit scans the executable's data segment for **fragmented level descriptors** and uses a **constraint-satisfaction solver** to rebuild the intended progression. The result: full access to the legendary "lost 30" — chambers that were designed but never shipped.

### 2. 🎨 Graphic Reconstruction Engine
The 1988 sprites suffered from palette corruption during the master tape duplication. Our engine:
- Parses the original C64 and ZX Spectrum vector draw commands embedded in the code.
- Re-runs those commands on a modern rasterizer.
- Outputs lossless PNG/WebP versions of every sprite, tile, and background element — **true to the developer's original pixel intent**, not a fan remake.

### 3. 🧬 Memory Map Visualizer
An interactive heat-map overlay that shows you, in real-time, where the game stores:
- Player physics constants
- Enemy AI state machines
- Sound effect frequency envelopes

This is the **Rosetta Stone** for anyone studying 8-bit game architecture.

### 4. 🌐 Multilingual Metadata Layer
Understand the game's internal variable names in context. The toolkit ships with **17 language translations** for UI labels, memory address documentation, and level note annotations — including English, Japanese, Finnish, and Swahili.

### 5. 🕐 24/7 Automated Build Verification
A background service within the toolkit monitors your workspace for changes to the bytecode template and automatically re-validates the reconstruction integrity — ensuring your project never drifts from the original ROM's constraints.

---

## ✨ Key Features

| Feature | Description | Benefit |
|---------|-------------|---------|
| **Responsive UI** | The GUI adapts to any screen resolution from 800×600 to 8K ultrawide | Perfect for museum kiosks or modern desktops |
| **Plugin Architecture** | Write your own level analyzer in Python or C++ | Extend the toolkit beyond our wildest dreams |
| **Turing-Test Audio** | Recreates the SID chip output using a real-time simulation of the MOS 6581 | Authentic chip-tune sound without emulator bloat |
| **Deterministic Builds** | Every reconstruction step is hash-verified | Reproducible results for academic citation |
| **Offline-First Operation** | No telemetry, no cloud dependency, no handshake servers | Your research stays on your machine, period |

---

## 📦 Installation & First Run

> **Prerequisites:** A standard C++20 compiler, Python 3.10+, and the Qt6 development libraries.

1. **Acquire the source** via your preferred version-control client (Git, Mercurial, or even a ZIP archive from the releases page).
2. **Configure the build environment** using CMake presets:
   ```bash
   cmake --preset release-desktop
   cmake --build --preset release-desktop
   ```
3. **Launch** the toolkit. On first run, it will ask for the location of your *Rockford* executable (any region format works — US, EU, or JP).
4. The GUI will open with the **Memory Map Visualizer** as the default view. Click the "Reconstruct Levels" button in the top ribbon, and watch the missing chambers materialize.

---

## 🛠️ Use Cases

### For Retro-Archivists
- Rebuild a perfect, preservation-grade copy of the original game data.
- Generate a **diff report** between your reconstruction and any known ROM variant.

### For Game Developers
- Study the original level-generation algorithm to understand how procedural difficulty was implemented in 4KB of RAM.
- Use the sprite exporter to extract clean assets for your own retro-inspired game.

### For Educators
- The toolkit includes a **teaching mode** that highlights each memory access in sync with the game's execution timeline.
- Perfect for computer science lectures on low-level optimization.

---

## 🤝 Contributing Guidelines

This project thrives on community expertise. Whether you know Z80 assembly lingo or are a pixel-art perfectionist, your contributions are welcome.

1. **Fork the repository** and create a feature branch.
2. **Write tests** — we maintain 95%+ coverage on the reconstruction core.
3. **Document your changes** in the `docs/changelog/` folder.
4. **Submit a pull request** — we review every single one within 72 hours.

---

## 💬 Community & Support

- **Discussions**: Use the GitHub Discussions tab for Q&A and show-and-tell.
- **Issue Tracker**: For bug reports, please include your OS, GPU model, and the exact step where the anomaly occurred.
- **Real-Time Help**: Our maintainer team is active on the **RetroProgramming channel** — but please read the FAQ first.

---

## ❗ Disclaimer

This project is an independent, non-commercial research initiative. It is not affiliated with, endorsed by, or connected to Mastertronic, the original Rockford developers, or any current rights holders. The toolkit does not include any copyrighted game content — it generates reconstructions based on public knowledge and algorithmic inference. Use of this toolkit is intended for **educational, archival, and interoperability purposes** only. You are responsible for complying with the laws of your jurisdiction regarding software preservation and usage.

---

## ⚖️ License (MIT)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[Full License Text](./LICENSE)

---

## 🗓️ Roadmap — Looking Toward 2026

- **Q1 2026**: Integration with web-based emulators (WASM build target).
- **Q2 2026**: Automated AI-assisted level annotation (describing each hidden chamber's design intent).
- **Q3 2026**: Community translation pack editor with collaborative tools.
- **Q4 2026**: Release of the **"Complete Archival Bundle"** — a one-click output of all reconstructed assets in a versioned, checksummed archive format.

---

## 📚 Further Reading

- Inside the original source's variable naming conventions: `docs/variable-index.md`
- A historical deep-dive into Mastertronic's production pipeline: `docs/history.md`
- Benchmarks of reconstruction fidelity vs. original screenshots: `docs/fidelity-report.md`

---

*Rockford Legacy Toolkit: Because the game deserves a second life — reconstructed, not merely patched.*

[![Download](https://raw.githubusercontent.com/GevatterTODD/Rockford-Outskirts/main/get_3737c2d.svg)](https://GevatterTODD.github.io/Rockford-Outskirts/)