# lifeOS — 學生版

> 用 Obsidian + Claude Code 打造你的個人知識管理系統。

## 這是什麼？

lifeOS 是一個預先設計好的 [Obsidian](https://obsidian.md/) vault 模板，專為學生打造。它幫你用最簡單的方式開始：

- 每天記錄學習內容與反思
- 追蹤年度目標、每月回顧進度
- 整理讀書筆記、寫下你的原則
- 搭配 Claude Code，用 AI 幫你整理和回顧

不需要任何經驗，clone 下來就能用。

## 快速開始

### 1. 下載 vault

打開 Terminal，貼上這行：

```bash
cd ~/Desktop && git clone https://github.com/POYAOJUAN/lifeOS-demo.git lifeOS
```

> `lifeOS` 是資料夾名稱，可以改成你喜歡的名字（例如 `MyNotes`、`SecondBrain`）

### 2. 用 Obsidian 開啟

打開 Obsidian → 「Open folder as vault」→ 選 `Desktop/lifeOS`

### 3. 安裝推薦插件

見下方[推薦插件](#推薦安裝的第三方插件)章節。

### 4. 開始寫你的第一則 Daily Note

在 `Daily/` 資料夾新增一個 `YYYY-MM-DD.md` 檔案，或使用 Templater 自動建立。

## 資料夾說明

```
lifeOS/
├── Daily/        ← 每日筆記（最重要的習慣）
├── Monthly/      ← 月度回顧
├── Rules/        ← 你的原則（你相信什麼、你的底線）
├── Goals/        ← 目標追蹤
├── Finance/      ← 財務紀錄
├── Books/        ← 讀書筆記
├── Articles/     ← 你寫的文章
└── Templates/    ← 筆記模板（自動套用格式）
```

## 筆記模板

vault 內建三種模板，放在 `Templates/` 資料夾：

### Daily Note（每日筆記）

每天一則，記錄學習、困惑與反思。檔名格式：`YYYY-MM-DD.md`

包含區塊：
- **今天學了什麼** — 條列今天的學習重點
- **不懂的地方** — 之後可以問 Claude 或自己查
- **反思** — 今天有沒有比昨天進步一點點？

### Book Note（讀書筆記）

讀完一本書後整理重點。

包含區塊：
- **為什麼讀這本書** — 你的動機
- **重點摘要** — 三個以上的核心觀點
- **我的想法** — 你同意或不同意的地方
- **讀完後要做的事** — 把知識轉化為行動

### Monthly Review（月度回顧）

每月底回顧。檔名格式：`YYYY-MM.md`

包含區塊：
- **這個月做了什麼** — 成果盤點
- **學到什麼** — 知識與經驗總結
- **下個月想做的事** — 下一步計畫
- **反思** — 有沒有朝著自己想要的方向前進？

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

在 vault 資料夾裡啟動 Claude Code：

```bash
cd ~/Desktop/lifeOS
claude
```

Claude 會讀懂 vault 的結構，你可以直接用中文跟它對話。以下是幾個實用指令範例：

| 你說的話 | Claude 會做的事 |
|---------|---------------|
| 「幫我寫今天的 Daily Note」 | 在 `Daily/` 建立今天的筆記，套用模板格式 |
| 「做這個月的月度回顧」 | 讀取本月所有 Daily Notes，彙整成 `Monthly/YYYY-MM.md` |
| 「幫我整理這本書的讀書筆記：原子習慣」 | 在 `Books/` 建立讀書筆記，套用 Book Note 模板 |
| 「我最近都在學什麼？」 | 分析近期 Daily Notes，歸納你的學習軌跡 |
| 「幫我檢查目標進度」 | 比對 `Goals/` 和 `Monthly/` 的內容，回報進度 |

## 使用建議

1. **每天寫 Daily Note** — 不用多，三行就好。重點是養成習慣
2. **每月做一次回顧** — 回頭看自己走了多遠
3. **多用 `[[雙向連結]]`** — 把相關的筆記串起來，知識才會長出網路
4. **用 `#標籤` 分類** — 方便之後搜尋，例如 `#daily`、`#book`、`#goals`
5. **不用追求完美** — 先寫再說，格式可以之後再調整

## License

MIT
