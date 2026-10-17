# Share MusicBox 網站

Share MusicBox（iPhone / iPad 家庭音樂盒）的產品介紹網站，包含操作示範影片、功能說明與下載 QR Code。

網站網址：https://squall.github.io/share-musicbox/

## 上架後設定 App Store 連結

打開 `index.html`，找到最上方這一行，填入 App Store 連結：

```js
const APP_STORE_URL = "";
```

例如：

```js
const APP_STORE_URL = "https://apps.apple.com/tw/app/id1234567890";
```

存檔並推上 GitHub 後，網頁會自動：

- 在兩個 QR Code 位置產生下載 QR Code
- 啟用所有「App Store 下載」與「免費下載」按鈕

沒有填連結時，QR Code 位置會顯示「QR Code 即將提供」，下載按鈕為停用狀態。

## 檔案結構

```
index.html                 網頁（樣式與程式都在這個檔案裡）
assets/video/demo.mp4      App 操作示範影片
assets/video/demo-poster.jpg
assets/img/*.webp          App 截圖、電腦端上傳頁截圖、App 圖示
favicon.png / apple-touch-icon.png
```

示範影片與截圖使用 App 的示範模式錄製，專輯、歌名與歌詞皆為原創示範內容。
