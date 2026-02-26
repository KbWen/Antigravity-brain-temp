# AGENTS.md (Lite Version)

本檔定義專案的基本開發原則與指令入口，供 Codex 與 Antigravity 讀取。

## 核心憲法

- 必須遵守 `.agent/CONSTITUTION.md` 的原則。
- **正確性優先**：結果正確比速度重要。
- **規劃先行**：實作前必先執行 `/plan`。

## 核心指令

1. `/bootstrap`：初始化任務上下文。
2. `/plan`：規劃實作步驟與檔案。
3. `/implement`：根據計畫執行開發。
4. `/test`：執行最小必要驗證。
5. `/handoff`：輸出交接摘要。

## 安全規範

- 禁止洩漏 API Keys 或敏感憑證。
- 涉及資料異動時採可回退方式設計。

## 平台路徑

- Antigravity: `.agent/workflows/`
- Codex: `.agents/skills/`
