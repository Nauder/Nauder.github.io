---
title: "Floowandereeze & Modding ETL"
description: "An ETL pipeline that reverse-engineers Yu-Gi-Oh! Master Duel to extract and structure card metadata: card names, art references, sleeves, fields, and more."
tags: ["Python", "pandas", "UnityPy", "Parquet", "GitHub Actions"]
github: "https://github.com/Nauder/floowandereeze-and-modding-etl"
featured: true
order: 3
---

## Overview

A data pipeline that reverse-engineers the global release of Yu-Gi-Oh! Master Duel to extract structured metadata from the game's Unity bundles. The output is Parquet files of card names, art references, sleeve IDs, deck boxes, field designs, and player icons, that feed the modding tools in the same project family.

## Features

- Extracts card artwork references, names, and descriptions (English)
- Processes card faces, deck boxes, fields, player icons, and sleeves
- Outputs structured Parquet files for efficient downstream consumption
- CI/CD with GitHub Actions running Pylint and Black on every push

## Stack

- **Python 3.8+** — core language
- **UnityPy** — Unity game asset reverse-engineering
- **pandas** — data transformation and Parquet output
- **PIL** — image processing
- **pytest** — test suite
- **GitHub Actions** — automated linting and formatting checks
