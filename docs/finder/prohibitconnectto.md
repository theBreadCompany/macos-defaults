---
title: "Connect To Server..." Button
description: Allow connecting to a server using a button or shortcut.
head:
  - - meta
    - property: 'og:title'
      content: macOS defaults > Finder > "Connect To Server..." Button
  - - meta
    - property: "og:description"
      content: Allow connecting to a server using a button or shortcut.
---

# "Connect To Server..." Button

Allow connecting to a server using a button or shortcut.

NOTE: Disabling this still allows connecting by opening the server url in a browser as long as the protocol (ftp/smb/...) is handled by Finder.

<!-- break lists -->

- **Tested on macOS**:
  - Sonoma
- **Parameter type**: bool

## Set to `true` (default value)

Do not allow connecting to servers in Finder

```bash
defaults write com.apple.finder "ProhibitConnectTo" -bool "true" && killall Finder
```

## Set to `false`

Allow connecting to servers in Finder

```bash
defaults write com.apple.finder "ProhibitConnectTo" -bool "false" && killall Finder
```

## Read current value

```bash
defaults read com.apple.finder "ProhibitConnectTo"
```

## Reset to default value

```bash
defaults delete com.apple.finder "ProhibitConnectTo" && killall Finder
```
