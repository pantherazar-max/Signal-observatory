# Test Plan v0.1

## A. Language tests

- Confirm every token in examples exists in the dictionary.
- Confirm each invitation includes KAI.
- Confirm each complete message ends with Ω.
- Confirm clause ordering matches the grammar.
- Confirm unknown tokens are rejected rather than guessed.

## B. Puzzle tests

- Have at least two independent human reviewers attempt the puzzle.
- Have an independent AI system attempt the puzzle without access to the intended interpretation.
- Record the exact prompt/context supplied to each solver.
- Compare reasoning steps, not only final answers.
- Mark each conclusion as verified, plausible, or unsupported.

## C. Security tests before any gateway launch

- Confirm no secrets or credentials are present in the repository.
- Confirm no automatic link fetching or attachment execution exists.
- Confirm private keys are stored outside version control.
- Confirm rate limits, moderation, retention, and deletion procedures.
- Confirm no path from the gateway to Market, RTM, or trading infrastructure.

## D. Release gate

Do not publish an active call for private submissions until:
- the private contact route exists and is tested,
- publisher identity/pseudonym policy is decided,
- a reuse license is selected,
- the repository has been checked for secrets,
- the final public text is reviewed.
