# ALPINE RUSH

一款可直接在瀏覽器遊玩的無盡高山滑雪板跑酷遊戲。

## 開始遊玩

開啟 GitHub Pages 網址，點擊畫面或按下 `Space` 即可開始。

## 操作方式

- `A` / `D` 或方向鍵：刻滑轉向
- `W` / `Shift`：壓低身體、降低風阻
- `Space`：跳躍
- `Q` / `E`：空中旋轉
- `S`：空中抓板
- `R`：重新定位
- `F`：顯示 FPS

手機可使用畫面左右區域刻滑，並使用畫面上的 `JUMP` 與 `SPIN` 按鈕。

## 技術

遊戲邏輯與 shader 完整包含在單一 [`index.html`](./index.html) 中，Three.js 由 jsDelivr CDN 載入，不需要建置步驟。

雪場植被與岩石使用 KayKit Forest Nature Pack 的少量 CC0 glTF 資產，從同一個 GitHub Pages 網站載入；如果資產載入失敗，會自動使用程序生成模型。來源與授權紀錄見 [`ASSETS.md`](./ASSETS.md)。
