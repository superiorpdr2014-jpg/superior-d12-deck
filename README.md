# D12 招募簡報（線上版）

凹痕職人初階養成班第十二堂給學員看的「卓越的下一步」，27 頁，網頁播放。

**線上**：<https://superiorpdr2014-jpg.github.io/superior-d12-deck/>
（`<meta name="robots" content="noindex, nofollow">`，不會被搜尋引擎收錄 —— 跟 `superior-echo-deck`、`superior-brandbook` 同一個做法。）

## 這個 repo 只是「網站」，不是來源

| | 位置 |
|---|---|
| 來源程式 | `Myke_Agent\教育部\小班制\D12招募簡報\build_recruit.py` |
| 系統動畫影片 | `Myke_Agent\教育部\小班制\D12招募簡報\DENTFIXO影片\`（做法見該資料夾 README）|

⚠️ **不要直接改這裡的 `index.html`** —— 下次重跑 `build_recruit.py` 會整份蓋掉。
改內容一律改 `build_recruit.py` 的 `S`，重跑之後再把產出的 HTML 複製成這裡的 `index.html`。

## 怎麼更新上線

```bash
PYTHONUTF8=1 python -I "教育部/小班制/D12招募簡報/build_recruit.py"
```

然後把 `D12招募簡報_卓越的下一步.html` 複製成本 repo 的 `index.html`，
`images/`、`media/` 有變動也一起複製，commit → push main，GitHub Pages 一兩分鐘後生效。

## 播放方式

- `←` `→` 翻頁，`F` 全螢幕，畫面左右兩側也可以點
- 第 16 頁是 **ECHO × MOC × DENT FIXO 系統動畫**：翻到就自動播（靜音、無聲軌），
  點影片暫停／繼續，右下角可切「完整版 2:27」
- 網址加 `?still=1` 會關掉所有進場動畫（截圖、匯 PDF 用）

## 檔案

| | |
|---|---|
| `index.html` | 簡報本體（含播放器、CSS、JS）|
| `images/` | 照片素材 |
| `media/dentfixo-74s.mp4` | 系統動畫 社群短版 74 秒（簡報內播這支）|
| `media/dentfixo-full.mp4` | 系統動畫 完整版 2:27（右下角按鈕切換）|
| `media/dentfixo-poster.jpg` | 影片封面（未播放時、列印時顯示）|
