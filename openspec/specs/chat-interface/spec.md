# Capability: 聊天介面 (Chat Interface)

## Purpose
提供一個基於 Vue 3 與 Gemini API 的簡單聊天介面，讓使用者可以與 AI 進行對話。
## Requirements
### Requirement: Send Message
使用者 SHALL 能夠向 AI 發送文字訊息。

#### Scenario: 使用者發送訊息
- **WHEN** 使用者在輸入欄位輸入文字並點擊發送或按回車鍵
- **THEN** 訊息將被添加到聊天記錄並發送到 Gemini API
- **AND** AI 的回應將顯示在聊天記錄中

### Requirement: Tech Stack
該應用程式 SHALL 為一個使用 Vue 3 和 Tailwind CSS 的單頁 HTML 檔案。
Gemini API 調用時使用的 API Key MUST 從 UI 輸入欄位動態獲取。
仍以非串流 (non-streaming) 模式調用。

#### Scenario: 動態 API Key 使用
- **WHEN** 發送訊息時
- **THEN** 請求網址中包含的金鑰參數由 UI 上的輸入欄位提供

### Requirement: Default Model
該應用程式 SHALL 在初始加載時默認使用 `gemini-3-flash-preview` 模型。

#### Scenario: Default model selection
- **WHEN** the application is first loaded
- **THEN** the model selection dropdown defaults to "Gemini 3 Flash (Preview)"

### Requirement: Model Selection
使用者 SHALL 能夠從 UI 的下拉選單中選擇 Gemini 模型。

#### Scenario: User selects a different model
- **WHEN** user selects a model from the dropdown (e.g., "Gemini 1.5 Pro")
- **THEN** future messages sent SHALL use the selected model endpoint
- **AND** the selection MUST be limited to Gemini series models

### Requirement: API Key Input
使用者 SHALL 能夠在 UI 上輸入 Gemini API Key。

#### Scenario: User provides an API Key
- **WHEN** 使用者在 API Key 輸入欄位填入金鑰
- **THEN** 之後發送的所有 API 請求 MUST 使用該金鑰進行驗證
- **AND** 輸入欄位 MUST 隱藏金鑰內容 (使用 password 類型)

