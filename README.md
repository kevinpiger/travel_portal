# 旅行手帖入口

正式入口： https://kevinpiger.github.io/travel_portal/

GitHub Pages 從 main 分支的 /(root) 發布，HTTPS 已啟用。首頁以 Card＋原創 SVG 呈現旅行地點、日期與回憶意象；點選卡片開啟各自的行程。

網址規則：`https://kevinpiger.github.io/travel_portal/{yearmonth}/{location}/`

| 旅程 | 路徑 |
| --- | --- |
| 東京 2025/11/21–24 | `202511/tokyo/` |
| 北海道 2026/12/5–13 | `202612/hokkaido/` |

`yearmonth` 為旅程出發年月（六位數），`location` 使用小寫英文目的地。日期屬不同年份時，各自存放；不要覆寫其他行程。

北海道入口保留查詢參數與 hash，導向既有 https://kevinpiger.github.io/travel/2026_hokido/ 。原 travel repo、根頁轉址與北海道行程完全不變。

東京是原試算表「202511東京」的手工快照，未重新查核歷史航班／交通／營業資訊；修改試算表不會自動更新網站。網站以獨立相對路徑資源運作，清單儲存使用東京專屬 localStorage key。

GitHub Pages 設定：Deploy from a branch → main → /(root)。不需安裝或建置。新增旅程時建立 `{yearmonth}/{location}/index.html`，再於根 `index.html` 加入入口連結。不要把來源試算表、訂單與個人憑證放入公開網站。
