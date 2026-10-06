# My lab evidence / 我的實作紀錄

Use a group code, not real names or student IDs in shared files. / 共用檔只寫組別代碼，不寫姓名或學號。

- Group code / 組別：W05-IND
- Tool / 工具：ChatGPT / GitHub Web UI
- Route / 路線：individual 個人
- Tasks completed / 完成題目：A, B, D
- Material / 素材：NDHU classroom tasks 東華課堂版
- For original-pack work: task number, author/source link and version / 原版實作：N/A
- My role and what I checked / 我的角色與實際檢查：負責提示詞下達、檢查 AI 產出的程式碼與文件品質，並手動於 GitHub 網頁 UI 完成檔案建立、路徑校對與 Commit 提交。

## Scope and plan / 範圍與計畫

Allowed input and output folders / 可讀取與輸出的資料夾：
`practice/01-club-files/output/`, `practice/02-campus-picker/output/`, `practice/04-review/`, `evidence/`

What I asked for / 原始需求：
1. 整理社團檔案，剔除冗餘檔並產出總表 (Task A)。
2. 開發校園活動選擇器 HTML 介面，並新增搜尋過濾功能 (Task B)。
3. 撰寫審查退回說明文件 (Task D)。

What I checked before execution / 動手前我檢查了什麼：
1. 確認各 Task 的目標目錄與 `output/` 路徑規則。
2. 確認每一題要求的 Commit Message 規範。
3. 確認內容均使用虛構資料，無真實姓名與學號。

## Tests actually performed / 我真的做過的測試

| Test / 測試 | Expected / 預期 | Observed / 實際 | Evidence / 證據 |
|---|---|---|---|
| 1 (Task A) | 生成去重歸類的 `summary.md` 於 `01-club-files/output/` | 成功清理重複檔並完成四大類別歸檔 | Commit: `A: organize club files`[cite: 1, 2] |
| 2 (Task B) | 在 `02-campus-picker/output/index.html` 實現關鍵字過濾功能 | 頁面可同時透過分類按鈕與搜尋框篩選活動 | Commit: `B v2: add search bar`[cite: 3, 4] |

## One revision / 一次修改

Before / 原來的情況：
Task B v1 版僅支援「按鈕類別篩選」（全部、學術、社團）。

Request / 我提出的修改：
新增「即時關鍵字搜尋框」輸入介面，並改善卡片視覺樣式[cite: 3]。

After and retest / 修改後與重測結果：
Task B v2 能同時依據類別按鈕與文字輸入即時顯示符合條件的卡片，運作正常[cite: 3, 4]。

New requirement or defect? / 新需求還是原規格未做到？
新需求（功能的優化升級）[cite: 3]。

## One rejection / 一次退回

Which action I reject and why / 退回哪個動作、為什麼：
退回一份包含真實學生姓名與未放在 `output/` 目錄的提交案，因違反個資規範與資料夾路徑規格[cite: 1, 3]。

An acceptable alternative / 可以怎麼改：
將個資全面改為虛構範例，並將檔案移至正確的 `output/` 目錄後重新提交[cite: 1, 3]。

## Still unverified / 還沒驗證

What I cannot claim is complete / 哪些事不能說已完成：
由於學校電腦限制無法使用 Git CLI 與 Antigravity 本地環境，目前所有操作皆經由 GitHub 網頁端（Web Route）完成，未在本地終端機執行自動化測試腳本[cite: 1]。
