## ADDED Requirements

### Requirement: API Key Input
使用者 SHALL 能夠在 UI 上輸入 Gemini API Key。

#### Scenario: User provides an API Key
- **WHEN** 使用者在 API Key 輸入欄位填入金鑰
- **THEN** 之後發送的所有 API 請求 MUST 使用該金鑰進行驗證
- **AND** 輸入欄位 MUST 隱藏金鑰內容 (使用 password 類型)

## MODIFIED Requirements

### Requirement: Tech Stack
該應用程式 SHALL 為一個使用 Vue 3 和 Tailwind CSS 的單頁 HTML 檔案。
Gemini API 調用時使用的 API Key MUST 從 UI 輸入欄位動態獲取。
仍以非串流 (non-streaming) 模式調用。

#### Scenario: 動態 API Key 使用
- **WHEN** 發送訊息時
- **THEN** 請求網址中包含的金鑰參數由 UI 上的輸入欄位提供
