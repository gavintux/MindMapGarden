# 🎨 Mindomo 心智圖展示平台
把你的 Mindomo 心智圖變成超酷的個人網站！✨
[![License: MIT](https://img.shields.io/badge/License-MIT-Hub Pages](https://img.shields.io/badge/部署-GitHub%20Pages-bright是一個神奇的網頁工具，可以讓你把在 Mindomo 上畫的心智圖，變成一個漂亮的網站展示出來！只要加上 `#share` 標籤，你的作品就能讓全世界的人看到囉！
[👉 看看範例網站](https://gavintux.github.io/yi/)

## ✨ 功能特色
- 🎯 自動顯示有 `#share` 標籤的心智圖
- 🔐 管理員模式可以看到所有心智圖
- 📱 手機、平板、電腦都能用
- 🎨 介面簡潔又好看
- 🚀 完全免費部署到網路上

## 🎬 開始之前

### 你需要準備：

1. 📝 一個 Mindomo 帳號（用來畫心智圖）
2. 💻 這個 HTML 檔案
3. 🌐 一點點時間來設定

## ⚙️ 設定步驟

### 第一步：取得 Mindomo API 金鑰 🔑

1. 打開這個教學網頁：[如何取得 Mindomo API](https://2blog.ilc.edu.tw/linkc/2025/11/21/mindomo-%e5%a6%82%e4%bd%95%e5%8f%96api/)
2. 跟著步驟操作，複製你的 API 金鑰

### 第二步：修改檔案設定 ✏️

用記事本或任何文字編輯器打開 `mindomo_view.html`，找到下面這些地方來修改：

#### 1️⃣ 修改傳送門網址

找到這一行（大約在第 XXX 行）：
```javascript
const portalUrl = "https://你的網址.com";
```
把網址改成：
- 你的個人首頁
- 學校網站
- 或任何你想連結的地方

#### 2️⃣ 修改 API 金鑰

找到這一行：
```javascript
const apiKey = "你的API金鑰";
```
把 `你的API金鑰` 換成剛才複製的 Mindomo API

#### 3️⃣ 修改管理員密碼 🔒

找到這一行：
```javascript
const adminPassword = "123456";
```
⚠️ **重要！** 請把 `123456` 改成只有你知道的密碼！

#### 4️⃣ 更換你的 Logo 圖片 🖼️

找到這一行：
```html
<img src="你的logo網址" alt="Logo">
```
把 `你的logo網址` 換成你的圖片網址（可以用 imgur、Google Drive 等）

## 🚀 發佈到網路上

### 使用 EZPage 超簡單部署工具

我們要用 [EZPage](https://gg90052.github.io/ezpage/) 這個超棒的工具！它可以幫你快速把網頁放到網路上。

***

### 🎈 情況 A：我還沒有 GitHub 帳號

#### Step 1：註冊 GitHub 帳號
1. 去 [GitHub](https://github.com) 網站
2. 點擊右上角的 **Sign up**（註冊）
3. 填寫你的 Email、密碼和使用者名稱
4. 完成信箱驗證

#### Step 2：第一次使用 EZPage
1. 打開 [EZPage 網站](https://gg90052.github.io/ezpage/)
2. 點擊 **連接 GitHub** 按鈕
3. 登入你的 GitHub 帳號
4. 允許 EZPage 存取你的 GitHub（點選「Authorize」授權）
5. 上傳你修改好的 `mindomo_view.html` 檔案
6. 取一個專案名稱（例如：`my-mindomo`）
7. 點擊 **部署** 按鈕
8. 等待 1-2 分鐘，完成！🎉

你的網站網址會是：`https://你的GitHub帳號.github.io/專案名稱/`

***

### 🎈 情況 B：我已經有 GitHub 帳號了

#### 第一次使用 EZPage 📗
1. 打開 [EZPage 網站](https://gg90052.github.io/ezpage/)
2. 點擊 **連接 GitHub** 按鈕
3. 登入你的 GitHub 帳號（如果沒登入的話）
4. 允許 EZPage 存取（點選「Authorize」授權）
5. 上傳你的 `mindomo_view.html`
6. 填寫專案名稱
7. 點擊 **部署**
8. 完成！🎊

#### 已經用過 EZPage 了 📘
1. 打開 [EZPage 網站](https://gg90052.github.io/ezpage/)
2. 選擇 **更新現有專案** 或 **建立新專案**
3. 如果是更新：選擇要更新的專案，上傳新檔案
4. 如果是新建：跟上面步驟一樣
5. 點擊 **部署**
6. 完成！🎯

***

## 🏷️ 重要：設定心智圖標籤

### 為什麼我的網站是空白的？ 🤔

如果你發佈完成後，網站上沒有顯示任何心智圖，那是因為你還沒有加上 `#share` 標籤！

### 如何添加標籤：

1. 打開 Mindomo，選擇你想分享的心智圖
2. 在心智圖設定中找到「標籤」功能
3. 加上 `#share` 標籤
4. 儲存

📚 詳細教學看這裡：[如何增加 Mindomo 標籤](https://2blog.ilc.edu.tw/linkc/2025/11/21/mindomo-%e5%a6%82%e4%bd%95%e5%a2%9e%e5%8a%a0%e6%a8%99%e7%b1%a4/)

## 🎮 使用方式

### 一般模式 👀
- 打開網站，就能看到所有有 `#share` 標籤的心智圖
- 點擊心智圖可以放大查看

### 管理員模式 👨‍💼
1. 點擊右上角的 **管理員登入**
2. 輸入你設定的密碼
3. 現在可以看到所有心智圖（包括沒有 `#share` 標籤的）

## 🎁 額外功能

- 點擊 **🏠 傳送門** 可以回到你設定的首頁
- 心智圖會自動排列，不用手動調整
- 支援搜尋功能（如果心智圖很多的話）

## 🐛 遇到問題？

### 問題 1：網站打不開
- 檢查 GitHub Pages 是否已啟用
- 等待 5-10 分鐘讓設定生效

### 問題 2：API 無法連接
- 確認 API 金鑰是否正確
- 檢查 Mindomo 帳號是否正常

### 問題 3：心智圖沒顯示
- 確認心智圖有加上 `#share` 標籤
- 重新整理網頁試試看

## 📜 授權

本專案採用 **MIT 授權條款**

這表示你可以：
- ✅ 自由使用
- ✅ 修改內容
- ✅ 分享給朋友
- ✅ 用在學校專案

只要保留原作者的版權聲明就可以了！

## 💖 支持我們

如果您覺得這個工具對您有幫助，歡迎小額贊助，支持未來的開發！

- **台灣使用者 (Taiwan)**: [點此使用綠界贊助 (支援信用卡/ATM)](https://p.ecpay.com.tw/您的綠界連結代碼)

## 🌈 給爸爸媽媽和老師的話

這個專案適合：
- 學習分享自己的作品
- 了解網頁運作的基礎
- 練習跟著步驟完成任務
- 培養資訊安全意識（密碼管理）

建議家長或老師可以陪同孩子一起操作前幾次，確保他們理解每個步驟的意義。

## 📞 聯絡資訊

- 作者網站：[https://gavintux.github.io/yi/](https://gavintux.github.io/yi/)
- 有問題嗎？歡迎在 GitHub Issues 發問！

***

⭐ 如果你喜歡這個專案，別忘了給我們一顆星星！

**祝你使用愉快！Have fun! 🎉**

***

