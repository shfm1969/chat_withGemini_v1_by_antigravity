## ADDED Requirements

### Requirement: Model Selection
使用者 SHALL 能夠從 UI 的下拉選單中選擇 Gemini 模型。

#### Scenario: User selects a different model
- **WHEN** user selects a model from the dropdown (e.g., "Gemini 1.5 Pro")
- **THEN** future messages sent SHALL use the selected model endpoint
- **AND** the selection MUST be limited to Gemini series models

## MODIFIED Requirements

### Requirement: Default Model
該應用程式 SHALL 在初始加載時默認使用 `gemini-1.5-flash` 模型。

#### Scenario: Default model selection
- **WHEN** the application is first loaded
- **THEN** the model selection dropdown defaults to "Gemini 1.5 Flash"
