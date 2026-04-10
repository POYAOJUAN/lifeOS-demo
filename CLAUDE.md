# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

這是一個 Obsidian vault（lifeOS 學生版），用來做個人知識管理。所有筆記內容使用**繁體中文**。

## Structure

```
Daily/        - 每日筆記（YYYY-MM-DD.md）
Monthly/      - 月度回顧（YYYY-MM.md）
Rules/        - 個人原則與框架
Goals/        - 目標追蹤
Finance/      - 財務紀錄
Books/        - 讀書筆記
Articles/     - 文章備份
Templates/    - 筆記模板（建立筆記時參照這裡的格式）
```

## 筆記格式規範

- 所有筆記使用 YAML frontmatter（`tags`, `date`, `created` 等欄位）
- 使用 `[[筆記名稱]]` 建立雙向連結
- 使用 `#標籤` 分類（如 `#daily`, `#book`, `#monthly`）

## 常見操作

### 建立今天的 Daily Note
根據 `Templates/Daily Note.md` 的格式，在 `Daily/` 建立今天的筆記。檔名格式：`YYYY-MM-DD.md`。包含三個區塊：今天學了什麼、不懂的地方、反思。

### 月度回顧
讀取當月所有 Daily Notes，彙整為 `Monthly/YYYY-MM.md`，套用 `Templates/Monthly Review.md` 格式。

### 讀書筆記
在 `Books/` 建立筆記，套用 `Templates/Book Note.md` 格式。包含：為什麼讀、重點摘要、我的想法、讀完後要做的事。
