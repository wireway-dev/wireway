# Wireway

Wireway is an HTTPS debugging proxy for the apps you build. Point an Android or iOS device, the iOS Simulator or your Mac
at it, and it shows and saves every request and response, HTTPS included.

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

## Support

Write to [support@wireway.dev](mailto:support@wireway.dev).
