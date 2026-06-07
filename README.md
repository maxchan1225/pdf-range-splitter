# PDF Range Splitter

把 PDF 拖進頁面，輸入多組「起始頁」與「結束頁」，即可一次切出多個新的 PDF。

## 功能

- PDF 只在瀏覽器本機處理，不會上傳到伺服器。
- 支援拖放或選取 PDF。
- 可新增多組分割範圍。
- 單一結果會直接下載 PDF，多個結果會打包成 ZIP。
- 支援 Firebase Hosting 靜態部署。

## 線上網址

https://teacherstudy-ac70b-pdf-splitter.web.app

## 本機預覽

```powershell
npx.cmd -y serve public
```

## 部署

```powershell
npx.cmd -y firebase-tools@latest deploy --only hosting
```

若使用 GitHub Actions 自動部署，請在 GitHub repo secrets 加入
`FIREBASE_SERVICE_ACCOUNT_TEACHERSTUDY_AC70B`。
