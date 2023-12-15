# Recursive proofs with Noir

Recursive proofs mean you prove that another proof is correct. A bit of a proofinception but bear with me:

- You prove that `x != y`
- You pick that proof and send it to another circuit (the "outer" proof)
- You generate the outer proof and verify it

Why is this useful? In this example, it doesn't do much. But you could verify two proofs within a proof, which can be incredibly useful. You could also avoid verifying stuff on-chain for turn-based games, for example.

## Getting Started

1. Install dependencies by running `yarn`
2. Run `yarn dev`

## Testing

To run the [test file](./test/index.ts), try `yarn test`
