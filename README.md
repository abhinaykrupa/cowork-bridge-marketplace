# cowork-bridge-marketplace

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

In Claude Code, run:

```
/plugin marketplace add abhinaykrupa/cowork-bridge-marketplace
/plugin install cowork-to-code-bridge@cowork-bridge-marketplace
```

The first command registers this marketplace. The second installs the plugin from it.

For full plugin docs (what it does, how to set it up, security model), see the plugin repo: **https://github.com/abhinaykrupa/cowork-to-code-bridge**

## Updating

```
/plugin marketplace update cowork-bridge-marketplace
```

## Maintainer note

This is a single-author marketplace. PRs adding unrelated third-party plugins won't be accepted — fork it and host your own instead.

## License

MIT. See [LICENSE](./LICENSE).
