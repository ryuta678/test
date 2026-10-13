# AWS Amplifyとは

AWS Amplifyは、WebサイトやWebアプリケーションを簡単に公開できるAWSのサービスです。

## 特徴

- サーバ構築が不要
- GitHubと連携可能
- HTTPSが自動で有効化される
- Git Pushだけでサイト更新が可能

## 構成例

```text
作業PC
 ↓
GitHub
 ↓
AWS Amplify
 ↓
公開サイト
```

## メリット

### 運用が簡単

EC2のような以下の作業が不要です。

- OSアップデート
- Webサーバ設定
- セキュリティパッチ適用
- サーバ監視

### GitHub連携

GitHubへPushすると自動的にサイトが更新されます。

```bash
git add .
git commit -m "記事追加"
git push
```

## EC2との比較

| 項目 | EC2 | Amplify |
|------|------|------|
| サーバ構築 | 必要 | 不要 |
| OS管理 | 必要 | 不要 |
| Webサーバ設定 | 必要 | 不要 |
| HTTPS