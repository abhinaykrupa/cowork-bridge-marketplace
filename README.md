# cowork-bridge-marketplace

> ## ⚠️ Archived — you don't need this repo
>
> This marketplace existed to install the bridge via `/plugin install`. **That command doesn't work inside Claude Cowork**, which is the bridge's main audience, so this path is retired.
>
> **To set up the bridge, go to the main repo and follow its one-line setup:**
> **→ https://github.com/abhinaykrupa/cowork-to-code-bridge**
>
> You just paste one line into a Claude chat — no marketplace, no `/plugin`, no second setup.

---

A Claude Code plugin marketplace maintained by [Abhi Gadikoppula](https://github.com/abhinaykrupa).

## What's in this marketplace

Currently one plugin:

| Plugin | Description |
|---|---|
| [`cowork-to-code-bridge`](https://github.com/abhinaykrupa/cowork-to-code-bridge) | Let Claude Cowork run things on your Mac — scripts, builds, git, etc. Safe by design: token-protected, no internet listener, only runs scripts you approve. |

## Why this matters

Cowork can edit your files, but it can't reach your actual machine — it can't run your build, run your tests, or push to GitHub. This bridge fixes that, so a single Cowork chat can run a whole project end to end: build, run, test, and ship, all without leaving the conversation.

See the [plugin README](https://github.com/abhinaykrupa/cowork-to-code-bridge#what-you-can-build-with-it) for what that looks like step by step.

## Install

> **Using Cowork? You don't need this marketplace.** The `/plugin` command does not work inside Cowork. Install the bridge directly instead — one curl command on your Mac, then a plain-English request in Cowork. Full instructions: **https://github.com/abhinaykrupa/cowork-to-code-bridge#install-about-2-minutes**

This marketplace is only for the **interactive Claude Code terminal CLI** (the `claude` command you launch in a terminal), where `/plugin` is available:

```
/plugin marketplace add abhinaykrupa/cowork-bridge-marketplace
/plugin install cowork-to-code-bridge@cowork-bridge-marketplace
```

The first command registers this marketplace. The second installs the plugin from it. You still run the Mac-side `install.sh` (see the plugin repo) to start the daemon.

For full docs (what it does, how to set it up, security model), see the plugin repo: **https://github.com/abhinaykrupa/cowork-to-code-bridge**

## Updating (terminal CLI only)

```
/plugin marketplace update cowork-bridge-marketplace
```

## Maintainer note

This is a single-author marketplace. PRs adding unrelated third-party plugins won't be accepted — fork it and host your own instead.

## License

MIT. See [LICENSE](./LICENSE).
