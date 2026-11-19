# 🪐 UJJWAL 3D

> **Interactive Tokenizer, 3D Semantic Vector Space & Word Similarity Studio**  
> Built as a self-contained web application in a single file (`index.html`) styled in a **Slideshow presentation deck** with **Raleway** typography and the **60-30-10 Pastel & Pale** design system.
> llmpipline.vercel.app


---

## 📖 Overview

**UJJWAL 3D** is an educational and exploratory Natural Language Processing (NLP) studio. It provides an intuitive, slide-by-slide presentation workflow to understand how text tokenization, word co-occurrence matrices, dimensional projection, and vector similarity metrics function together in semantic space.

Everything runs entirely on the client side in the browser using modern HTML5, CSS3, and [Three.js](https://threejs.org/) via CDN, with zero dependencies or server setups.

---

## 🎞️ Slideshow Deck Architecture

The application interface is structured as an interactive **4-Slide Presentation Deck** paired with a live 3D Semantic Space:

* **Slide 1 — Train & Build Vocabulary**:
  * Input corpus text or pick presets (*AI & Tech*, *Astronomy*, *Nature*).
  * Text normalization toggles (lowercase & punctuation).
  * **"Build Vocabulary"** button with live metrics (Unique Tokens, Total Corpus Tokens, and 3D Embeddings plotted).
* **Slide 2 — Encode Sentence**:
  * Query sentence encoder translating words into token pills and Token IDs.
  * `[OOV]` (out-of-vocabulary) detection badge.
  * Output array vector sequence (e.g. `[1, 14, 5, 2]`).
* **Slide 3 — Add Word with Same Similarity**:
  * Form to insert any new unseen word into 3D space.
  * Anchor word selector and live target similarity slider ($0.10$ to $0.99$) with gradient preview.
  * Mathematical angular positioning: $\mathbf{v}_{\text{new}} = \cos(\theta)\mathbf{u}_{\text{anchor}} + \sin(\theta)\mathbf{u}_{\perp}$.
* **Slide 4 — Vocabulary Inspector**:
  * Quick search filter and detailed view of all active tokens.
  * Bottom drawer table view with one-click **"Focus 3D"** camera navigation.

### 🕹️ Slideshow Controls
* **Header Step Pills**: Jump directly to any slide (`1. Train & Vocab`, `2. Encode`, `3. Add Word`, `4. Table`).
* **Navigation Arrows**: `◀ Prev` and `Next ▶` buttons.
* **Keyboard Navigation**: Use **Left Arrow (`←`)** and **Right Arrow (`→`)** to switch slides anytime.
* **Footer Indicator Dots**: Real-time visual progress tracker.

---

## 🎨 60-30-10 Pastel & Pale Design System

Styled with the **Raleway** font family from Google Fonts and adhering to the 60-30-10 color balance rule:

| Role | Coverage | Palette & Purpose |
| :--- | :--- | :--- |
| **Dominant** | **60%** | Soft pale porcelain and cloud canvas (`#f6f8fb`, `#eef2f7`). Open, airy workspace that reduces visual fatigue. |
| **Secondary** | **30%** | Pure white cards (`#ffffff`), subtle slate borders (`#e2e8f0`), frosted glass HUDs, and dark slate typography (`#0f172a`, `#334155`). |
| **Accent** | **10%** | Strategic pastel accents: <br>• **Periwinkle** (`#6366f1` / `#818cf8`): Primary actions, corpus nodes, active toggles.<br>• **Lilac** (`#a855f7` / `#c084fc`): Feature 3 card, similarity slider thumb.<br>• **Rose** (`#f472b6` / `#ec4899`): Custom-added words and badges.<br>• **Amber** (`#f59e0b`): Selected active nodes & highlighted links.<br>• **Mint** (`#10b981`): Live status indicator dot & high-similarity scores. |

---

## 📐 High-Visibility 3D Semantic Space

* **Small-Size Word Nodes & Compact Badges**:
  * Word spheres have a compact radius ($0.45$) to keep the 3D space clean and uncluttered.
  * High-contrast white pill badges with Raleway bold typography.
* **Multi-Level 3D Coordinate Grid**:
  * High-contrast ground grid ($y = -22$) in dark slate (`#64748b`) and rich indigo (`#4338ca`) at $0.85$ opacity.
  * Equatorial reference grid at the origin ($y = 0$).
  * Color-coded $X$ (Red), $Y$ (Green), and $Z$ (Blue) axes with 3D dimension badges (`X (Dim 1)`, `Y (Dim 2)`, `Z (Dim 3)`).
  * Volumetric boundary wireframe box ($52 \times 44 \times 52$).
* **Interactive Tooling**:
  * 3D Grid toggle, Auto-Rotate toggle, Labels toggle, Similarity Links toggle, Center View button.
  * Dynamic similarity chord filter slider ($\ge 0.50$).
  * Click-to-inspect card with closest semantic neighbors and cosine similarity percentages.

---

## 🚀 Getting Started

No build tools, Node.js packages, or local web servers are required.

1. Double-click **[`index.html`](file:///Users/ujjwal/Desktop/untitled%20folder%202/untitled%20folder/index.html)** to open it directly in any modern browser (Chrome, Safari, Edge, Firefox).
2. The default AI corpus will automatically build and visualize on initial load.
3. Use the slideshow controls or `←` / `→` arrow keys to tour through all features!

---

## 📁 Repository Structure

```text
.
├── index.html   # Complete, self-contained web app (HTML + CSS + Three.js logic)
└── README.md    # Documentation and usage guide
```

---

## 📄 License
MIT License. Free for educational and personal use.
