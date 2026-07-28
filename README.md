# GameDev Shooter（槍戰類型層）

> `gamedev-shooter` — 射擊遊戲的武器手感、彈道、敵人 AI 與波次難度規範

這是一個 **AI skill**：一份規範文件，讓 AI 產出的成果達到可交付水準，而不是只有能動的骨架。
規範全文在 **[SKILL.md](./SKILL.md)**。

**依賴：[gamedev-feel](https://github.com/chris58530/gamedev-feel) ＋ [gamedev-3d](https://github.com/chris58530/gamedev-3d)（或 gamedev-2d）。** 未安裝時仍可運作，但請套用 SKILL.md 內的最小 fallback。

---

## 安裝

### Claude Code

```bash
/plugin marketplace add chris58530/gamedev-skills
```

```bash
/plugin install gamedev-shooter@gamedev-skills
```

或不透過 marketplace，直接從本 repo 安裝：

```bash
/plugin install chris58530/gamedev-shooter
```

### Codex / Cursor / Windsurf 等

Clone 本 repo，或把 [`SKILL.md`](./SKILL.md) 複製進你的專案，
並在專案的 `AGENTS.md`（或 `.cursorrules`）加一行指向它：

```markdown
處理遊戲開發需求時，先完整讀取 skills/gamedev-shooter/SKILL.md 並遵循其中規範。
```

### 其他 AI（ChatGPT、Gemini 等）

直接把 [`SKILL.md`](./SKILL.md) 全文貼進對話，接在你的需求前面即可。

---

## gamedev 系列

模組化設計，依需求疊加。基礎層是所有遊戲共用的，表現層依維度選，類型層依玩法選。

| 層級 | Skill | 用途 |
|------|-------|------|
| 基礎 | [gamedev-feel](https://github.com/chris58530/gamedev-feel) | 手感、音效、回饋、兩階段流程與自我驗收 |
| 表現 | [gamedev-3d](https://github.com/chris58530/gamedev-3d) | 3D 建模、渲染、材質、燈光 |
| 表現 | gamedev-2d | 精靈圖、序列動畫（規劃中） |
| 適配 | [gamedev-mobile](https://github.com/chris58530/gamedev-mobile) | 觸控操作、觸覺回饋、安全區、手機效能 |
| 類型 | [gamedev-shooter](https://github.com/chris58530/gamedev-shooter) | 槍戰射擊 |
| 類型 | gamedev-farming / puzzle / horror | 種田 / 解謎 / 恐怖（規劃中） |

索引：**[gamedev-skills](https://github.com/chris58530/gamedev-skills)**

---

## 授權

MIT
