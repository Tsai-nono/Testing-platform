# CLAUDE.md — Testing Platform

## 這個專案是什麼

個人技術實驗場，用來測試 Python、VBA 腳本與各種小工具。

## 開發慣例

- 腳本放 `scripts/`，依語言建子資料夾（`scripts/python/`、`scripts/vba/`）
- 新想法先開 GitHub Issue，整理後移進 `ideas/` 作為 Markdown 文件
- commit message 格式：`type: 描述`
  - `idea:` 新構思
  - `feat:` 新功能
  - `fix:` 修正
  - `exp:` 實驗性程式碼

## 常見任務

- **整理想法 issue 成文件**：把 issue 內容整理至 `ideas/YYYY-MM-DD-標題.md`
- **新增腳本**：在 `scripts/` 對應語言子資料夾建立，頂部加一行說明用途的註解
- **跨環境同步**：確保 push 後在另一台機器 pull，不要讓兩端差太多 commit
