# PDFページ工房（GitHub Pages版）

このフォルダの内容は、そのまま静的Webサイトとして公開できます。

## GitHub Pagesで公開する

1. GitHubで新しいリポジトリを作成します。
2. このフォルダのファイルを、リポジトリのルートへアップロードします。
3. GitHubの **Settings → Pages** を開きます。
4. **Build and deployment** を **Deploy from a branch** にします。
5. ブランチを **main**、フォルダを **/(root)** にして保存します。
6. 数分後、GitHub PagesのURLからアプリを使用できます。

アップロードしたPDFはブラウザ内で処理され、サーバーには保存されません。

## ソースから公開用ファイルを作り直す

プロジェクトのルートで次を実行すると、`docs` フォルダが更新されます。

```powershell
pnpm build:github
```

プロジェクト全体をGitHubへ登録する場合は、GitHub Pagesの公開フォルダとして
**main** ブランチの **/docs** を選択してください。
