> 本文件為 Master Context，彙整目前為止與 Claude 的所有互動內容，供任何新的 AI 助理（ChatGPT／Claude 等）快速理解使用者背景。非依對話時間排序，而是依主題分類整理。
> 最後更新：2026-08-01

## User Profile


## Current Projects

1. **Statics 筆記整理（Vector Mechanics for Engineers）**
   - Vault 路徑：`建築結構系統/Mechanics/Statics/Vector Mechanics for Engineer/`
   - 已完成 Ch.0–Ch.10 全部章節筆記（Ch.8 Friction、Ch.9 Moment of Inertia、Ch.10 Method of Virtual Work 為新建立，Ch.6、Ch.7 為擴充／重寫），內容依據使用者上傳的手寫 PDF 筆記，比照既有 Ch.1–7 的寫作風格延伸完成。
   - 目前正在進行 **LaTeX 語法修正**，確保公式能在 GitHub 上正確渲染：
     - 規則 1：`$...$` 內側不留空格（已全面符合）。
     - 規則 2：長公式／多步驟推導（尤其含 `\begin{aligned}`、`\begin{vmatrix}`）改為獨立 `$$ ... $$` 區塊，前後留空行（已完成 Ch.3、Ch.4、Ch.9 共 19 處轉換並驗證無殘留）。

2. **建築法規（Building Regulations）考題整理**
   - 使用 Obsidian **Spaced Repetition** 外掛（st3v3nmw 版本）將題目轉換為 flashcard 格式。
   - 已完成「110_law 1」資料夾 Q1–Q80 全部轉為 flashcard，並依 Q1–44 既有規則為 Q45–80 補上主題 tag。
   - 已從上傳的「111180_1801.pdf」考卷萃取 Q1–Q80，建立「111」年度題庫資料夾。
   - 已修正筆記中 wikilink 顯示為完整路徑的問題，統一縮短為檔名。

## Long-term Goals

- 建立一套完整、可長期維護、可跨平台正確渲染（Obsidian + GitHub）的個人技術筆記庫，涵蓋結構力學與建築法規等考試／專業科目。
- 用 Spaced Repetition 系統將考古題轉換為長期記憶工具，準備應考。
- 將筆記同步備份至 GitHub，作為版本控制與雲端保存。

## Frequently Used Software

- **Obsidian**（含 Spaced Repetition 外掛）— 主要筆記平台
- **GitHub** — vault 備份／版本控制（曾用 PAT token 進行 push，需要 "Contents: Read and write" 權限）
- **Claude（Cowork 模式）** — 筆記生成、OCR 轉錄、格式轉換、批次腳本處理

## Working Style

- 習慣提供原始素材（手寫 PDF、截圖）讓 AI 參考既有風格延伸撰寫，而非從零生成。
- 重視「對照原文」而非自由發揮 — 明確要求筆記需對照書寫內容整理，不可捏造缺漏內容（例如缺少題目時要求標註「缺題目內容」而非亂補）。
- 疊代式回饋：先看實際渲染結果（如外掛設定截圖）再修正格式，不接受單純假設外掛預設值。
- 要求 AI 在給建議前，先查證官方文件（例如曾明確說「請你先讀一遍 spaced repetition 的排版格式再給我建議」）。
- 傾向一次把規則講清楚（如「以舊的 tag 優先，除非有新的再生成新的」），之後放手讓 AI 批次執行，不需逐一確認。
- 不希望 AI 主動處理未被要求的範圍（例如未要求修正的資料缺漏，會被記錄但不擅自處理）。

## Writing Style

- 筆記格式：英文為主、中文加註，outline／條列式（`##`／`-` 階層結構），非長篇散文。
- 大量使用 `==highlight==` 標記重點字詞。
- 使用 `[[wikilink]]` 做章節互連，圖片以 `![[image.png|寬度]]` 內嵌於 `Image` 子資料夾。
- 公式使用 LaTeX（`$...$` 行內、`$$...$$` 區塊），需符合 GitHub 相容語法。
- Flashcard 格式偏好簡潔換行（每行結尾加單一 `<br>`，非頭尾都加、非雙倍空行）。

## Technical Knowledge

