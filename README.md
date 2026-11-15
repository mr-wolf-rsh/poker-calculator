# Poker Calculator — Polyglot Set

One exercise, implemented in several languages. Each implementation reads a file of poker
hands, compares two five-card hands per line, and reports the winner.

This repository is the **hub**: it owns the problem statement, the input/output contract, and
the shared fixtures. The implementations live in their own repositories, each with its own
build, run, and test instructions.

## Implementations

| Language | Repository | Status |
|---|---|---|
| C# | [poker-calculator-csharp](https://github.com/mr-wolf-rsh/poker-calculator-csharp) | ✅ |
| Java | [poker-calculator-java](https://github.com/mr-wolf-rsh/poker-calculator-java) | ✅ |
| JavaScript | [poker-calculator-js](https://github.com/mr-wolf-rsh/poker-calculator-js) | ✅ |
| Python | [poker-calculator-python](https://github.com/mr-wolf-rsh/poker-calculator-python) | ✅ |
| Go | — | **To Do** |

Go is the next planned implementation. The row stays `To Do` until a working, tested
implementation exists.

## How the set fits together

- **This repo** — problem statement, [`spec.md`](spec.md), and shared test data in [`fixtures/`](fixtures/).
- **Each implementation repo** — the algorithm plus its own README with the commands to
  build, run, and test that language. Instructions are never duplicated here, because they
  differ per toolchain.
- **Same input, same answers** — every implementation consumes the shared fixtures and
  produces the same results as the others.
- **Growing over time** — each new language lands as its own repository, so the set stays
  comparable instead of turning into one mixed codebase.

## License

[GNU General Public License v3.0](LICENSE)
