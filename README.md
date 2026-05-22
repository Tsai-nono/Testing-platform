# Testing Platform

個人技術實驗場 — Python、VBA 及其他。

---

## 快速開始

### 環境需求

```bash
# 確認 Python 版本
python --version   # 建議 3.10+

# 複製專案
git clone https://github.com/tsai-nono/testing-platform.git
cd testing-platform
```

---

## 多環境開發

### 公司 / 家中切換

每次換環境前，先同步：

```bash
# 拉最新進度
git pull origin main

# 確認目前在哪個環境
git config user.email
```

建議在不同機器設定不同的 git identity，方便追蹤：

```bash
# 公司機器
git config user.name  "Your Name (Work)"
git config user.email "work@company.com"

# 家中機器
git config user.name  "Your Name (Home)"
git config user.email "pter333@gmail.com"
```

### 分支慣例

| 分支 | 用途 |
|------|------|
| `main` | 穩定版本 |
| `dev/work-*` | 公司開發中 |
| `dev/home-*` | 家中開發中 |
| `idea/*` | 來自手機的想法草稿 |

---

## 手機記錄想法

最快的方式：用 **GitHub Issues**（手機瀏覽器或 GitHub App 皆可）

1. 開啟 [Issues](../../issues/new/choose)
2. 選擇 **快速想法** 模板
3. 填上標題 + 幾個關鍵字即可

想法整理後移進 [`ideas/`](./ideas/) 資料夾。

---

## 資料夾結構

```
testing-platform/
├── ideas/          # 整理過的想法與實驗構思
├── scripts/        # 工具腳本（Python、Shell）
├── .github/
│   └── ISSUE_TEMPLATE/   # 手機快速記錄模板
└── README.md
```

---

## 常用指令速查

```bash
# 建立新想法分支
git checkout -b idea/my-new-idea

# 快速提交（在任何環境都能用）
git add . && git commit -m "idea: 簡短描述" && git push -u origin HEAD
```
