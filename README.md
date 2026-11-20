# KIBF2026 謎解きクリアページ

京都インディーボドゲ祭2026の謎解きクリア報告用ページです。

公開予定URL：

https://clear.kibf.tatami-studio.games/

## GitHub Pagesの公開手順

1. GitHubで新しいリポジトリを作成します。
2. このフォルダ内のファイルを、リポジトリ直下へすべてアップロードします。
3. リポジトリの `Settings` → `Pages` を開きます。
4. `Build and deployment` のSourceを `Deploy from a branch` にします。
5. Branchを `main`、フォルダを `/(root)` にして保存します。
6. `Custom domain` に `clear.kibf.tatami-studio.games` を入力して保存します。

## DNS設定

ドメインのDNS管理画面で、以下のCNAMEレコードを追加します。

| 種類 | ホスト名 | 値 |
|---|---|---|
| CNAME | clear | GitHubユーザー名.github.io |

`GitHubユーザー名`の部分だけ、実際のGitHubユーザー名へ置き換えてください。リポジトリ名は付けません。

DNS確認とHTTPS証明書の発行が完了したら、GitHub Pages設定の `Enforce HTTPS` を有効にします。

## QRコードへ入れるURL

QRコードは、このクリアページそのものではなく、次の形式のX投稿画面URLへ向けます。

```text
https://x.com/intent/post?text=URLエンコード済みの投稿本文
```

投稿本文の内容：

```text
京都インディーボドゲ祭2026の謎解きイベント、全問正解しました！
#kibf2026
https://clear.kibf.tatami-studio.games/
```

公開後は、ページ内の「Xでクリアを報告する」ボタンを押すことで同じ投稿画面を確認できます。そのボタンのリンクをQRコードへ使用しても構いません。

## 公開前の確認

- `https://clear.kibf.tatami-studio.games/` がHTTPSで開けること
- 画像が表示されること
- 「KIBF公式サイトへ」が `https://kibf.tatami-studio.games/` を開くこと
- 「Xでクリアを報告する」で本文とハッシュタグが入力されること
- Xへ投稿する前に、カード画像が表示されること

Xが画像情報をキャッシュする可能性があるため、画像・タイトル・URLを完成させてから最初の投稿テストを行ってください。
