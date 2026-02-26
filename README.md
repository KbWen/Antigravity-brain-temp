# AI Brain Template Lite (v0.1.0)

> **極簡版 AI Agent 工作流模板，專為 Google Antigravity 與 Codex Web 優化。**

## 🎯 專案理念

本模板將 AI Agent 的開發流程標準化，透過「指令優先」與「規範先行」的核心思維，讓開發過程更可控、更可追溯。

- **Correctness First**: 正確性優先，無法驗證的行為視為不安全。
- **Think Before Code**: 先規劃，後實作，避免盲目寫碼。
- **Context Hygiene**: 保持最小上下文，降低噪音。

> **參考來源**
> 本模板理念參考自 [Superpowers 專案](https://github.com/obra/superpowers)。

## 🚀 快速上手

1. **部署到專案**：將 `.agent`, `.agents`, `.antigravity`, `AGENTS.md` 複製到您的專案根目錄。
2. **開場指令**：在新對話開始時輸入：

   ```text
   請遵循 AGENTS.md 與 .agent/CONSTITUTION.md 的規範。
   先執行 /bootstrap。
   ```


## 🧪 用 GitHub Repository Template 建立自己的 Repo

若您想用「模板方式」建立自己的專案（而非手動複製檔案）：

1. 在 GitHub 開啟此模板 repo。
2. 點選 **Use this template** → **Create a new repository**。
3. 設定新 repo 名稱與可見性後建立。
4. clone 你的新 repo，直接開始使用本模板流程。

> 本模板核心是 `.agent`, `.agents`, `.antigravity`, `AGENTS.md`。
> `.github/` 屬於可選配，不是本模板運作的必要條件。

## 🛠️ 核心指令

| 指令 | 說明 |
| :--- | :--- |
| `/bootstrap` | 設定任務目標、限制與驗收標準。 |
| `/plan` | 列出檔案變更、實作步驟與風險。 |
| `/implement` | 依據已確認的計畫進行實作。 |
| `/test` | 執行驗證指令並記錄結果。 |
| `/handoff` | 產出交接摘要（進度、風險、下一步）。 |

## 🧩 檔案結構

- `.agent/CONSTITUTION.md`：核心工程規範。
- `.agent/workflows/`：Antigravity 工作流定義（含 `plan.md`、`test.md` 等）。
- `.antigravity/`：Antigravity 平台規則（例如 `rules.md`）。
- `.agents/skills/`：Codex Web 技能定義（`SKILL.md` 與相關設定）。
- `AGENTS.md`：跨平台通用指令定義。

## 🧭 路徑判定原則

- Antigravity 規則檔：`.antigravity/rules.md`
- Antigravity 工作流：`.agent/workflows/`
- Codex Skills：`.agents/skills/`

`tools/audit_ai_paths.sh` 會依上述路徑進行檢查，確保文件與稽核腳本一致。
