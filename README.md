# Github-action
🚀 GitHub Actions – Node.js Version Check

This repository demonstrates a basic GitHub Actions CI workflow that checks the Node.js version on every push using GitHub-hosted runners.

📌 Project Purpose

Learn GitHub Actions fundamentals

Understand CI workflow structure

Verify Node.js setup in CI/CD pipelines

🛠️ Technologies Used

GitHub Actions

Node.js

YAML

Ubuntu Runner

📂 Repository Structure
.github/
└── workflows/
    └── all file 
README.md

⚙️ Workflow Details

Trigger: Runs on every push

Runner: ubuntu-latest

Steps:

Checkout repository

Setup Node.js

Display Node.js version

🧾 Sample Workflow Code
name: Node.js Version Check

on: push

jobs:
  check-node-version:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v4

      - name: Setup Node.js
        uses: actions/setup-node@v4
        with:
          node-version: '20'

      - name: Check Node.js version
        run: node -v

✅ Output Example
v20.x.x

🎯 Learning Outcome

Basic GitHub Actions workflow creation

YAML syntax and indentation

Using official GitHub actions

CI automation basics

📌 Future Enhancements

Add npm install

Run unit tests

Docker build & push

Terraform / AWS CI pipeline
