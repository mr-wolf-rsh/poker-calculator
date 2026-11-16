<p align="center">
  <img alt="Poker Calculator" src="https://img.shields.io/badge/Poker%20Calculator-Polyglot%20Set-1B1B1B?style=for-the-badge">
</p>

<h1 align="center">♠️ Poker Calculator — Polyglot Set</h1>

<p align="center"><i>One exercise, one deck, five seats — the same poker-hand problem solved in several languages, each in its own repository.</i></p>

<p align="center">
  <img alt="C#" src="https://img.shields.io/badge/C%23-239120?logo=csharp&logoColor=white">
  <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
  <img alt="Go" src="https://img.shields.io/badge/Go-planned-00ADD8?logo=go&logoColor=white">
</p>

---

## The exercise

A round is one line of ten cards — the first five to player 1, the last five to player 2 — and
standard poker hand ranking decides who takes the pot. The full contract (input format, ranking,
tie-breakers, output shape) lives in [`spec.md`](spec.md).

```
5H KS 9C 7D 9H  |  8D 3S 5D 5C AH
└── player 1 ──┘    └── player 2 ──┘
```

## The seats

### 🔷 C#
`C#` `.NET Core` `xUnit`

A console implementation on **.NET Core** (SDK 2.2.x), tested with **xUnit**. It prompts for the
`pokerdata.txt` source and target directories, then prints each round's winner.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-csharp)**

### ☕ Java
`Java 8+` `Maven` `JUnit`

Built with **Maven** (Archetype Quickstart for Java 8, JDK 8+) and tested with **JUnit**. Run it
from a real terminal — VS Code's Output Console can't take input — and it asks for the source and
target directories.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-java)**

### 🟨 JavaScript
`Node.js` `Jest` `esm`

**Node.js** (12.x) with ES modules via `esm` and **ESLint**, tested with **Jest**. Prompts for the
source and target directories and writes the winner per round.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-js)**

### 🐍 Python
`Python 3` `Pipenv` `Pytest`

**Python 3** in a **Pipenv** environment, tested with **Pytest**. Prompts for the `pokerdata.txt`
source and target directories.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-python)**

### 🐹 Go
`planned`

The next seat at the table — empty until a working, tested implementation exists.

---

## How the set fits together

- **The house** (this repo) — the problem, the [`spec.md`](spec.md) contract, and the shared deck
  in [`fixtures/`](fixtures/).
- **Each player** (an implementation repo) — the algorithm plus its own README and run commands.
  Instructions are never duplicated here, because they differ per toolchain.
- **Same deck, same result** — every implementation plays the shared hands and must call the same
  winner. No house edge.
- **Always room for one more** — each new language lands as its own repository, so the set stays
  comparable instead of turning into one mixed codebase.

---

<p align="center">Built by <a href="https://github.com/mr-wolf-rsh">Renzo S.</a> · Licensed under <a href="LICENSE">GPL-3.0</a></p>
