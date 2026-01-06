## Python

## Python Debugger

## Chinese (Traditional) Language Pack for Visual Studio Code

## GitLens

## Git Graph

## Git History

## markdownlint

## Markdown All in One

## Office Viewer

## 修改Markdown文字顏色
(需切換原生的Markdown介面才可操作)
在 VS Code 中，點擊左下角的 齒輪圖示 ⚙️。
1. 選擇 「使用者程式碼片段」(User Snippets)。
2. 在上方出現的搜尋框中輸入 markdown，然後點擊搜尋到的 markdown (Markdown) 檔案。這會開啟一個 markdown.json 檔案。
3. 在 markdown.json 的大括號 { ... } 之中，貼上以下這段代碼（如果原本裡面有範例註解，可以直接刪除或貼在後面）：
```
{
	"Red Text": {
    "prefix": "cr",
    "body": ["<span style=\"color:red\">$1</span>$0"]
 	 },
  	"Blue Text": {
    "prefix": "cb",
    "body": ["<span style=\"color:blue\">$1</span>$0"]
 	 },
  	"Green Text": {
    "prefix": "cg",
    "body": ["<span style=\"color:green\">$1</span>$0"]
}
```
使用指令面板 (Command Palette)
1. 按下 F1 或 Ctrl(command) + Shift + P。
2. 在上方出現的輸入框中輸入 user settings json。
3. 選擇 「偏好設定: 開啟使用者設定 (JSON)」 (Preferences: Open User Settings (JSON))。
將以下代碼貼在大括號 { } 裡面（記得如果前面有其他設定，要加個逗號 , 分隔）：
```
"[markdown]": {
    "editor.quickSuggestions": {
        "other": true,
        "comments": true,
        "strings": true
    },
    "editor.snippetSuggestions": "top"
}
```
