# Week 01 / Day 02 — File Viewing, Redirects, Pipes, Search

## Goals

- 用指令快速讀檔：`cat/less/head/tail/wc`
- 會用重導向把輸出寫進檔案：`>` 覆寫、`>>` 追加
- 會用 pipe `|` 串接指令
- 會用 `grep`（或 PowerShell `Select-String`）搜尋關鍵字

---

## Key Concepts

### File Viewing

- `cat <file>`：直接輸出整個檔案（小檔用）
- `less <file>`：分頁檢視（大檔/Log 必備）
  - 常用：`/keyword` 搜尋、`n` 下一個、`q` 離開
- `head <file>`：看前幾行（預設 10）
- `tail <file>`：看最後幾行（預設 10）
- `wc <file>`：統計行數/字數/bytes（用來驗證資料量是否符合預期）

---

### Redirects（重導向）

- `>`：把輸出**覆寫**到檔案（會清空原內容）
- `>>`：把輸出**追加**到檔案（保留原內容）

> 工程習慣：產出「可驗證結果檔」比手動複製貼上可靠。

---

### Pipe（管線）

- `A | B`：把 A 的輸出當成 B 的輸入
- 常見用法：把大量輸出丟給 `grep` 篩選

---

### Search（搜尋）

- `grep "keyword" <file>`：找包含 keyword 的行
- `grep -n "keyword" <file>`：加上行號，方便定位
- `grep -i "keyword" <file>`：忽略大小寫（若要同時抓 `error/ERROR` 要用它）

---

## Lab Output

- `week01/day02/lab/sample.txt`
  - 行數：>= 15（實際：21）
  - 內容包含：`error / warn / info`（含大小寫版本）
- `week01/day02/lab/results.txt`
  - 以區塊標題分段保存指令輸出（可追溯、可驗收）
