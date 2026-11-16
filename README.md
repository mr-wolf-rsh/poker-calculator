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
standard poker hand ranking decides who takes the pot.

```
5H KS 9C 7D 9H  |  8D 3S 5D 5C AH
└── player 1 ──┘    └── player 2 ──┘
```

Strongest to weakest: straight flush · four of a kind · full house · flush · straight · three of
a kind · two pair · one pair · high card. Ties break on the ranks involved, then the remaining
cards; ace is high, and `A-2-3-4-5` counts as a straight.

## The seats

### 🔷 C#
`C#` `xUnit`

A console implementation of the hand comparison, tested with **xUnit**.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-csharp)**

### ☕ Java
`Java` `Maven` `JUnit`

The same comparison built with Maven (Java 8 archetype), tested with **JUnit**.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-java)**

### 🟨 JavaScript
`Node.js` `Jest`

The comparison in Node.js, tested with **Jest** (ES modules through `esm`).

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-js)**

### 🐍 Python
`Python` `Pipenv` `Pytest`

The comparison in Python, tested with **Pytest** inside a Pipenv environment.

**[Code](https://github.com/mr-wolf-rsh/poker-calculator-python)**

### 🐹 Go
`planned`

The next seat at the table — empty until a working, tested implementation exists.

---

## Shared deck

[`fixtures/pokerdata.txt`](fixtures/pokerdata.txt) is the canonical input every implementation
plays. Same deck, same result.

---

<p align="center">Built by <a href="https://github.com/mr-wolf-rsh">Renzo S.</a> · Licensed under <a href="LICENSE">GPL-3.0</a></p>
