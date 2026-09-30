# Quick Start Guide

This guide will help you understand how functions work in this scripting language.

## Basic Concepts

Functions always start with a dollar sign (`$`), followed by the function name, and enclose their parameters inside square brackets (`[...]`).

### Syntax Format

```text
$functionName[arg1;arg2;...]
```

- **Arguments:** Separated by a semicolon `;` when a function accepts multiple inputs.
- **Order:** Functions are evaluated in order from top to bottom.

## Building Your First Embed

To send an embed response, combine embed structure functions with a message trigger:

```bhscript
$title[Welcome Server Member!]
$description[We are glad to have you here.]
$thumbnail[https://example.com/welcome-avatar.png]
$sendMessage[Welcome!]
```
