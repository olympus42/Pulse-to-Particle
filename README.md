# Scale 🧬

> An interactive descent through the human body — from a live pulse on your wrist all the way down to a single carbon atom forged in a star.

**[▶ Live demo](https://<your-username>.github.io/pulse-to-particle)** · Built with zero dependencies · One HTML file

![Scale walkthrough](scale_walkthrough.gif)

---

## The idea

Biology happens across an absurd range of scales. Your heartbeat is something you can feel on your wrist — and the very same rhythm reaches all the way down to the mitochondria burning oxygen inside a single cell, and to the atoms those cells are built from.

**Scale** is a "Powers of Ten" for the human body. You start on an Apple Watch reading a live heartbeat, then descend through six orders of magnitude — heart, cell, neuron, DNA, atom — each one a fully animated, interactive scene. The beat you set at the top propagates all the way down: set your pulse on the wrist and the cell, the helix, and even the atomic nucleus pulse in time with it.

It's meant to sit at the intersection I care about: **applied biology, physics, and Apple-grade design.**

## The six scales

| # | Scene | Scale | Field |
|---|-------|-------|-------|
| 01 | **The Wrist** | 10⁰ m · one metre | wearables / physiology |
| 02 | **The Heart** | 10⁻¹ m · ten centimetres | anatomy / physiology |
| 03 | **The Cell** | 10⁻⁵ m · ten microns | cell biology |
| 04 | **The Neuron** | 10⁻⁷ m · the synapse | neuroscience |
| 05 | **The Helix** | 10⁻⁹ m · two nanometres | genomics |
| 06 | **The Atom** | 10⁻¹⁰ m · one ångström | chemistry / physics |

## What you can do

- **Set your heartbeat** on the wrist and watch a real PQRST ECG waveform, activity ring, and BPM respond live — then feel that rhythm carry down through every scene below.
- **Reveal the cell's machinery** — tap the nucleus, mitochondria, or membrane to identify it; the mitochondria brighten on every beat as the cell draws oxygen.
- **Fire a neuron** — trigger an all-or-nothing action potential and watch the −70 mV → +40 mV spike sprint down the axon to the synapse, plotted on a live membrane-potential graph.
- **Turn the double helix** — drag to rotate the DNA, hover a rung to read its base pair (A–T / G–C).
- **Meet carbon** — orbiting electrons around a six-proton nucleus, with a toggle between the classic Bohr model and a probabilistic electron cloud.
- **Take the guided tour** — one button auto-flies through all six scales, performing each scene's key interaction, with a progress bar you can stop anytime.

Navigate with the on-screen depth rail, the ↑ / ↓ arrow keys, scroll, swipe, or number keys `1`–`6`.

## Built with

No frameworks. No build step. No dependencies. **One self-contained HTML file (~60 KB).**

- **Vanilla JavaScript** — ~1,000 lines, no libraries
- **Canvas 2D** — every organ, cell, neuron, helix, and atom is drawn procedurally in real time with `requestAnimationFrame`
- **CSS custom properties** — a single `--accent` token recolors the entire interface as you descend, shifting smoothly from cardiac red through cellular green to electric indigo, gold, and atomic cyan
- **Type** — Apple's `-apple-system` stack (real SF Pro on Apple devices), with **Inter** as the web fallback and **JetBrains Mono** for the scientific readouts

The whole thing respects `prefers-reduced-motion` and is keyboard-navigable.

## Run it locally

No tooling required — it's a single static file.

```bash
# clone
git clone https://github.com/<your-username>/pulse-to-particle.git
cd pulse-to-particle

# open it directly...
open index.html          # macOS

# ...or serve it (recommended, so fonts load cleanly)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Because it's one static file, it hosts anywhere:

- **GitHub Pages** — Settings → Pages → deploy from `main`. Lands at `https://<your-username>.github.io/pulse-to-particle`.
- **Netlify Drop** — drag `index.html` onto [app.netlify.com/drop](https://app.netlify.com/drop) for an instant URL.
- **Vercel / Cloudflare Pages** — import the repo, no config needed.

> Note: fonts are loaded from Google Fonts, so the page needs an internet connection to render exactly as designed.

## A note on the science

The physiology and molecular biology here are accurate but **stylized** — this is procedural art in service of intuition, not a rendered simulation. The ECG waveform, the −70/+40 mV action potential, the A–T / G–C base pairing, and carbon's 2-4 electron configuration are all faithful to the real thing. The carbon atom in particular uses the iconic **Bohr model**; the "electron cloud" toggle is there to acknowledge that real electrons live in probability clouds, not neat orbits.

## About

Built by an **Applied Biology** student heading to the **University of Bonn** — with a long-term aim of working at the intersection of biology, physics, and space science. Scale is a small love letter to how astonishing living systems are when you look at them across every scale at once.

## Credits

**Proudly built on Apple's MacBook Air.**
Typeset in SF Pro · Inter · JetBrains Mono.

## License

MIT © <Your Name>
