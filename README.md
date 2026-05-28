# cowork-bridge-marketplace

A Claude Code plugin marketplace maintained by [Abhi Gadikoppula](https://github.com/abhinaykrupa).

## What's in this marketplace

Currently one plugin:

| Plugin | Description |
|---|---|
| [`cowork-to-code-bridge`](https://github.com/abhinaykrupa/cowork-to-code-bridge) | Let Claude in your browser (Cowork) run things on your Mac — scripts, builds, git, etc. Safe by design: token-protected, no internet listener, only runs scripts you approve. |

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
