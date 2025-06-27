# 📱 iPhoneでアプリを開く手順

## 🚀 Streamlit Cloudでデプロイ

### 1️⃣ GitHubにアップロード

1. **GitHub.com**にログイン
2. **New repository**をクリック
3. Repository name: `ai-character-chatbot`
4. **Public**を選択（無料でデプロイするため）
5. **Create repository**をクリック

### 2️⃣ コードをアップロード

コマンドプロンプトで以下を実行：

```bash
cd "c:\Users\kohar\Desktop\script\chat"
git remote add origin https://github.com/YOUR_USERNAME/ai-character-chatbot.git
git branch -M main
git push -u origin main
```

※ `YOUR_USERNAME`を実際のGitHubユーザー名に変更

### 3️⃣ Streamlit Cloudでデプロイ

1. **https://share.streamlit.io** にアクセス
2. **GitHubアカウントでログイン**
3. **New app**をクリック
4. Repository: `ai-character-chatbot`を選択
5. Branch: `main`
6. Main file path: `app.py`
7. **Deploy!**をクリック

### 4️⃣ 環境変数の設定

1. デプロイ後、アプリのSettings → **Secrets**
2. **Add secret**をクリック
3. Key: `GEMINI_API_KEY`
4. Value: あなたのGemini APIキー
5. **Save**をクリック

### 5️⃣ iPhoneでアクセス

1. **Safari**を開く
2. 生成されたURL（例：https://your-app.streamlit.app）にアクセス
3. **ホーム画面に追加**で、アプリのように使用可能！

## 🔧 トラブルシューティング

### 音声機能について
- iPhoneでは音声機能は制限される場合があります
- チャット機能は完全に動作します

### 画像生成について
- Stable Diffusionサーバーがローカルの場合は動作しません
- キャラクター機能とチャットは正常動作します

## 📞 サポート

問題が発生した場合は、以下をチェック：
1. Gemini APIキーが正しく設定されているか
2. GitHub repository が Public になっているか
3. ブラウザのエラーコンソールを確認

## 🎉 完了！

これでiPhoneからいつでもAIキャラクターチャットボットを楽しめます！
