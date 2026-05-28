# 店舗別売上・GA4アクセス分析ダッシュボード

店舗名を「A店、B店、C店」などのアルファベット表記に匿名化したダッシュボードです。
GitHub Pagesにアップロードすることで、Webブラウザ経由でアクセス可能なダッシュボードを公開できます。

## 構成ファイル
- **[index.html](file:///C:/Users/33249/.gemini/antigravity/scratch/github_pages/index.html)**: 匿名化済みのダッシュボード本体（HTML/CSS/JavaScriptおよびデータがすべて含まれるスタンドアロン版です）。

## GitHub Pages への公開方法

### 方法1: ブラウザの画面から手動でアップロードする場合（最も簡単）

1. **GitHubアカウントにログインし、新しいリポジトリを作成します。**
   - リポジトリ名を設定します（例: `store-sales-dashboard`）。
   - 公開設定（Public/Private）を選択します（GitHub Pagesの無料枠では **Public** に設定する必要があります）。
   - 「Add a README file」にチェックを入れずに「Create repository」をクリックします。
2. **ファイルをアップロードします。**
   - リポジトリの初期画面で **「uploading an existing file」** リンクをクリックします。
   - このフォルダにある **[index.html](file:///C:/Users/33249/.gemini/antigravity/scratch/github_pages/index.html)** をドラッグ＆ドロップしてアップロードします。
   - 画面下部の「Commit changes」をクリックして保存します。
3. **GitHub Pagesを有効化します。**
   - リポジトリ画面上部のメニューから **「Settings」**（歯車マーク）を選択します。
   - 左サイドバーの「Code and automation」セクション内にある **「Pages」** を選択します。
   - 「Build and deployment」の中の **「Branch」** 設定で、`None` から `main`（または `master`）を選択し、保存（Save）します。
4. **公開されたURLにアクセスします。**
   - 数分待ってからページを再読み込みすると、画面上部に公開URL（例: `https://<ユーザー名>.github.io/store-sales-dashboard/`）が表示されます。

---

### 方法2: Git コマンドを使用する場合

Gitがインストールされている場合、以下のコマンドで直接デプロイ可能です。

```bash
# github_pages フォルダに移動
cd C:\Users\33249\.gemini\antigravity\scratch\github_pages

# git リポジトリを初期化
git init

# リポジトリにファイルを追加してコミット
git add index.html
git commit -m "Initial commit with anonymized dashboard"

# ブランチ名を main に変更
git branch -M main

# リモートリポジトリ（GitHub）の登録
# ※ URLはご自身で作成したリポジトリのものに書き換えてください
git remote add origin https://github.com/<あなたのユーザー名>/<リポジトリ名>.git

# 変更をプッシュ
git push -u origin main
```

その後、GitHubのリポジトリ設定（Settings -> Pages）から公開設定を行ってください。
