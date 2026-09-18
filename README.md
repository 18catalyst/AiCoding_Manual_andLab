# Fixed-Supply SPL Token Training Project

This repository is intended to hold a local/devnet training project for fixed-supply SPL token creation.

[Training manual](docs/Coding_with_AI_Training_Manual.pdf)

## Status

This repository is currently documentation-first and unverified. The scaffold was not compiled, deployed, or otherwise verified in the authoring environment, so you must generate, install, and check the project locally before relying on it.

Use this material for localnet/devnet-only workflows. Do not send writes to mainnet, and do not add wallet credentials, recovery phrases, or private key material to the repository.

## Expected project layout

The intended project keeps these files at the repository root:

- `AGENTS.md`
- `Anchor.toml`
- `Cargo.toml`
- `package.json`
- `tsconfig.json`

The documented checks for the eventual scaffold are:

- `anchor build`
- `npm run typecheck`
- `anchor test --validator legacy`
- `npm --prefix app run build`

## Missing referenced files and directories

The current repository tree does **not** yet include the full training scaffold. Based on the intended layout and documented checks above, these referenced files or directories are still absent after this organization pass:

- `Anchor.toml`
- `Cargo.toml`
- `package.json`
- `tsconfig.json`
- `app/`
- program source directories such as `programs/`
- test directories such as `tests/`

Those items are intentionally listed as missing rather than reconstructed with unverified contents.
