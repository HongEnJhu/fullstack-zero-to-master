# Week 01 / Day 01 — Reflection

## What I did（今天完成了什麼）
- 建立學習主倉庫 repo 與固定資料夾結構
- 在 `lab/` 用終端機練習檔案操作（create/rename/copy/delete）
- 完成至少一次 commit 並 push

---

## What blocked me（今天最卡的點）
- 我一開始以為 push 之後就「沒有狀態」了，但其實 push 只是同步遠端；本地是否乾淨仍要看 `git status`。

---

## How I fixed it（我怎麼解決）
- 回到 repo 根目錄跑 `git status` 確認 modified 檔案
- 使用 `git add` → `git commit` → `git push` 完成追蹤與同步

---

## Key takeaway（今天最重要的學到）
- Terminal：操作前先確認「我在哪（pwd）」與「目標是誰（路徑/檔名）」
- Git：一切以 `git status` 為準；**push ≠ 工作區乾淨**

---

## Next time（明天我會怎麼做得更好）
- 做刪/移/改名之前固定跑一次 `pwd` + `ls`
- 交作業紀錄只用可重現的「相對路徑 + 實際檔名」
- 任何「我覺得應該好了」的時候先跑 `git status` 再說