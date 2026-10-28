# 3D 紙飛機物理模擬實驗室

以單一 HTML 頁面製作的互動式 3D 紙飛機模擬器。可調整紙飛機型號、迴紋針配重、機翼設定、發射條件與環境，並查看飛行遙測資料。

## 功能

- 經典飛鏢、Suzanne、獵鷹及太空梭等紙飛機外型
- 迴紋針配重、升降尾舵、上反角、翼尖小翼與紙張外觀調整
- 橡皮筋、升降台及導軌等發射裝置，以及航向、張力、高度和仰角設定
- 實驗室、沙漠、草原、賽博與月球環境
- 匯入 GLTF/GLB 或 OBJ 飛機模型，以及全景圖或 3D 地形
- 追逐、側面與自由環繞視角；即時顯示速度、高度、距離、攻角及升阻比

## 本機執行

需要 Node.js 20 或更新版本，以及 pnpm。先在終端機切換到專案資料夾，確認工具已安裝：

```bash
node --version
pnpm --version
```

如果尚未安裝 pnpm，可使用 npm 安裝：

```bash
npm install --global pnpm
```

接著安裝專案依賴並啟動本機開發伺服器：

```bash
pnpm install --frozen-lockfile
pnpm dev
```

在瀏覽器開啟終端機顯示的網址，通常是 `http://localhost:5173/`。開發伺服器會在修改檔案後自動更新頁面；按 `Ctrl+C` 可停止伺服器。

若要檢查正式版建置，可執行：

```bash
pnpm build
pnpm preview
```

`pnpm build` 會將網站輸出至 `dist/`；`pnpm preview` 可在本機預覽建置結果。頁面使用 Tailwind CSS、Three.js、OrbitControls、GLTFLoader、OBJLoader 與 Lucide 的 CDN，開發和使用時都需要網路連線。

## 授權

本專案採用 [MIT License](LICENSE)。
