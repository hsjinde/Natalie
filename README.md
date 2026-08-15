# 2026 七夕限定任務

一個純靜態的單頁網站（HTML / CSS / JavaScript，無需建置流程）。

## 目錄結構

```
index.html      入口頁面
css/style.css   樣式
js/content.js   文案、照片清單、Spotify 曲目等內容設定
js/main.js      動畫與互動邏輯
images/         照片與背景圖
```

## 在本機預覽

因為頁面會載入 `js/` 與 `images/`，請用簡易伺服器開啟，不要直接雙擊 `index.html`：

```bash
python3 -m http.server 8000
```

然後開啟 http://localhost:8000

## 部署到 GitHub Pages

網站檔案放在儲存庫根目錄，目前已設定為**從分支部署**：

Settings → Pages → Build and deployment → Source 為 **Deploy from a branch**，
Branch 為 **main** 與 **/ (root)**。

只要有東西推送到 `main`，GitHub 就會自動重新發佈，不需要額外的 workflow。

網址：https://hsjinde.github.io/Natalie/

> `.nojekyll` 用來關閉 Jekyll 處理，確保所有靜態檔案原封不動地被提供。

## 修改內容

大部分文字、照片說明、測驗題目與約會選項都集中在 `js/content.js`，直接編輯該檔即可。
替換照片時，把新圖片放進 `images/` 並沿用相同檔名，就不用改程式碼。
