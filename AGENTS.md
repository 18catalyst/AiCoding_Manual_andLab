# Project Instructions

- Purpose: a local/devnet training project for fixed-supply SPL token creation.
- Rust and TypeScript use Anchor 1.2.0. Use @anchor-lang/core, web3.js v1, and the original Token Program. Do not add Token-2022 or Solana Kit imports.
- Supply is exactly 1,000,000 tokens at six decimals: 1,000,000,000,000 raw units.
- The mint PDA uses [b"mint", creator public-key bytes]. Each creator gets one mint.
- Initialization is signed by the creator, mints to the creator ATA, and removes mint authority in the same transaction. Freeze authority must remain absent.
- Never remove an account constraint just to make a failing test pass.
- Do not read or print wallet files, recovery phrases, or credentials.
- Do not send writes to mainnet. Keep changes small and explain affected invariants.
- Checks: anchor build; npm run typecheck; anchor test --validator legacy; npm --prefix app run build. Network tests need the documented Solana toolchain.
- Report checks actually run separately from proposed checks.
