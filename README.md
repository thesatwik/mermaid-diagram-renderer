# Mermaid Diagram Renderer

**A free, browser-based tool to convert any [Mermaid](https://mermaid.js.org/) diagram into a downloadable PNG or SVG image. No install. No account. No server.**

🔗 **Live tool → [thesatwik.github.io/mermaid-diagram-renderer](https://thesatwik.github.io/mermaid-diagram-renderer/)**

---

## What it does

Paste your Mermaid diagram code into the editor, click **Render**, and download a crisp PNG or SVG — ready for docs, slides, or design files.

Everything runs in your browser. Your diagrams never leave your machine.

## Supported diagram types

| Type | Keyword |
|---|---|
| Flowchart | `flowchart` |
| Sequence diagram | `sequenceDiagram` |
| C4 Context | `C4Context` |
| ER diagram | `erDiagram` |
| Gantt chart | `gantt` |
| Class diagram | `classDiagram` |
| State diagram | `stateDiagram-v2` |
| Mind map | `mindmap` |
| …and all other Mermaid types | — |

## Quick example

```
flowchart TD
    A[Start] --> B{OK?}
    B -- Yes --> C[Done]
    B -- No  --> D[Retry]
    D --> B
```

Paste that in, click **Render**, then **Download** as PNG.

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+Enter` / `⌘+Enter` | Render |
| `Tab` | Insert 4 spaces |

## Tech

- [Mermaid.js v11](https://mermaid.js.org/) — runs entirely in the browser
- Plain HTML + CSS + ES modules — no framework, no build step
- SVG → PNG via Canvas API (2× resolution for retina screens)
- Hosted on [GitHub Pages](https://pages.github.com/)

## Contribute

Issues and PRs welcome. The entire app is a single file: [`docs/index.html`](docs/index.html).

## License

MIT
