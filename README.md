# Vincent

**Product marketing videos in your terminal.**

Vincent is a CLI tool that takes a product image and collaborates with you to produce a polished marketing video — scene generation, image editing, and video animation, all driven by Google Gemini and Veo 3.

---

## Requirements

- **Node.js 22+** — Vincent requires Node 22 (LTS) or later; Node 24 recommended. If you're not on a recent version, use [nvm](https://github.com/nvm-sh/nvm):

  ```sh
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/HEAD/install.sh | bash
  # restart your shell, then:
  nvm install 24
  nvm use 24
  ```

- **Google Gemini API key** — free at [Google AI Studio](https://aistudio.google.com/apikey)

---

## Install

```sh
npm install -g @magyk/vincent
```

Then run `vincent` with a product image:

```sh
vincent ./product.jpg
```

---

## Links

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
