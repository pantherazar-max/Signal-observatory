# NEXUS-Ω Grammar Rules v0.1

## 1. Lexical form

Tokens are uppercase ASCII strings from the dictionary, except the terminal marker `Ω`. Separators are:
- a space between tokens in one clause,
- `·` for a close semantic grouping,
- `/` between clauses,
- `:` between a field label and its value.

## 2. Basic clause patterns

```
OBSERVATION := NEX · VEX [· ORI]
RESPONSE    := AUR · SYN · KAI
MESSAGE     := OBSERVATION / RESPONSE / Ω
```

Square brackets indicate an optional token; they are not literal characters.

## 3. Interpretation

- `NEX · VEX · ORI` means “observe the signal in its stated source context.”
- `AUR · SYN · KAI` means “a responding participant may choose to communicate.”
- `Ω` closes the message.

The presence of KAI is important: a response is optional. Removing KAI changes the intended semantics and makes the phrase invalid under v0.1.

## 4. Field notation

A field has the form `LABEL : VALUE`. Numeric values in puzzle fragments are indices or measurements defined by the puzzle; they are not opcodes.

## 5. Validity checks

A valid invitation message must:
1. contain an observation clause,
2. contain a response clause,
3. contain KAI in the response clause,
4. end with Ω,
5. contain no undeclared token.

## 6. Example

```
NEX · VEX · ORI / AUR · SYN · KAI / Ω
```

Plain-language reading: “Notice the signal and its context; a participant may choose to communicate; end.”
