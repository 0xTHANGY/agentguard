# AgentGuard

**Planning stage. There is no code yet.**

AgentGuard is a project for the XRPL Commons AI Fintech hackathon, Agentic Finance track.

## Planned architecture

1. An AI agent initiates a payment.
2. A deterministic TypeScript policy engine evaluates the payment and returns `ALLOW`, `REQUIRE_APPROVAL`, or `DENY`. Payments that require approval can proceed only after approval. Denied payments stop.
3. A Ledger hardware wallet or a software signer signs the permitted payment.
4. The signed payment is submitted through the QuickNode XRPL testnet endpoint using `submitAndWait`.
5. The UI or CLI shows the transaction hash and `validated:true` once the transaction is validated.

## Planned tech stack

- TypeScript for the policy engine
- xrpl.js for XRPL client operations
- QuickNode XRPL testnet endpoint for submission and validation
- Ledger for hardware wallet signing, with a software signer as an alternative

## Status

All components are planned. Implementation has yet to begin.

## How to run

Not available yet.
