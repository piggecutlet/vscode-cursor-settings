- Cursor テーマ (斜体 無効)

```
cd "%LOCALAPPDATA%\Programs\cursor\resources\app\extensions"
git clone git@github.com:piggecutlet/cursor-themes-no-italic.git themes-cursor-no-italic
```

```
cd "~/Library/Application Support/Cursor/extensions"
git clone git@github.com:piggecutlet/cursor-themes-no-italic.git themes-cursor-no-italic
```

- 拡張機能 共有

```
mklink /j "%USERPROFILE%\.cursor\extensions" "%USERPROFILE%\.vscode\extensions"
```

```
$ code --list-extensions
dbaeumer.vscode-eslint
esbenp.prettier-vscode
mechatroner.rainbow-csv
ms-ceintl.vscode-language-pack-ja
ms-dotnettools.csharp
ms-dotnettools.vscode-dotnet-runtime
ms-vscode.hexeditor
```

```
code --install-extension dbaeumer.vscode-eslint --install-extension esbenp.prettier-vscode --install-extension mechatroner.rainbow-csv --install-extension ms-ceintl.vscode-language-pack-ja --install-extension ms-dotnettools.csharp@2.93.22 --install-extension ms-dotnettools.vscode-dotnet-runtime --install-extension ms-vscode.hexeditor
```

- settings.json 共有
  ※ 管理者権限が必要

```
mklink "%APPDATA%\Code\User\settings.json" "C:\Users\user\main\git\vscode-cursor-settings\settings.json"
mklink "%APPDATA%\Cursor\User\settings.json" "C:\Users\user\main\git\vscode-cursor-settings\settings.json"
```
- keybindings.json 共有
  ※ 管理者権限が必要

```
mklink "%APPDATA%\Code\User\keybindings.json" "C:\Users\user\main\git\vscode-cursor-settings\keybindings.json"
mklink "%APPDATA%\Cursor\User\keybindings.json" "C:\Users\user\main\git\vscode-cursor-settings\keybindings.json"
```

```
C:\Users\user>mklink
シンボリック リンクを作成します。

MKLINK [[/D] | [/H] | [/J]] リンク ターゲット

        /D          ディレクトリのシンボリック リンクを作成します。既定では、
                    ファイルのシンボリック リンクが作成されます。
        /H          シンボリック リンクではなく、ハード リンクを作成します。
        /J          ディレクトリ ジャンクションを作成します。
        リンク      新しいシンボリック リンク名を指定します。
        ターゲット  新しいリンクが参照するパス (相対または絶対)
                    を指定します。
```
