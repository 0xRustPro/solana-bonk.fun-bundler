# 🐶 Bonk.fun Multi-Wallet Bundle Trading Bot

A high-performance MEV bot built for Solana, optimized to trade $BONK via **Raydium v2** using **Jito bundles** with support for dynamic multi-wallet execution.

## 🚀 Features

- ✅ Supports **flexible multi-wallet bundling** (12+ wallets)
- ✅ Uses **Jito** relayer for atomic bundle submission
- ✅ Executes trades via **Raydium SDK v2**
- ✅ Dynamically constructs high-throughput parallel bundles
- ✅ Configurable compute unit pricing for priority inclusion

---

## 📸 Sample Bundles on Jito Explorer

These are **just examples** — the bot supports any number of wallets:

| Wallet Count | Jito Bundle                                                                                                  |
| ------------ | ------------------------------------------------------------------------------------------------------------ |
| 2 Wallets    | [🔗 View](https://explorer.jito.wtf/bundle/56ac378f193c9b90a4b6d2c52096a2d783653f300c343d59976691b2a6fcb184) |
| 9 Wallets    | [🔗 View](https://explorer.jito.wtf/bundle/8116172ad6bea279b6873020ac412eb36c9777b311b96ab38c58204637166bf1) |
| 12 Wallets   | [🔗 View](https://explorer.jito.wtf/bundle/eb6d075d4f3e065d5e127ec76c328e00e08d3608ee858a15fa13a21c8f922d98) |

---

## ⚙️ How It Works

1. Detects profitable arbitrage opportunities on **Raydium**
2. Constructs multiple swap transactions across separate wallets
3. Packages them into a **single atomic bundle** using Jito
4. Submits with priority settings for faster inclusion

---

## 🛠 Tech Stack

- [Solana Web3.js](https://solana-labs.github.io/solana-web3.js/)
- [Raydium SDK v2](https://github.com/raydium-io/raydium-sdk)
- [Jito-Solana](https://jito.network/)
- Custom multi-wallet bundler logic

---

## ⚡ Performance Tuning

Configure compute priority for inclusion in high-load conditions:

```ts
ComputeBudgetProgram.setComputeUnitPrice({ microLamports: 200_000 }); // High speed
```

Use higher microLamports for faster confirmation, or lower values for cheaper runs.

---

## 🧪 Planned Features

- Auto-retry bundles during congestion
- Live dashboard for monitoring bundle results
- Strategy plugin support (sandwich, backrun, etc.)
- Telegram/Discord notifications

---

## 📞 Contact Info

For MEV bot customization, consulting, or private collaboration:
**Open an issue** or reach out via Discord/Telegram (on request).

**Telegram**: [@Tru3B1iss](https://t.me/Tru3B1iss)
**X (Twitter)**: [@XTruebliss](https://x.com/XTruebliss)
**Discord**: [@trueb1iss](https://discord.com/users/1274339638668038187)

---
