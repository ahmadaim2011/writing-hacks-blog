---
layout: post
title: "Getting Started with GitHub Actions"
date: 2025-09-03
categories: [GitHub, CI/CD]
---

GitHub Actions let you **automate workflows** like testing or deploying.

Here’s a simple workflow file (`.github/workflows/hello.yml`):

```yaml
name: Say Hello
on: [push]
jobs:
  hello-world:
    runs-on: ubuntu-latest
    steps:
      - name: Print message
        run: echo "Hello from GitHub Actions!"
