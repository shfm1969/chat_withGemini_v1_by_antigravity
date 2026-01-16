## 1. Implementation

### 模型選擇功能 (已實作)
- [x] 1.1 在發送按鈕左側新增 `<select>` 下拉選單。
- [x] 1.2 綁定 `selectedModel` 並更新 `getApiUrl` 邏輯。

### API Key 輸入功能 (已實作)
- [x] 2.1 在發送按鈕及其所屬行的下方新增 API Key 輸入欄位。
- [x] 2.2 欄位須設為 `type="password"` 以保護金鑰隱私。
- [x] 2.3 使用 Tailwind CSS 套用玻璃擬態樣式。
- [x] 2.4 將欄位綁定至 Vue 的 `apiKey` 反應式變數。
- [x] 2.5 更新 `getApiUrl` 邏輯，使其從 `apiKey` 變數獲取金鑰，而非硬編碼。
- [x] 2.6 在發送訊息前檢查 API Key 是否已填寫。

## 2. Validation
- [x] 3.1 驗證模型切換功能正常運作。
- [x] 3.2 驗證 API Key 輸入後能正確套用於請求中。
- [x] 3.3 驗證輸入欄位的隱蔽性 (`type="password"`)。
