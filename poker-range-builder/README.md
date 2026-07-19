# Poker Range Builder

ブラウザだけで動作するポーカーハンドレンジ作成アプリです。

## 機能

- 13×13のハンドマトリクス
- Bet / Raise、Call、Mixed、Foldの入力
- クリック・ドラッグによる連続入力
- 同じアクションの再クリックで未入力へ戻す
- スペースキー＋クリック／ドラッグで消去
- 頻度設定
- コンボ数・レンジ割合の集計
- ブラウザ内保存
- JSON入出力
- PNG出力

## ローカルで開く

`index.html`をダブルクリックしてブラウザで開いてください。

## GitHub Pagesで公開する手順

1. GitHubで新しいリポジトリを作成します。
2. このフォルダ内のファイルをリポジトリへ追加します。
3. GitHubのリポジトリ画面で `Settings` を開きます。
4. 左側の `Pages` を開きます。
5. `Build and deployment` の `Source` を `Deploy from a branch` にします。
6. Branchを `main`、フォルダを `/(root)` に設定して `Save` を押します。
7. 数分後、GitHub PagesのURLからアプリを開けます。

## コマンドでGitHubへ登録する例

```bash
cd poker-range-builder-github

git init
git add .
git commit -m "feat: add poker range builder"
git branch -M main
git remote add origin https://github.com/ユーザー名/リポジトリ名.git
git push -u origin main
```

## 保存について

「保存」ボタンで保存したレンジは、使用中のブラウザのLocalStorageに保存されます。

- 同じ端末・同じブラウザでは次回も読み込めます
- 別の端末や別のブラウザには自動共有されません
- ブラウザデータを削除すると消える可能性があります
- 別端末へ渡す場合はJSON出力を使用してください
