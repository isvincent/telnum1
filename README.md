# 🌸 楊梅高中分機覽表 (Yangmei High School Phone Directory)

> 專為手機直式瀏覽打造的校園語音電話分機互動資訊網，具備即時檢索、一鍵直撥、語音朗讀與電話撥號音效。

[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-brightgreen?logo=github)](https://pages.github.com/)
[![Pure Frontend](https://img.shields.io/badge/Stack-Vanilla%20HTML%2FCSS%2FJS-blue?logo=javascript)](https://developer.mozilla.org/zh-TW/)
[![Responsive](https://img.shields.io/badge/Design-Mobile%20First%20Vertical-orange)](https://developer.mozilla.org/zh-TW/docs/Learn/CSS/CSS_layout/Responsive_Design)
[![Language](https://img.shields.io/badge/%E8%AA%9E%E8%A8%80-%E7%B9%81%E9%AB%94%E4%B8%AD%E6%96%87-rose)](#)

---

## 📖 專案簡介

本專案根據**桃園市立楊梅高級中學語音電話分機一覽表**官方資料製作，將原本複雜的紙本／PDF 表格轉化為現代化、色彩明亮且高度互動的直式手機專用網頁。無論是校內師生、家長或訪客，皆能透過智慧型手機秒速查找處室分機並一鍵快速撥號。

---

## ✨ 核心特色

### 📱 1. 手機專用直式版面 (Mobile-First)
- **旗艦手機直立體驗**：專為手機單手操作優化，支援 iOS / Android 全螢幕無縫瀏覽。
- **電腦端手機模擬外觀**：在桌機大螢幕開啟時，自動以高質感擬真智慧型手機外框呈現。
- **底部觸控導覽列**：固定式底部選單，單手即可迅速在「總覽」、「我的常用」、「檢索」、「撥號盤」之間切換。

### 🔍 2. 智慧檢索與多維分類
- **即時搜尋**：支援分機號碼（如 `1201`）、姓名（如 `鍾校長`、`邱組長`）、處室組別或建築地點，輸入即時高亮標註搜尋結果。
- **多維標籤滑動瀏覽**：提供「全部」、「我的常用」、「🏛️ 行政處室」、「👨‍🏫 教學導師」、「🔬 專科實驗」、「🏢 大樓專區」、「🏪 校園設施」等分類一鍵切換。
- **一鍵展開／摺疊**：支援一鍵展開或摺疊全部處室，閱讀更俐落。

### 📞 3. 便捷通訊與電話撥號盤
- **一鍵直撥**：點擊分機號碼自動調用手機撥號器，並透過延時轉分機協定自動帶入號碼（`tel:034789618,分機`）。
- **一鍵號碼複製**：貼心複製按鈕，點擊立即複製並跳出懸浮提示（Toast）。
- **模擬電話撥號盤 (DTMF 雙音)**：具備真實電話機鍵盤互動介面，按壓數字鍵即可發出標準電話雙音多頻（DTMF）音調。

### 🔊 4. 豐富互動與聽覺反饋
- **純前端 Web Audio API 音效引擎**：無須外部音檔，輕巧順暢。提供輕觸點選音、收藏星號音、複製成功鈴聲與 DTMF 電話撥號音，可隨時一鍵靜音／開啟。
- **語音朗讀分機 (Web Speech API)**：點擊 📢 廣播按鈕，手機即會以親切中文自動朗讀：「教務處 李主任，分機 1201」。

### 🌸 5. 明亮豐富的校園視覺
- **梅花飄落動態背景**：首頁頂部以 HTML5 Canvas 繪製輕柔優美的校花梅花飄落微動態。
- **處室專屬色彩識別**：行政處室（藍/綠/紅/橘）、導師室（靛藍/紫）、實驗室（青藍）等 19 個空間均有專屬明亮漸層配色與精緻圖示。

### 🔤 6. 閱讀友好與大字體設計
- **特大號分機號碼**：分機數字採用 20px~30px 特大號粗體膠囊按鈕，醒目易按。
- **三段字級切換**：右上角提供「🔤 字級切換」按鈕，可一鍵切換「標準 / 大字體 / 特大字體」，兼顧所有年齡層閱讀體驗。

### ⭐ 7. 個人常用分機收藏
- 點選任一分機旁的 ★ 星號，即可儲存至「我的常用」（使用瀏覽器 LocalStorage 儲存），下次開啟網頁秒查最常聯絡處室！

---

## 🚀 部署至 GitHub Pages 教學

本專案為零依賴的純前端架構（Pure HTML/CSS/JavaScript），無須安裝 Node.js 或建立後端，直接利用 GitHub Pages 即可永久免費上線！

### 步驟 1：建立 GitHub 儲存庫並推動程式碼
```bash
# 初始化 Git 儲存庫
git init

# 加入所有檔案
git add .

# 建立初次提交
git commit -m "feat: 建立楊梅高中分機覽表互動網頁"

# 設定分支名稱為 main
git branch -M main

# 關聯至您的 GitHub 遠端儲存庫 (請替換為您的 repo 網址)
git remote add origin https://github.com/<您的使用者名稱>/<儲存庫名稱>.git

# 推送至 GitHub
git push -u origin main
```

### 步驟 2：開啟 GitHub Pages 免費託管
1. 開啟 GitHub 儲存庫頁面，點選上方的 **Settings**（設定）。
2. 在左側選單中找到 **Pages**。
3. 在 **Build and deployment** > **Source** 選擇 `Deploy from a branch`。
4. **Branch** 選擇 `main` 分支，資料夾選擇 `/ (root)`，點選 **Save**。
5. 靜候約 1~2 分鐘，頁面上方即會出現您的專屬網址：  
   `https://<您的使用者名稱>.github.io/<儲存庫名稱>/`

---

## 📁 專案檔案架構

```text
├── index.html            # 互動資訊網主程式 (包含完整 UI、音效、語音、搜尋與動畫)
├── directory_data.json   # 完整結構化分機資料庫 (JSON 格式)
└── README.md             # 專案說明文件
```

---

## 🛠️ 使用技術

- **語言與標記**：HTML5, CSS3, Modern JavaScript (ES6+)
- **音訊與合成**：Web Audio API (原生合成音效、DTMF 雙音多頻)、Web Speech API (語音朗讀)
- **字型資源**：Google Fonts ([Noto Sans TC](https://fonts.google.com/specimen/Noto+Sans+TC), [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk))
- **視覺動態**：HTML5 Canvas 梅花粒子動畫、CSS3 3D Transform & Cubic-Bezier 微動畫

---

## 📋 資料版本與宣告

- **資料來源**：桃園市立楊梅高級中學總務處
- **版本資訊**：115/09/07 版本
- **總機號碼**：03-4789618（代表號）、4780449（二線）、4780740（三線）
- **聲明**：本專案僅供校園資訊查詢與學術技術交流使用，所有分機號碼均以楊梅高中校方最新公告為準。
