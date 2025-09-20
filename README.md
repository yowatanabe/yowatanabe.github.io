# yowatanabe.github.io

プロフィールサイトです。SREとしてのキャリア、技術スキル、保有資格などを紹介しています。

## 🌐 サイトURL

https://yowatanabe.github.io/

## 📄 ページ構成

- **Profile**: 経歴・スキル・資格の詳細
- **Career**: キャリア履歴
- **Side Job**: 副業募集情報

## 🛠 技術スタック

- **静的サイトジェネレーター**: [Hugo](https://gohugo.io/)
- **テーマ**: [hugo-theme-hello-friend-ng](https://github.com/rhazdon/hugo-theme-hello-friend-ng)
- **ホスティング**: GitHub Pages
- **デプロイ**: GitHub Actions

## 🚀 ローカル開発

```bash
# 開発サーバー起動
hugo server
```

## ⚙️ 副業募集の表示制御

副業募集を終了する場合は、`hugo.toml`で以下の設定を変更：

```toml
[params]
  # プロフィールページに副業募集のお知らせを表示(true|false)
  showSideJobNotice = false  # true → false に変更
```

これにより、プロフィールページのお知らせとヘッダーのSide Jobリンクが非表示となる。
