# Fazal AI Trading Bot (v2.0 — Standalone Android APK)

Lightweight, 60-second real-time Smart Money Concepts (SMC) signal scanner & alert engine for **XAUUSD (Gold)**, **XAGUSD (Silver)**, and **BTCUSD (Bitcoin)**.

## Features
- **Fast & Lightweight UI:** No heavy auto-loading chart iframes; fetches ~3 KB JSON OHLC candle data every 60 seconds.
- **Confirmed Closed-Candle SMC Engine:** Detects Sell-Side / Buy-Side Liquidity Sweeps + Fair Value Gaps (FVG) + EMA-50 Trend Alignment + ATR-based SL & TP1/TP2/TP3.
- **Strict Offline Guard:** Pauses signal generation when offline (`OFFLINE — PAUSED`) so synthetic/fake signals are never created.
- **True Android Background Service:** Uses `FOREGROUND_SERVICE_DATA_SYNC`, `PARTIAL_WAKE_LOCK`, and `@capacitor/local-notifications` for lock-screen sound, vibration & popup alerts.
- **Automatic GitHub APK Build:** Push to `main` branch and download the compiled `.apk` directly from the **Actions** tab.

## How to Build APK via GitHub Actions
1. Create a new repository on GitHub (e.g., `fazal-ai-trading-bot`).
2. Upload all files from this folder to the `main` branch.
3. Open the **Actions** tab on GitHub -> click **Build Fazal AI Trading APK** -> download `Fazal-AI-Trading-v2` artifact.
4. Install on Android and set **App Info -> Battery -> Unrestricted** for uninterrupted 24/7 background alerts.
