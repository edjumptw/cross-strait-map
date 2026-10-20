# 兩岸市場進入地圖｜陳執董 Jump

> 給下一位接手的 AI 或協作者：先讀這份，就知道這個網站做到哪一步、哪些內容是誰決定的。
> 最後更新：2026-10-20｜Claude（Anthropic）

## 這是什麼

一支單頁靜態網站（純 HTML/CSS/JS，無框架、無外部圖片，插畫全是手刻 SVG），風格仿照
[fatnerdstock.com/alex-hormozi-map](https://fatnerdstock.com/alex-hormozi-map/) 的
neo-brutalism 風格（粗黑框、硬陰影、糖果色、Rammetto One + Noto Sans TC）。

- **上線網址**：https://edjumptw.github.io/cross-strait-map/
- **Repo**：https://github.com/edjumptw/cross-strait-map
- **部署**：GitHub Pages，`main` 分支 `/` 根目錄，push 後自動建置
- **本機測試**：`.claude/launch.json` 設定了 `python3 -m http.server 4173`，用 Claude Code 的 preview 工具開

## 內容是什麼

把陳執董（陳建蒲，BNC 建橋雲智執行董事）的兩岸市場進入方法整理成一套「8 零件診斷地圖」，
模式是 Hormozi 那頁的「症狀 → 找零件 → 看卡片 → 下一步」：

1. **Hero**：8 宮格總覽 + 症狀診斷入口
2. **Diagnose**（`#diagnose`）：13 個常見症狀 chip，點一個 → 跳出對應零件的診斷結果
3. **The Map**（`#cards`）：8 張零件卡（定位／信任狀／引薦網／在地夥伴／試點驗證／基礎設施／現金流／複製擴張），每張有一句話核心、重點、關鍵數字、地雷、「遇到這些情況怎麼用」
4. **Rules**（`#rules`）：10 條鐵律 + 數字速查
5. **OPC**（`#opc`）：台灣 vs 大陸一人公司比較 + 成都／廈門／武漢三城落地資訊
6. **Podcast**（`#podcast` 位置在頁面第 5 段，無獨立 id）：136 集「陳執董的商業洞察」的素材來源說明 + 3 集真正談兩岸/台青賽道的集數連結（EP113/116/117）
7. **Community**（LINE 社群 CTA）
8. **Who's Jump**（`#about`）：真實經歷卡片 + 連回 `edjumptw.github.io/me`

## 重要：哪些內容是「真的」，哪些是我編的

- **8 個零件的框架文字（標題/重點/地雷/症狀）是 Claude 根據陳執董的背景資料推演寫的草稿**，
  不是他原本就有的方法論逐字稿。他在對話中明確說「我還沒有成形的方法論，你幫我完成它」。
  **這塊內容使用者還沒有逐條確認過**，之後有調整都正常。
- **OPC 法規內容有做過 WebSearch 查證**（台灣公司法最低資本額廢除、大陸一人公司舉證責任倒置等），
  但兩岸公司法規常變，頁面上已經加了免責聲明，正式使用前仍要請使用者的會計師/代辦覆核。
- **Podcast 區塊的 3 集連結是真實的 YouTube 連結**（從頻道實際撈的，不是編的）。136 集的其餘內容
  使用者確認「是在地台灣中小企業訪談，沒有真的帶去大陸」，所以頁面文案刻意沒有把那些來賓包裝成
  兩岸案例，只當作「方法論素材來源」的信任狀。
- **陳執董是誰」的經歷**來自他自己的 `edjumptw.github.io/me` 頁面，是真實資料。

## 變現相關（跟 BNC 建橋雲智專案共用同一個漏斗）

- 「症狀診斷」結果面板下面有一個金色「想要不只是自己摸索？」upsell 區塊，導去
  `https://lin.ee/8H1uS3c`（陳執董個人 LINE），文案是「了解 BNC 會員／創始元老方案」。
- 這個 LINE 連結跟 `~/Claude/建橋雲智/claude/Claude交接筆記.md` 裡記錄的 Podcast 報價方案、
  BNC 會員方案用的是**同一個入口**——這兩個專案雖然是分開做的，但導流終點是同一條漏斗。
  之後如果要調整 LINE 入口或報價，兩邊都要一起改，不然會對不上。
- 詳細的 BNC 會員定價（初階 NT$3,600 / 中級 NT$12,000）、Podcast 專訪報價
  （音訊 NT$19,800、影音 NT$39,800）都在 `~/Claude/建橋雲智/claude/可用/` 裡，這個網站
  目前**沒有**顯示任何具體價格，刻意讓使用者自己在 LINE 上報價。

## 跟 `edjumptw.github.io/me` 的關係

兩個站互相連結，各自負責不同功能，不是同一個東西：

- `/me`：正式個人形象頁（真人照片、履歷式），「核心內容」第一條已加連結指到這個地圖
- 這個地圖：單一主題的深度互動內容頁（卡通插畫、互動診斷），「陳執董是誰」區塊有連結指回 `/me`

使用者明確表示**不想把這個 neo-brutalism 風格直接套用去取代 `/me`**，兩者風格刻意不同，
因為 `/me` 要給人第一次認識他時的專業信任感，這個地圖是功能性的 lead magnet。

## 待辦／使用者還沒拍板的事

- 8 個零件框架的具體文字內容，使用者說「先這樣，我再慢慢改」——還沒逐條確認過
- 以下真實存在、但還沒放上 `/me` 或這個地圖的變現項目（使用者已確認是真的在跑）：
  - BNC 會員／創始元老招募（對應 Google Drive 裡的 `bnc-intent-2026` repo 與交接筆記）
  - 看房團／考察團（中山珠海）
  - 青年培訓考察計畫
  - AI 手機行銷／直播帶貨課程（KK 老師課程團隊合作）
- Podcast 區塊目前只有「延伸收聽」功能，**沒有**放上企業贊助/專訪報價的 CTA——
  `~/Claude/建橋雲智/claude/可用/02_Podcast廣告合作方案與專訪收費定價.md` 裡已經有現成對外版
  文案，是很自然的下一步，但使用者還沒有要求做這塊

## 技術細節速記

- 設計代幣（CSS 變數）：`--mint --gold --coral --teal --sky --navy --cream --rose --ink` 等，
  全部定義在 `:root`，不要在元件裡寫死色碼
- 卡片公式：`border:3px solid var(--ink)` + 圓角 + `box-shadow:Npx Npx 0 var(--ink)`（純色、零模糊）
- 字體：`Rammetto One`（展示字，只用在英文/數字）+ `Noto Sans TC`（中文內文，只載 500/700/900）
- 內容是資料驅動：`PARTS` / `SYMPTOMS` / `RULES` / `NUMS` 這幾個 JS 物件定義資料，
  `renderMap()` 統一渲染，要改內容改資料就好，不用動 HTML 樣板
- GitHub 帳號 `edjumptw` 已經透過 `gh auth login` 授權，`gh` CLI 裝在 `~/.local/bin/gh`
  （不是用 Homebrew 裝的，因為這台機器沒裝 Homebrew）
