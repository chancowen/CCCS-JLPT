# JLPT N5–N3 自學課程庫（GitHub Pages 版）

呢個 repo 係 JLPT N5–N3 每日自學課程嘅靜態網站，可直接用 **GitHub Pages** host，唔使任何後端。

## 目錄結構

```
index.html                  ← 課程庫入口（30 日課程表＋統計）
jlpt_style.css              ← 課程頁樣式
JLPT_課程庫/                ← 每日課程原始檔（.md ＋ .pdf）
課程頁/                     ← 課程嘅網頁版（喺瀏覽器直接閱讀）
```

## 部署到 GitHub Pages（三步搞掂）

### 方法一：用戶網站（建議，網址最短）

1. 喺 GitHub 開一個新 repo，**名一定要叫**：`<你的用戶名>.github.io`（例如 `janedoe.github.io`），public。
2. 將呢個資料夾嘅**所有內容**上傳到 repo 根目錄（可以用 `git push`，或者喺網頁按 "uploading an existing file" 直接拖入去）。
3. 等一兩分鐘，開 `https://<你的用戶名>.github.io/` 就得。

### 方法二：專案網站

1. 開一個任何名嘅 repo（例如 `jlpt-course`），上傳呢個資料夾嘅所有內容。
2. 去 repo **Settings → Pages**，Source 揀 **Deploy from a branch**，branch 揀 `main`、資料夾揀 `/(root)`，Save。
3. 網址係 `https://<你的用戶名>.github.io/<repo名>/`。

## 之後每日更新點做？

每日出新課後，只要將新嘅 `.md`／`.pdf` 放入 `JLPT_課程庫/`、新嘅課程頁 HTML 放入 `課程頁/`、更新 `index.html`，然後 commit＋push，GitHub Pages 會自動更新（通常 1–2 分鐘內生效）。

## 注意事項

- 檔案名有日文同中文，GitHub 支援 UTF-8 檔名冇問題；不過 GitHub Pages 伺服器係 **case-sensitive**（大細階敏感），上傳時保留原檔名就得。
- `.pdf` 連結喺瀏覽器會直接開啟預覽；`.md` 連結會顯示原始文字。
- 如果想 `.md` 都渲染成網頁，可以改用 `課程頁/` 入面嘅 `.html` 版本（index.html 已經有連結）。
