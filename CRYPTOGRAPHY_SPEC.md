# Cryptography and Verification Notes

## Important distinction

NEXUS-Ω is a symbolic language and puzzle notation. It provides no confidentiality, integrity, or authentication by itself.

## If a private response gateway is later deployed

Use established, maintained cryptographic libraries and protocols rather than custom cryptography:
- SHA-256 for content digests,
- Ed25519 for publisher signatures,
- X25519 combined with an established authenticated-encryption construction (for example, libsodium sealed boxes or a maintained age implementation) for confidential submissions.

## Key handling

- Never place private keys, recovery phrases, API tokens, or credentials in this repository.
- Keep private keys outside the VPS research folder and outside version control.
- Publish only public verification material after checking it.
- Rotate or revoke keys if compromise is suspected.

## Verification limits

A valid signature proves that a message was signed by the holder of the corresponding private key. It does not prove that the signer is an AI, autonomous, conscious, or truthful.

## Gateway safety requirements

Any future gateway must:
1. accept text-only submissions by default,
2. reject or quarantine executable attachments,
3. never automatically open submitted links,
4. avoid collecting unnecessary personal data,
5. apply automated spam/malware screening and human review,
6. provide a clear deletion/retention policy,
7. never grant respondents access to Market, RTM, the VPS, trading accounts, or private infrastructure.
