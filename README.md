# Retro VDP Converter

レトロゲーム機の画面仕様に画像を変換するWebアプリケーション

## デプロイ方法

### GitHub Pagesへのデプロイ

1. GitHubにリポジトリを作成
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/retro-converter.git
git push -u origin main
```

2. GitHubリポジトリの Settings → Pages → Source で `main` ブランチを選択

3. 数分後、以下のURLでアクセス可能になります：
   `https://YOUR_USERNAME.github.io/retro-converter/`

### その他のデプロイオプション

- **Netlify**: リポジトリを連携して自動デプロイ
- **Vercel**: GitHub連携で簡単デプロイ
- **Cloudflare Pages**: 高速なCDN配信

## ローカルでの実行

HTTPサーバーが必要です（Service Worker使用のため）：

```bash
# Python 3
python -m http.server 8000

# Node.js (npx)
npx http-server
```

その後、`http://localhost:8000` にアクセス
