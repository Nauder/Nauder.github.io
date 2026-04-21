---
title: "Floowandereeze & Modding - Duel Links"
description: "A desktop modding tool for Yu-Gi-Oh! Duel Links that lets you replace card art, sleeves, and playmats, sister project to the Master Duel tool."
tags: ["Python", "PySide6", "SQLAlchemy", "UnityPy", "Windows"]
github: "https://github.com/Nauder/floowandereeze-and-modding-dl"
featured: false
order: 4
---

## Overview

A Windows desktop application for customizing Yu-Gi-Oh! Duel Links game assets. Like its Master Duel counterpart, it works by extracting and injecting Unity textures directly into the game — no manual asset editing required.

## Features

- Replace card artwork, card sleeves, and playmats
- Configurable compression and mipmap settings for exported assets
- Qt6 UI consistent with the rest of the modding tool family

## Stack

- **Python 3.8+** — core language
- **PySide6 / Qt6** — GUI framework
- **SQLAlchemy 2.0** — local database operations
- **UnityPy** — Unity asset extraction and injection
