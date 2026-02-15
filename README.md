- 拡張機能 共有

```
mklink /j "%USERPROFILE%\.cursor\extensions" "%USERPROFILE%\.vscode\extensions"
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
