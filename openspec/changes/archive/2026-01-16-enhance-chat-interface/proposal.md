# Change: 強化聊天介面功能 (Enhance Chat Interface)

## Why
為了提供更彈性且安全的使用體驗，使用者需要能夠在介面上切換不同的 Gemini 模型，並能動態輸入自己的 API Key，避免將私密金鑰硬編碼在程式中。

## What Changes
- 在「發送」按鈕左側新增模型選擇器（已完成）。
- 在「發送」按鈕下方新增 API Key 輸入欄位。
- 更新 API 請求邏輯，使其同時支援選定的模型與使用者輸入的 API Key。
- 欄位樣式應統一採用玻璃擬態 (glassmorphism) 設計。

## Impact
- 受影響的規格：`specs/chat-interface/spec.md`
- 受影響的程式碼：`index.html` (Vue 3 邏輯與 UI)
