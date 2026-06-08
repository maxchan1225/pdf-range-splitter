# PDF Range Splitter

把 PDF 拖進頁面，輸入多組「起始頁」與「結束頁」，即可一次切出多個新的 PDF。所有處理都在瀏覽器本機完成，不會上傳到伺服器。

## 功能

- 拖放或選取 PDF，並在左側預覽。
- 多組頁碼範圍分割，可同時輸出多份 PDF。
- 單一結果直接下載 PDF，多個結果自動打包 ZIP。
- 一頁一檔：把整份 PDF 拆成單頁 ZIP。
- 奇偶頁抽取：只保留奇數頁或偶數頁。
- 刪除指定頁：支援 `2-4, 7` 這類頁碼格式。
- 旋轉指定頁：支援右轉 90 度、轉 180 度、左轉 90 度。
- 合併多個 PDF，依選取順序輸出成 `merged.pdf`。
- 加入文字：點選 PDF 頁面定位後，可寫入新文字並下載。
- 修改文字：以白底遮蓋舊字，再寫入修正後文字；適合表格、講義、申請表等常見修正。
- 文字功能支援中文，輸出時會嵌入 Noto Sans CJK TC 字型。
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
