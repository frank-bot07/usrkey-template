# USRKey — onboarding prototype

A self-contained prototype of the USRKey experience: **forge your key** (four
questions, share only what you choose) → your **Context Card** assembles → a
fresh AI greets you using *only* what you shared → a control panel shows which
tool sees what, over the plain markdown file underneath.

Single file, no build step. Open it:

```bash
python3 -m http.server 4599 --directory app
# → http://127.0.0.1:4599
```

or just open `app/index.html` in a browser.

The concept: the product is a markdown file; the *experience* is the wrapper.
The four questions are the ritual, the card is the payoff, the magic moment is
the hook, and control is the emotional core — you decide what every AI knows.
