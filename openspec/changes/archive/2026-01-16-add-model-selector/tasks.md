## 1. Implementation

### UI 更新
- [x] 1.1 在 `index.html` 的發送按鈕左側新增一個 `<select>` 下拉選單。
- [x] 1.2 使用 Tailwind CSS 設定下拉選單樣式，以符合玻璃擬態 (glassmorphism) 主題。
- [x] 1.3 將下拉選單綁定到名為 `selectedModel` 的新 Vue `ref`。

### 邏輯更新
- [x] 2.1 定義可用 Gemini 模型列表（例如：`gemini-1.5-flash`, `gemini-1.5-pro`, `gemini-2.0-flash-exp`）。
- [x] 2.2 更新 `API_URL` 的生成邏輯，動態使用 `selectedModel`。
- [x] 2.3 確保 UI 中的模型指示器反映當前選擇的模型。

## 2. 驗證 (Validation)
- [x] 3.1 驗證切換模型是否會更新 `API_URL`。
- [x] 3.2 驗證下拉選單中僅提供 Gemini 系列模型。
- [x] 3.3 測試使用不同模型發送訊息的功能。
