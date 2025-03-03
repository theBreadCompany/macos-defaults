---
title: Emplacement des screenshots | Simulateur
---

::: warning Attention
La langue française n'est plus supportée sur macos-defaults.com. Cette page redirigera automatiquement vers la version anglaise correspondante en 2024.
:::

# Emplacement des screenshots

Préciser le chemin par défaut des screenshots du Simulateur.

Le dossier doit obligatoirement exister dans le système.

<!-- break lists -->

- **Testé sur macOS**:
  - Catalina
- **Type de paramètre**: string

## Avec la valeur `~/Pictures/Screenshots` (par défaut)

```bash
defaults write com.apple.iphonesimulator "ScreenShotSaveLocation" -string "~/Pictures/Screenshots"
```

## Avec la valeur `~/Pictures/Simulator Screenshots`

```bash
defaults write com.apple.iphonesimulator "ScreenShotSaveLocation" -string "~/Pictures/Simulator Screenshots"
```

## Lire la valeur courante

```bash
defaults read com.apple.iphonesimulator "ScreenShotSaveLocation"
```

## Remettre la valeur à l'état initial

```bash
defaults delete com.apple.iphonesimulator "ScreenShotSaveLocation"
```
