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

需要 Node.js 20 或更新版本，以及 pnpm。

```bash
pnpm install
pnpm dev
```

開啟終端機顯示的本機網址。建置網站可執行：

```bash
pnpm build
```

建置結果會輸出至 `dist/`。本專案使用 Tailwind CSS、Three.js、OrbitControls、GLTFLoader、OBJLoader 與 Lucide 的 CDN，因此使用時需要網路連線。

## 授權

本專案採用 [MIT License](LICENSE)。
