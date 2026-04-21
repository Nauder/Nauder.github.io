---
title: "Floowandereeze & Modding"
description: "A desktop modding tool for Yu-Gi-Oh! Master Duel that lets you replace card art, sleeves, fields, icons, and more. Built with Python and PySide6."
tags: ["Python", "PySide6", "SQLAlchemy", "UnityPy", "Windows"]
github: "https://github.com/Nauder/floowandereeze-and-modding-qt"
featured: true
order: 2
---

## Overview

A Windows desktop application for customizing Yu-Gi-Oh! Master Duel game assets. It extracts and replaces Unity textures directly, letting players swap card artwork, sleeves, duel fields, backgrounds, and player icons without manual asset editing.

## Features

- Replace card art, card faces, sleeves, duel fields, home backgrounds, and player icons
- Modify card names and descriptions
- Configurable compression and mipmap settings for exported assets
- Clean Qt6 UI built with PySide Designer

## Stack

- **Python 3.8+** — core language
- **PySide6 / Qt6** — GUI framework
- **SQLAlchemy 2.0** — local database operations
- **UnityPy** — Unity asset extraction and injection
- **PyInstaller** — standalone Windows executable packaging
