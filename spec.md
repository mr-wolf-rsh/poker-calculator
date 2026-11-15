# Poker Calculator — Shared Contract

This document is the single definition of the exercise. Every implementation must follow it.

## Input

A plain-text file, conventionally named `pokerdata.txt`, with one round per line.

- Each line holds **10 cards** separated by single spaces.
- The **first 5 cards** belong to player 1.
- The **last 5 cards** belong to player 2.
- Each card is a rank followed by a suit, with no separator:
  - rank: `2`–`9`, `T` (ten), `J`, `Q`, `K`, `A`
  - suit: `C` (clubs), `D` (diamonds), `H` (hearts), `S` (spades)

Example line:

```
5H KS 9C 7D 9H 8D 3S 5D 5C AH
```

Player 1: `5H KS 9C 7D 9H` · Player 2: `8D 3S 5D 5C AH`

## Evaluation

Compare the two five-card hands using standard poker hand ranking, strongest to weakest:

1. Straight flush
2. Four of a kind
3. Full house
4. Flush
5. Straight
6. Three of a kind
7. Two pair
8. One pair
9. High card

Ties are broken by the ranks involved, then by the remaining cards in descending order. Ace is
high (`A` > `K`), and a straight may end with `A-2-3-4-5`.

## Output

Per round, the result is the winning player (`Player 1` or `Player 2`). The summary is the total
number of wins for each player.

The exact output file or directory is chosen at runtime by each implementation; the program
prompts for a source file and a target location.

## Shared fixtures

[`fixtures/pokerdata.txt`](fixtures/pokerdata.txt) is the canonical input used across
implementations. It is copied from the original exercise data and must not diverge.

## Status

The input format and hand rankings above match the existing implementations. The output shape
still needs to be confirmed as identical across all four before this contract can be called
verified — tracked as a follow-up.
