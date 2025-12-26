# Week 01 / Day 02 — Reflection

## What I did

- 用 `wc/head/tail` 驗證檔案內容與行數
- 用 `grep` 搜尋關鍵字，並用 `-n` 加行號方便定位
- 用 `>>` 把每段指令輸出追加到 `results.txt`，形成可驗收紀錄
- 用 pipe `|` 把 `cat` 的輸出交給 `grep` 篩選

---

## What I learned

- `>` 是覆寫、`>>` 是追加；要做「紀錄檔」通常用 `>>`
- `grep -n` 很像 debug 定位：直接給行號，後續查檔更快
- 若要同時抓 `error/ERROR`，需要 `grep -i`（大小寫不敏感）

---

## What to improve next time

- 每個輸出都加上區塊標題，讓結果檔像 log 一樣可讀
- 需要「不分大小寫搜尋」時，優先想到 `-i`
- 任何感覺「怪怪的」先回到 `wc/head/tail` 做快速 sanity check
