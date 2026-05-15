# yazi dotfiles

[yazi](https://github.com/sxyazi/yazi) の設定ファイル（TOML）を管理するリポジトリです。

## ファイル構成

| ファイル | 説明 |
|---|---|
| `yazi.toml` | 基本設定（パネル比率、隠しファイル表示など） |
| `keymap.toml` | キーバインド設定 |
| `package.toml` | プラグイン依存関係 |

## 設定の概要

### yazi.toml

- パネル比率: 左非表示 / 中央最大幅 / 右非表示（`ratio = [0, 10, 0]`）
- 隠しファイルをデフォルトで表示

### keymap.toml

- `<Backspace>` で親ディレクトリに戻る
- `<Enter>` でディレクトリ移動またはファイルを開く（`smart-enter` プラグイン使用）
- `<Esc>` で入力をキャンセル

### package.toml

- [`smart-enter`](https://github.com/yazi-rs/plugins) プラグインを使用

## セットアップ

```bash
# リポジトリをクローン
git clone https://github.com/noxsyn-z27/yaji-dotenv.git ~/.config/yazi

# プラグインをインストール
ya pack -i
```

> `plugins/` ディレクトリは `.gitignore` により管理対象外です。`ya pack -i` で再生成してください。
