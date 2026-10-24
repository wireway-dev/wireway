# Wireway

Wireway is an HTTPS debugging proxy for the apps you build. Point an Android or iOS device, the iOS Simulator or your Mac
at it, and it shows and saves every request and response, HTTPS included.

Wireway is a commercial app and its source code is not public. This repository is its public home: the
[releases](https://github.com/wireway-dev/wireway/releases) the app updates itself from, the
[issue tracker](https://github.com/wireway-dev/wireway/issues) for bugs and ideas, and the source of the website,
[wireway.dev](https://wireway.dev), in `site/`.

- **See the traffic of a device's apps**: requests and responses, with JSON, protobuf, gRPC, MessagePack and images
  shown readably, and the app that made each request on Android.
- **Change it on the way**: map a host to another server, answer requests locally, rewrite them, pause them at a
  breakpoint, or slow the connection down.
- **Work with AI agents**: Wireway includes an MCP server, so tools such as Claude Code and Codex can read and search
  the captured traffic.

## Requirements

- A Mac with Apple silicon, running macOS 26 or later.
- A Wireway license key. Wireway asks for one the first time it opens.

## Install

1. Download the latest `Wireway-<version>-macos-arm64.zip` from [Releases](https://github.com/wireway-dev/wireway/releases).
2. Open the zip and move **Wireway** to your Applications folder.
3. Open Wireway and enter your license key.

Builds are signed with a Developer ID and notarized by Apple.

## Updates

Wireway updates itself. Choose **Wireway > Check for Updates**, or turn on automatic checks in **Settings > General**.
Every update is signed, and Wireway checks the signature before it installs anything. Your settings, captured
traffic and certificate stay as they are.

## Bugs and ideas

[Open an issue](https://github.com/wireway-dev/wireway/issues/new). Say which version you run (**Wireway > About Wireway**),
what you did and what happened. Leave out anything private from the traffic you captured: hosts, tokens, request bodies.

When something fails, a few lines from Wireway's log help a lot. It's at `~/Library/Logs/Wireway/engine.log`, with the
run before in `engine.previous.log`. The log names your Mac's network address and the hosts you decrypt, so paste the
lines around the problem rather than the whole file.

If a HAR file or a saved session would show the problem, say so in the issue and send the file to support instead of
attaching it: exports hide credentials, but URLs and bodies stay as you captured them.

For anything you'd rather not post in public, write to [support@wireway.dev](mailto:support@wireway.dev). For security
problems, see [SECURITY.md](SECURITY.md).
