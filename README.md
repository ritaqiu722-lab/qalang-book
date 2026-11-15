# mnanak na qalang 互動繪本

可翻頁、有旁白與配樂的互動繪本網頁(純 HTML/CSS/JS,不需要建置)。

## 檔案結構

```
index.html        主頁面(所有功能都在這裡)
img/              p0~p19.jpg 為 20 頁插圖;left/right/read/spirit 為介面圖示
audio/            speech0~19 旁白、music0~19 每頁配樂、bgm.mp3 封面主題曲
.nojekyll         告訴 GitHub Pages 不要用 Jekyll 處理
```

## 操作

- 點封面「開始閱讀」(瀏覽器規定要有點擊才能播放聲音)
- 翻頁:左右箭頭、鍵盤 ← →、手機左右滑動
- 下方按鈕:旁白開關、配樂開關、自動翻頁(旁白播完自動換頁)、重聽本頁
- 網址 `#5` 可直接跳到第 5 頁

## 調整

`index.html` 的 `<script>` 開頭有設定區:

- `MUSIC_VOL` 每頁配樂音量、`VOICE_VOL` 旁白音量、`BGM_VOL` 主題曲音量
- `BGM_ONLY_ON_COVER` 設成 `false` 則主題曲全書低音量循環播放
