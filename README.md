# 🕹️ Java Pac-Man 小精靈遊戲

歡迎來到經典小精靈（Pac-Man）的 Java 重製版專案！本專案使用 Java Swing 進行視窗繪製與事件處理，並實作了基本的地圖載入、小精靈移動與鬼魂機制。

## 📁 專案資料夾結構

本專案採用 VS Code Java 的標準結構：

- `src/`：存放所有 Java 原始碼（`.java`）以及遊戲所需的圖片資源（`.png`）。
- `bin/`：存放編譯後的位元組碼檔案（`.class`），由系統自動生成。
- `lib/`：存放專案外部依賴庫（目前主要使用 Java 內建 API，故此處可能為空）。

> ⚠️ **重要提醒**：所有遊戲圖片（如 `wall.png`、`blueGhost.png` 等）皆必須放置於 `src/` 根目錄下，以確保程式能透過 `getClass().getResource()` 順利讀取，避免引發 `NullPointerException`。

---

## 🚀 遊戲執行與打包說明

### 1. 在 VS Code 中開發與執行
- 程式的主要進入點為 `App.java`。
- 在 VS Code 中開啟本專案，至 `App.java` 並點擊右上方或主程式內的 **Run Java** 即可啟動遊戲。

### 2. 打包成獨立發行版（JAR 檔）
為了讓遊戲可以脫離 IDE 獨立執行，可以透過以下方式打包：
- **推薦方式**：在 VS Code 左下角的 `JAVA PROJECTS` 面板中，點擊專案右側的 **Export to Jar...** 箭頭圖示，並選擇 `App` 作為 Main Class。打包時請確保勾選 `src` 內的所有 `.png` 檔案。