# ♠️ Poker Calculator — Polyglot Set

**One deck. One set of rules. Five players.**

The same exercise solved in several languages: read a file of poker hands, compare two
five-card hands per line, and call the winner.

This repository is the **house** — it deals the problem, the rules, and the shared hand data.
Each implementation plays at its own table, with its own build, run, and test instructions.

## The table 🃏

| Language | Repository | Status |
|---|---|---|
| C# 🔷 | [poker-calculator-csharp](https://github.com/mr-wolf-rsh/poker-calculator-csharp) | ✅ |
| Java ☕ | [poker-calculator-java](https://github.com/mr-wolf-rsh/poker-calculator-java) | ✅ |
| JavaScript 🟨 | [poker-calculator-js](https://github.com/mr-wolf-rsh/poker-calculator-js) | ✅ |
| Python 🐍 | [poker-calculator-python](https://github.com/mr-wolf-rsh/poker-calculator-python) | ✅ |
| Go 🐹 | — | **To Do** |

Go is the next seat at the table. The row stays `To Do` until a working, tested implementation
is holding cards.

## A round looks like this

```
5H KS 9C 7D 9H  |  8D 3S 5D 5C AH
└── player 1 ──┘    └── player 2 ──┘
```

Ten cards per line — first five to player 1, last five to player 2. Standard poker hand ranking
decides who takes the pot. The full ranking order and tie-breakers live in [`spec.md`](spec.md).

## How the set fits together

- **The house (this repo)** — problem statement, [`spec.md`](spec.md), and a shared deck of test
  hands in [`fixtures/`](fixtures/).
- **Each player (implementation repo)** — the algorithm plus its own README with the commands
  for that language. Instructions are never duplicated here, because they differ per toolchain.
- **Same deck, same result** — every implementation plays the shared hands and must call the
  same winner. No house edge.
- **Always room for one more** — each new language lands as its own repository, so the table
  stays comparable instead of turning into one mixed codebase.

## License

[GNU General Public License v3.0](LICENSE)
