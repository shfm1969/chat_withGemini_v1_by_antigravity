# Change: 新增模型選擇器 (Add Model Selector)

## Why
使用者需要能夠直接從使用者介面切換不同的 Gemini 模型（例如：Flash 與 Pro, 或是不同版本) 以便平衡回應速度與品質。

## What Changes
- 在「發送」按鈕左側新增一個下拉選單或選擇欄位。
- 允許使用者從 Gemini 模型列表中進行選擇。
- 更新 API 請求以使用所選的模型。
- 限制選擇範圍與僅限於 Gemini 系列模型。

## Impact
- 受影響的規格：`specs/chat-interface/spec.md`
- 受影響的程式碼：`index.html` (Vue 3 邏輯與 UI)
