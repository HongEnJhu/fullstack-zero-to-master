# Week 01 / Day 02 — Checklist

## Acceptance（驗收標準）

- [ ] `week01/day02/` 結構完整（3 個 md + `lab/`）
- [ ] `sample.txt` 行數 >= 15（以 `wc` 驗證）
- [ ] `results.txt` 包含以下區塊，且每段都能對應一個指令輸出：
  - [ ] `wc sample.txt`
  - [ ] `head sample.txt`
  - [ ] `tail sample.txt`
  - [ ] `grep "error" sample.txt`（若要同時抓 `ERROR`，改用 `grep -i`）
  - [ ] `grep -n "warn" sample.txt`
  - [ ] `cat sample.txt | grep "info"`
- [ ] 至少 1 次 commit + push（Day02）

---

## Work Log（我做了什麼）

- [x] 建立 `week01/day02/` 與必交檔案
- [x] 在 `lab/` 產生 `sample.txt`
- [x] 用重導向 `>>` 產生 `results.txt`
- [x] 用 `grep` 與 pipe `|` 篩選內容
- [ ] Git：`add → commit → push`

---

## Issues / Blockers（卡點）

- [ ] 卡點：
- [ ] 我怎麼定位（我看了什麼輸出/錯誤訊息）：
- [ ] 我下次避免方式（具體行動）：
