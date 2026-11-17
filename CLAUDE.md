# KinkDeck

A swipe-based kink test for **PSY175 (Human Sexuality)**: 20 cards across 10 kinks, with an
instant breakdown. Live at <https://rossdavilla.github.io/KinkDeck/>.

`README.md` has the categories and the controls. The notes here are for changing it.

## Layout

The whole app is the single self-contained `index.html` — HTML, CSS and JS inline, no build step,
no dependencies.

## Conventions

- **Nothing is stored and nothing is sent.** No sign-up, no personal questions, no localStorage,
  no analytics, no backend. That promise is made on the page itself and in the README; keep it.
- Two statements per category, each category scored 0–100%, each result row a tap-to-expand
  explainer. Adding a kink means adding its two statements and its explainer in the same change,
  or the scoring goes lopsided.
- Swipe right / up / left map to Into it / Curious / Not for me, and every gesture also has a
  button and an arrow key (↑ ← →, Backspace to undo). Keep all three input paths working — it is
  used on phones in class and demoed on a laptop.
- It covers adult sexual content for a college audience: clinical, factual, non-judgmental, and
  the entertainment-only + consent note at the end of the README stays on the page.

## Publishing

GitHub Pages serves `main` from the repository root, so a push to `main` is the deploy. Already
listed in `data/sites.json` in the
[`rossdavilla.github.io`](https://github.com/rossdavilla/rossdavilla.github.io) repo under the
`PSY175` tag.
