# VSCode Cursor Settings

## extensions

- Windows (Command Prompt)

```
mklink /j "%USERPROFILE%\.cursor\extensions" "%USERPROFILE%\.vscode\extensions"
```

## extensions.json

```
code --list-extensions
```

```
anthropic.claude-code
dbaeumer.vscode-eslint
esbenp.prettier-vscode
jishii1204.markdown-live-editor
mechatroner.rainbow-csv
ms-ceintl.vscode-language-pack-ja
ms-dotnettools.csharp
ms-dotnettools.vscode-dotnet-runtime
ms-vscode.hexeditor
openai.chatgpt
webpro.vscode-knip
yoavbls.pretty-ts-errors
```

```
code --install-extension anthropic.claude-code --install-extension dbaeumer.vscode-eslint --install-extension esbenp.prettier-vscode --install-extension jishii1204.markdown-live-editor --install-extension mechatroner.rainbow-csv --install-extension ms-ceintl.vscode-language-pack-ja --install-extension ms-dotnettools.csharp@2.93.22 --install-extension ms-dotnettools.vscode-dotnet-runtime --install-extension ms-vscode.hexeditor --install-extension openai.chatgpt  --install-extension webpro.vscode-knip --install-extension yoavbls.pretty-ts-errors
```

## keybindings.json

- Windows (Command Prompt)

※ 管理者権限が必要

```
mklink "%APPDATA%\Code\User\keybindings.json" "%USERPROFILE%\main\git\vscode-cursor-settings\keybindings.json"
mklink "%APPDATA%\Cursor\User\keybindings.json" "%USERPROFILE%\main\git\vscode-cursor-settings\keybindings.json"
```

- macOS (bash / zsh)

```
curl -fLo "$HOME/Library/Application Support/Cursor/User/keybindings.json" "https://raw.githubusercontent.com/piggecutlet/vscode-cursor-settings/refs/heads/main/keybindings.json"
```

## mcp.json

```
mklink "%USERPROFILE%\.cursor\mcp.json" "%USERPROFILE%\main\git\vscode-cursor-settings\mcp.json"
```

## settings.json

※ 管理者権限が必要

```
mklink "%APPDATA%\Code\User\settings.json" "%USERPROFILE%\main\git\vscode-cursor-settings\settings.json"
mklink "%APPDATA%\Cursor\User\settings.json" "%USERPROFILE%\main\git\vscode-cursor-settings\settings.json"
```

- macOS (bash / zsh)

```
curl -fLo "$HOME/Library/Application Support/Cursor/User/settings.json" "https://raw.githubusercontent.com/piggecutlet/vscode-cursor-settings/refs/heads/main/settings.json"
```
