# ETCswap V2 SDK (Archived)

> **This repo is archived.** The SDK has been migrated to the [sdks monorepo](https://github.com/etcswap/sdks).

Legacy standalone V2 SDK for ETCswap. The `etcswap` branch contains ETC-specific customizations (factory address override, init code hash override).

## Replacement Packages

| Package | Scope | Description |
|---------|-------|-------------|
| `@etcswapv2/v2-sdk-legacy` | [npm](https://www.npmjs.com/settings/etcswapv2/packages) | V2 SDK with viem support (used by v2-interface) |
| `@etcswapv2/v2-sdk` | [npm](https://www.npmjs.com/settings/etcswapv2/packages) | V2 SDK (monorepo version) |
| `@etcswapv2/sdk-core` | [npm](https://www.npmjs.com/settings/etcswapv2/packages) | Shared core utilities |

## ETC Customizations (etcswap branch)

- `src/entities/pair.ts` — `initCodeHashManualOverride` for ETC INIT_CODE_HASH
- `src/entities/pair.ts` — `factoryAddressOverride` for ETC Factory address
- `dist/` — Pre-built artifacts for direct consumption

## Related Repos

- [sdks](https://github.com/etcswap/sdks) — Active SDK monorepo (replacement)
- [v2-interface](https://github.com/etcswap/v2-interface) — Trading frontend (uses @etcswapv2/v2-sdk-legacy)
