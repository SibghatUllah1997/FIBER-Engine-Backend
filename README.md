# FIBER Engine Backend

Backend orchestration for the **MultiSwap FIBER** cross-chain engine: Express API, scheduled cron workers, Web3/Hardhat integration, and asset routing checks (FAC / RIA) used by the bridge stack.

**Architect / engineering:** [Muhammad Sibghat Ullah](https://github.com/SibghatUllah1997)  
**Related:** [MultiSwap](https://github.com/SibghatUllah1997/MultiSwap) · [Ferrum docs](https://docs.ferrumnetwork.io/ferrum-network-ecosystem/v/multiswap-and-multichain-liquidity-pool-bridge/)

## Stack

TypeScript · Node.js · Express · Web3 · Hardhat · PM2 · MongoDB

## Install

```bash
npm install
```

## Local development

```bash
npm run nodemon-dev-api
npm run nodemon-dev-cron
```

## Build

```bash
npm run build
```

## Deploy (PM2)

| Environment | API | Cron |
|-------------|-----|------|
| Dev | `npm run pm2-dev-api` | `npm run pm2-dev-cron` |
| Staging | `npm run pm2-staging-api` | `npm run pm2-staging-cron` |
| Production | `npm run pm2-prod-api` | `npm run pm2-prod-cron` |

Default HTTP port: **8080** (configurable in `server.ts`).

## License

See repository `LICENSE`.