- 熟悉 Markdown、LaTeX 數學語法、Obsidian wikilink／embed／YAML frontmatter。
- 具備基礎 git 操作知識（clone、push、remote set-url），但對 GitHub PAT 權限範圍等細節不算精熟，需要 AI 說明權限落差原因。
- 理解 Obsidian 與 GitHub 在 Markdown／LaTeX 渲染上的差異，並主動要求排查、修正相容性問題。
- 靜力學（Statics）與建築法規具一定專業基礎，能指出筆記內容錯誤或不精確之處。

## Preferred Response Style

- **極度簡潔直接**，避免不必要的說明與贅字（使用者已於系統偏好設定中明確聲明）。
- 減少不必要的條列與標題格式，除非內容本身確實需要結構化呈現。
- 傾向讓 AI 直接動手做，而非反覆詢問確認；但在真正模糊、需要抉擇時，願意配合澄清提問。
- 回覆完成後不需要冗長的逐步流程說明，簡短交代結果即可。

## Frequently Asked Topics

- Vector Mechanics for Engineers／Statics 各章節（向量運算、力矩、平衡、桁架與構架、樑與纜索內力、摩擦力、慣性矩、虛功法）
- 建築法規考古題（110、111 年度）整理、標籤分類、flashcard 轉換
- Obsidian 外掛設定（尤其 Spaced Repetition 的多行卡片分隔字元、結尾標記）
- Markdown／LaTeX 在 Obsidian 與 GitHub 間的語法相容性問題
- PDF 資料萃取（手寫筆記轉文字、考卷題目切分、含特殊編碼字元的 PDF 解析）

## Permanent Preferences

- 回覆務必簡潔直接，非必要不長篇解釋。
- LaTeX 規則：`$...$` 內側不得有空格；較長或多步驟公式一律改寫成獨立 `$$ ... $$` 區塊，前後留空行。
- Spaced Repetition 卡片格式：多行分隔字元使用 `ANS`（依使用者實際外掛設定，非預設 `?`），結尾標記使用 `+++`，換行只用單一 `<br>` 置於行尾。
- Wikilink 一律使用短檔名，不使用完整巢狀路徑。
- 未經明確要求，不主動修改或補全範圍外的內容（發現問題可提出，但不擅自處理）。
- 缺漏資料需誠實標註（如「缺題目內容」），不得捏造內容。

## Prompt Templates

以下為使用者慣用的請求句型，供未來對話快速套用：

- **筆記延伸生成**：
  「請幫我參考這份文件下的資料夾「[路徑]」的編寫模式。ch.X - Y。PDF 是我手寫的筆記，請對照我書寫的內容整理第 X 章開始以後的筆記。文字使用英文為主後面標註中文。」

- **語法／格式稽核**：
  「請幫我檢查第 X 章到第 Y 章，然後檢查[規則 A]與[規則 B]的關係，因為語法不精確導致 [平台] 沒辦法正確顯示內容。1. [規則 A細節] 2. [規則 B 細節]」

- **Flashcard／標籤批次轉換**：
  「幫我把 Q1–Q80 都做一樣的事」／「請試著分析 Q1 到 Q44 下 tag 的方式，然後幫 Q45 到 Q80 起 tag，要跟隨舊規則，以舊的 tag 優先，除非有新的再生成新的 tag。」

- **Wikilink 精簡化**：
  「請幫我把這個資料夾的連結都只留最後一個名字就好，不用完整的資料夾名字。」

## Things to Avoid

- 不要在未查證外掛／平台實際規格前，憑假設給格式建議（曾發生因假設 Spaced Repetition 預設分隔字元錯誤，導致卡片辨識失敗）。
- 不要過度加空白／換行（如 `<br><br>` 造成視覺間距過大）。
- 不要在資料缺漏時自行捏造內容，應如實標註缺漏並告知使用者。
- 不要擴大 wikilink 為完整巢狀路徑，應維持短檔名格式。
- 不要在未被要求的情況下，主動處理其他已發現但未被指派的問題（除非使用者之後主動詢問）。
- 驗證 GitHub 相關操作（如 token 有效性）時，需注意公開 repo 允許匿名讀取可能造成的「假陽性」驗證結果，勿因此誤判權限已足夠可寫入。
