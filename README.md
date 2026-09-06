# StreamPulse Live Standalone

獨立的直播房、聊天室與創作者互動平台，可部署為網站並安裝為 PWA App。

## 直接使用

將 `dist` 資料夾部署至任何 HTTPS 靜態網站服務。使用者開啟網站後，可從頁面上的「安裝 App」或瀏覽器選單安裝。

## Google 登入

在 `dist/viewer-config.js` 的 `clientId` 填入 Google OAuth Web Client ID，並將正式網站網域加入 Google Cloud Console 的 Authorized JavaScript origins。

未設定 Google Client ID 時，本機 Email 註冊與登入仍可直接使用；帳號及資料只保存在目前裝置。

## 直播

房主可輸入 HTTPS MP4/WebM 或 HLS `.m3u8` 播放網址。OBS Stream Key 產生器需要另外部署 Google Cloud Live Stream 或 Cloudflare Stream API 後端，再於主播控制台填入 API URL。

## 注意

Points 購買、訂閱與贊助為測試模擬，不會真實扣款。若要正式營運，請連接安全的後端、資料庫、付款驗證與內容管理服務。
