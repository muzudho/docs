# Visual Studio Code 設定


## ターミナルのデフォルトをPowerShellからCommandPromptへ変更

VSCode の 📄 `settings.json` ファイルを開き、以下の行を追加（抜粋）：  

📄 `settings.json` 抜粋:  

```json
{
    "terminal.integrated.defaultProfile.windows": "Command Prompt",
}
```


## ターミナルの文字エンコーディングをUTF-8に変更


VSCode の 📄 `settings.json` ファイルを開き、以下の行を追加（抜粋）：  

📄 `settings.json` 抜粋:  

```json
{
    "terminal.integrated.profiles.windows": {
        "Command Prompt": {
            "args": ["/k", "chcp 65001"]
        }
    }
}
```


## Go言語のツールのの文字エンコーディングをUTF-8に変更

VSCode の 📄 `settings.json` ファイルを開き、以下の行を追加（抜粋）：  

📄 `settings.json` 抜粋:  

```json
{
    "go.toolsEnvVars": {
        "LANG": "ja_JP.UTF-8"
    }
}
```
