# lifeOS — 學生版

> 用 Obsidian + Claude Code 打造你的個人知識管理系統。

## 快速開始

1. 打開 Terminal，貼上這行下載 vault：
   ```bash
   cd ~/Desktop && git clone https://github.com/POYAOJUAN/lifeOS-demo.git MyNotes
   ```
2. 打開 Obsidian → 「Open folder as vault」→ 選 `Desktop/MyNotes`
3. 安裝推薦插件（見下方）
4. 開始寫你的第一則 Daily Note！

## 資料夾說明

```
lifeOS-demo/
├── Daily/        ← 每日筆記（最重要的習慣）
├── Monthly/      ← 月度回顧
├── Rules/        ← 你的原則（你相信什麼、你的底線）
├── Goals/        ← 目標追蹤
├── Finance/      ← 財務紀錄
├── Books/        ← 讀書筆記
├── Articles/     ← 你寫的文章
└── Templates/    ← 筆記模板（自動套用格式）
```

## 推薦安裝的第三方插件

打開 Obsidian → 設定（`Cmd + ,`）→ Community plugins → 關閉「Restricted mode」→ Browse

搜尋以下插件名稱，逐一安裝並啟用：

| 插件 | 搜尋名稱 | 說明 |
|------|---------|------|
| **Calendar** | `Calendar` | 日曆視圖，點日期直接跳到當天的 Daily Note |
| **Templater** | `Templater` | 建立筆記時自動套用模板，不用手動排版 |
| **Dataview** | `Dataview` | 把筆記當資料庫查詢（進階功能，先裝著） |
| **Omnisearch** | `Omnisearch` | 全文模糊搜尋，找筆記超快 |
| **Tasks** | `Tasks` | 任務管理，支援到期日和優先級 |
| **Kanban** | `Kanban` | 看板視圖管理任務 |
| **Git** | `Obsidian Git` | 自動備份 vault 到 GitHub |

### 安裝後建議設定

**Calendar**
- 設定 → Calendar → 確認 Daily Note 格式為 `YYYY-MM-DD`

**Templater**
- 設定 → Templater → Template folder location → 輸入 `Templates`

**Obsidian Git**
- 設定 → Obsidian Git → Auto backup interval → 設為 `30`（每 30 分鐘自動備份）

## 搭配 Claude Code

在這個資料夾裡啟動 Claude Code：

```bash
cd ~/Desktop/lifeOS-demo
claude
```

Claude 會讀懂這個 vault 的結構，幫你寫筆記、整理資料、做月度回顧。
