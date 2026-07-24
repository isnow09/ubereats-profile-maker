# 外送員簡介產生器

一個純前端（單一 HTML 檔）的趣味產生器：讓任何人做出一張仿外送 App 風格的「外送員簡介」圖片並下載／分享。

## 檔案

- `index.html` — 正式版（部署時用這支，GitHub Pages / Cloudflare Pages 預設會讀 `index.html`）
- `ubereats-profile-maker-v8.html` — 與 `index.html` 內容相同的備份／原始檔名

## 功能

- 範本一鍵套用、頭像上傳＋拖曳縮放
- 狀態列可自訂：時間、訊號文字、訊號強度（4/3/2/1 格，彈窗選）、電量數字、電量圖示（滿電／高／中／少電／缺電／充電中，彈窗選）
- 稱號徽章、原因區塊（底色／文字色可調）、通曉語言、顧客好評（Twemoji 開源圖示）
- 一鍵輸出 PNG，檔名為 `[名字]外送員簡介_YYYYMMDDhhmmss.png`
- 輸出圖片底部含系統推廣區塊與網址 QR（只出現在輸出圖，不在網頁預覽）

## 部署後要做一件事

發佈到網路後，打開 `index.html`，找到這一行，把網址換成你的正式網址（QR 會自動指向新網址）：

```js
const SITE_URL = 'https://your-generator-url.example';   // TODO: 換成正式網址
```

## 授權說明

圖示採用 Twitter Twemoji（CC-BY 4.0）。頁面標示為「創意模擬，非官方頁面」。
