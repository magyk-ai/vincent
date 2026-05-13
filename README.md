# Vincent

**Product marketing videos in your terminal.**

Vincent is a CLI tool that takes a product image and collaborates with you to produce a polished marketing video — scene generation, image editing, and video animation, all driven by Google Gemini and Veo 3.

```sh
npm install -g @magyk/vincent
```

Requires Node 25+ and a free Google Gemini API key.

- **Website:** [magyk.ai/vincent](https://magyk.ai/vincent)
- **npm:** [@magyk/vincent](https://www.npmjs.com/package/@magyk/vincent)
- **Get API key:** [Google AI Studio](https://aistudio.google.com/apikey)

---

## Filing issues

This repo is the public issue tracker for Vincent. The source code is developed privately.

**Before filing a bug, please run:**

```sh
vincent --self-test
```

and include the output in your report — it captures your node version, terminal type, binary availability, and settings state, which cuts resolution time significantly.

**What belongs here:**
- Bug reports (crashes, unexpected output, generation failures)
- Feature requests
- Usage questions you couldn't answer from `vincent --help`

**What doesn't belong here:**
- API key or billing issues → contact Google directly

---

## Changelog

Version history is on the [npm page](https://www.npmjs.com/package/@magyk/vincent?activeTab=versions). Run `vincent --version` to check what you have installed.
