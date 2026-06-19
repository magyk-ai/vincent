# Vincent

**Make video in your terminal.**

Vincent is a conversational AI agent in your terminal for making videos. Turn a **product photo** into a marketing video, or a **plain-language idea** into a narrated, multi-scene **story** video — Vincent drafts a storyboard for your review, renders when you approve, then keeps editing by conversation. Gemini + Veo are the zero-config default (one API key); Replicate, fal, ElevenLabs, and OpenAI are optional.

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

- **ffmpeg** — required to render video. Run `vincent doctor` to check it, or `vincent setup` (macOS/Linux) to install a verified build, with your consent. On macOS, Homebrew's `ffmpeg` no longer bundles **libass** (needed to burn subtitles into the video), so prefer `vincent setup` — `brew install ffmpeg` still renders video, but without captions.

---

## Install

```sh
npm install -g @magyk/vincent
```

Then start a conversation:

```sh
vincent                  # chat — pick Product or Story mode
vincent ./product.jpg    # start with a product image loaded
```

In **Story mode**, describe an idea and Vincent drafts a storyboard for your review before it renders. In **Product mode**, it turns a product photo into a marketing video. Switch anytime with `/mode`.

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

**If a specific session misbehaved,** run `/diagnostics` in the app (or `vincent diagnostics --latest` after quitting) and attach the `.zip` it writes to your current directory. It bundles that session's transcript, logs, and an environment report into one file — with no API keys (those live outside the session folder) and your home path rewritten to `<HOME>`.

**What belongs here:**
- Bug reports (crashes, unexpected output, generation failures)
- Feature requests
- Usage questions you couldn't answer from `vincent --help`

**What doesn't belong here:**
- API key or billing issues → contact Google directly

---

## Changelog

Version history is on the [npm page](https://www.npmjs.com/package/@magyk/vincent?activeTab=versions). Run `vincent --version` to check what you have installed.
