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
# --install-extension ms-dotnettools.csharp@2.93.22 --install-extension ms-dotnettools.vscode-dotnet-runtime
code --install-extension dbaeumer.vscode-eslint --install-extension esbenp.prettier-vscode --install-extension jishii1204.markdown-live-editor --install-extension mechatroner.rainbow-csv --install-extension ms-ceintl.vscode-language-pack-ja --install-extension ms-vscode.hexeditor --install-extension webpro.vscode-knip --install-extension yoavbls.pretty-ts-errors
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
curl -fLo "$HOME/Library/Application Support/Code/User/keybindings.json" "https://raw.githubusercontent.com/piggecutlet/vscode-cursor-settings/refs/heads/main/keybindings.json"

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
curl -fLo "$HOME/Library/Application Support/Code/User/settings.json" "https://raw.githubusercontent.com/piggecutlet/vscode-cursor-settings/refs/heads/main/settings.json"

curl -fLo "$HOME/Library/Application Support/Cursor/User/settings.json" "https://raw.githubusercontent.com/piggecutlet/vscode-cursor-settings/refs/heads/main/settings.json"
```

## WYSIWYG

- Windows (Command Prompt)

```pwsh
$file = "$env:LOCALAPPDATA\Programs\cursor\resources\app\out\vs\workbench\workbench.desktop.main.js"
(Get-Content $file -Raw -Encoding UTF8).Replace('[".cursor",".claude",".codex"]', '[]') | Set-Content $file -Encoding UTF8 -NoNewline
```

- macOS (bash / zsh)

```zsh
perl -pi -e 's/\["\.cursor","\.claude","\.codex"\]/[]/g' "/Applications/Cursor.app/Contents/Resources/app/out/vs/workbench/workbench.desktop.main.js"
```
