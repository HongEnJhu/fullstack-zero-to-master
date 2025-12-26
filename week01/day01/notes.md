# Week 01 / Day 01 — Terminal 基礎與 Repo 結構

## Context
- OS: Windows
- Shell: PowerShell / Git Bash（擇一操作；避免混用）
- Repo: `fullstack-zero-to-master`

---

## Goals
- 能用 Terminal 操作檔案/資料夾：定位、建立、移動/改名、複製、刪除
- 能建立固定的學習 repo 結構（week/day/檔案規格）
- 能用 Git 追蹤變更並提交（commit）到遠端

---

## Core Concepts

### Working Directory（工作目錄）
- 你目前「所在的資料夾」。
- 任何操作前先確認目前位置，避免對錯地方動手。

### Path（路徑）
- **Absolute path**：從最上層一路指到目標
- **Relative path**：從目前工作目錄出發到目標

### `.` and `..`
- `.`：現在這層
- `..`：上一層

### Command Shape（指令形狀）
- `command [options] <target>`
- options 會改變行為；target 是檔案/資料夾/路徑

---

## Commands Cheat Sheet

### Bash / Git Bash / WSL
- `pwd`：顯示目前位置（工作目錄）
- `ls`：列出檔案與資料夾
- `cd`：切換目錄
- `mkdir`：建立資料夾
- `touch`：建立檔案（或更新修改時間）
- `rm`：刪除檔案（刪資料夾通常需遞迴選項）
- `cp`：複製檔案/資料夾
- `mv`：移動（也常用來改名）
- `cat`：輸出檔案內容
- `less`：分頁檢視檔案內容
- `grep`：搜尋關鍵字
- `|`：pipe，把左邊輸出交給右邊當輸入
- `nano`：文本編輯器，退出(ctrl+Y)

> 註：`ls` 是 List（列出），不是 Segment。

### PowerShell（含常見別名）
> PowerShell 很多「像 Linux 的指令」其實是 alias。

- 目前位置：`Get-Location`（alias：`pwd`）
- 列出：`Get-ChildItem`（alias：`ls`, `dir`）
- 切換目錄：`Set-Location`（alias：`cd`）
- 建檔案：`New-Item -ItemType File <name>`
- 建資料夾：`New-Item -ItemType Directory <name>`（或 `mkdir`）
- 看內容：`Get-Content <file>`（alias：`cat`）
- 搜尋字串：`Select-String "keyword" <file>`（類似 `grep`）
- 複製：`Copy-Item`
- 移動：`Move-Item`
- 改名：`Rename-Item`
- 刪除：`Remove-Item`（資料夾常搭配 `-Recurse -Force`）

---

## Safety / Debug Checklist（操作前必做）
- 先 `pwd`：我在哪？
- 再 `ls`：目標存在嗎？
- 做刪/移/改名：只對「確定的相對路徑」動手
- Git 以 `git status` 為準：**push 不等於工作區乾淨**

---

## Output Today（今日產出）
- Repo 結構已建立：`week01/day01/{notes,checklist,reflection}.md` + `lab/`
- 已完成至少 1 次 commit 並 push
