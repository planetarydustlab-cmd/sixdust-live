# sixdust-live

Public **live-data feed** for [Sixdust Research](https://sixdust-research.vercel.app).

- `sector_hero_tw.json` / `sector_hero_us.json` — 資金浮力場（板塊輪動）即時資料，由 Mac mini 每約 10 分鐘（盤中）自動推送。
- **Derived / generated, NOT source of truth.** Holdings-blind（市場層級，無持倉）。
- 公開站 Hero + 台美總板塊頁以 `raw.githubusercontent.com/.../main/sector_hero_<mkt>.json?t=<ts>` 客端拉取（每 4 分鐘）。
- 單 commit、`--amend` force-push（不留歷史）。

取代舊架構（Supabase `live_state`）→ 零金鑰、零外部依賴、零 Vercel deploy。
