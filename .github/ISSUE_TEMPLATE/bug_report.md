---
name: Bug report
about: Something isn't working
labels: bug
---

**What happened?**


**What did you expect?**


**Steps to reproduce**
1.
2.

**Diagnostics bundle** (best for a misbehaving session)
Run `/diagnostics` in the app (or `vincent diagnostics --latest` after quitting) and drag the `.zip` onto this issue. It bundles the session transcript, logs, and an environment report — no API keys, and your home path is rewritten to `<HOME>`. This covers the environment details below, so you can skip them if you attach it.

**`vincent --self-test` output** (and, for a render/ffmpeg problem, also `vincent doctor`)
```
(paste output here)
```

**Environment**
- OS:
- Node version ():
- Terminal:
- Vincent version ():
