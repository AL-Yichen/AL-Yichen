# Hi, I'm AL-Yichen 👋

- 🔭 I'm currently working on AI-related projects, Minecraft mods, and web applications.
- 🌱 I'm currently learning AI algorithms, machine learning, deep learning, LLMs, and the mathematics behind AI.
- 💻 I have been learning both frontend and backend development, while continuing to improve my programming skills with Python and Java.
- 👯 I'm looking to collaborate on open-source AI/LLM projects and interesting experimental projects.
- 💬 Ask me about AI, web development, Minecraft modding, AstrBot, or the things I'm currently experimenting with.
- 📚 I'm also learning English and preparing for my next academic step.
- 📫 How to reach me: GitHub Issues or Discussions are welcome!

> 🐋 Learning, building, breaking, fixing, and learning again.

I build small, focused tools for the **DeepSeek Harness (dsh)** ecosystem — mostly
browser-side client plugins that fix one specific annoyance properly instead of
piling on features.

<!-- Profile-view counter. If it ever renders blank, delete this <picture> block —
     a broken counter image is worse than no counter. -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://count.getloli.com/@AL-Yichen?name=AL-Yichen&theme=gelbooru&padding=7&offset=0&align=top&scale=1&pixelated=1&darkmode=auto">
  <img alt="AL-Yichen profile views" src="https://count.getloli.com/@AL-Yichen?name=AL-Yichen&theme=gelbooru&padding=7&offset=0&align=top&scale=1&pixelated=1&darkmode=auto">
</picture>

## What I'm building

**[dsh-fullscreen-input](https://github.com/AL-Yichen/dsh-fullscreen-input)** — a full-screen
panel for the dsh composer. `Enter` only ever inserts a newline there; `Ctrl+Enter` is the
only key that sends. That sidesteps the host composer's 10 ms composition grace window, where
a Chinese IME's `Shift+Enter` is easily misread as "send".

[![npm](https://img.shields.io/npm/v/dsh-fullscreen-input?color=4176e6)](https://www.npmjs.com/package/dsh-fullscreen-input)
[![License](https://img.shields.io/github/license/AL-Yichen/dsh-fullscreen-input?color=4176e6)](https://github.com/AL-Yichen/dsh-fullscreen-input/blob/main/LICENSE)
[![DSH](https://img.shields.io/badge/DSH-%3E%3D0.2.0--rc.1%20%3C0.3.0--0-4176e6)](https://github.com/AL-Yichen/dsh-fullscreen-input#兼容性)

Install it with:

```sh
dsh plugin --profile web add dsh-fullscreen-input
```

## How I work

- **Fix the cause, not the symptom.** The full-screen panel exists because a 10 ms timing
  window in the host keymap cannot be patched from outside — so the panel removes the
  ambiguity instead of fighting it.
- **Keep the surface small.** That plugin makes no network requests, uses no `ctx.fs` or
  `ctx.shell`, and stores exactly one preference key. Its `SECURITY.md` states the whole
  attack surface in a single page.
- **Verify on the real machine.** Several bugs in that codebase were invisible to static
  checks and offline tests — they only showed up once actually loaded.

---

<sub>If [dsh-fullscreen-input](https://github.com/AL-Yichen/dsh-fullscreen-input) is useful to you, a ⭐ is the best support.</sub>
