# 🌸 Manifest Lab — Vercel + PWA 部署指南

## 檔案結構

```
manifest-lab-pwa/
├── index.html          ← 主App
├── manifest.json       ← PWA設定
├── sw.js               ← Service Worker（離線支援）
├── vercel.json         ← Vercel設定
├── icon-generator.html ← 圖示生成器（本地開啟用）
└── icons/
    ├── icon-192.png    ← App圖示（需要自己生成）
    └── icon-512.png    ← App圖示（需要自己生成）
```

-----

## Step 1：生成 App 圖示

1. 在瀏覽器開啟 `icon-generator.html`
1. 點「下載 icon-192.png」和「下載 icon-512.png」
1. 把兩個檔案放入 `icons/` 資料夾

-----

## Step 2：上傳到 GitHub

1. 在 GitHub 建立新 repository（例如 `manifest-lab-app`）
1. 上傳整個 `manifest-lab-pwa/` 資料夾的所有檔案
1. 確認以下檔案都在根目錄：
- `index.html`
- `manifest.json`
- `sw.js`
- `vercel.json`
- `icons/icon-192.png`
- `icons/icon-512.png`

-----

## Step 3：部署到 Vercel

1. 去 [vercel.com](https://vercel.com) 用 GitHub 帳號登入
1. 點 `Add New → Project`
1. 選你剛才建立的 repository
1. Framework Preset 選 **Other**
1. 點 `Deploy`
1. 等約1分鐘，得到網址：`https://manifest-lab-xxx.vercel.app`

-----

## Step 4：自訂域名（可選）

如果你想要 `app.mymanifestlab.com` 之類的網址：

1. 在 Vercel 的 Project Settings → Domains
1. 加入你的域名
1. 按照指示在你的域名商設定 DNS

-----

## iPhone 加到主畫面（iOS）

1. 用 Safari 開啟你的 Vercel 網址
1. 點底部分享按鈕 `⬆`
1. 選「加入主畫面」
1. 命名「Manifest Lab」→ 點「新增」
1. 主畫面出現 🌸 圖示，點開就像真正的App！

-----

## Android 加到主畫面（Chrome）

App 會自動出現「安裝」橫幅，點「安裝」即可。
或者：Chrome 右上角 `⋮` → 「安裝應用程式」

-----

## Gumroad 版本

Gumroad 賣的就是這個完整的資料夾（打包成 zip）。
買家下載後，可以：

1. 直接用瀏覽器開啟 `index.html` 使用
1. 或者自己部署到 Vercel

在 Gumroad 產品描述中加入你的 Vercel 連結，
讓買家直接用，不需要自己部署。