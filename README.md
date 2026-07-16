# AI demos

Nine interactive visualizations that walk from Turing's 1936 thought experiment to today's language models. Each demo is a single HTML file — open it in a browser and play with the idea instead of only reading about it.

Aimed at students, educators, and anyone who wants a clearer mental model of how we got from "Can machines think?" to ChatGPT.

## Catalog

| Demo | Focus |
|------|--------|
| **[Timeline](timeline/)** | Scrollable AI/NLP milestones (1936–2026), with hardware and algorithm strips showing how chips and math converged |
| **[Turing Machine](turing-machine/)** | Step a deterministic TM through four programs: binary increment, palindrome check, unary addition, busy beaver |
| **[Nondeterministic TM](nondeterministic-turing-machine/)** | Same machine, but it branches — useful intuition for computational complexity and P vs NP |
| **[Turing Test](turing-test/)** | Play the judge: read parallel conversations and decide which side is human |
| **[Word Vectors](word-vectors/)** | Drag embeddings in vector space; try arithmetic like `king − man + woman ≈ queen` |
| **[CNN](cnn/)** | Step through a LeNet-style convolutional neural network: convolution, pooling, and classification on a handwritten digit |
| **[Transformer](transformer/)** | Walk tiny vectors from tokens through attention to a next-word prediction — the core of modern LLMs |
| **[Chat](chat/)** | How a raw completion model becomes a conversational assistant: chat templates, not a smarter model |
| **[Tool Usage](tool-usage/)** | How models call tools — structured requests an external system runs and feeds back |

## Constraints

- **No build.** One HTML file per demo, inline CSS and JS. No framework, no npm.
- **One screen.** Each viz fits a single viewport (the timeline scrolls horizontally by design).

## Run locally

Open any `index.html` directly, or serve the folder:

```bash
cd demo-uis
python3 -m http.server 8000
# http://localhost:8000/timeline/
```

## GitHub Pages

Pushes to `main` deploy via [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

In the repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
