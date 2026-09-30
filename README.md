# pages

kage367 のアプリのページ（プライバシーポリシー・サポートページ）を GitHub Pages で公開する。

公開先: https://kage367.github.io/pages/

```
index.html            アプリ一覧
style.css             共通スタイル
.nojekyll             Jekyll の変換を使わず、ファイルをそのまま公開する
flashcard/
  index.html          ぴよカードの紹介ページ（App Store の「サポートURL」）
  privacy.html        ぴよカードのプライバシーポリシー（App Store の「プライバシーポリシーURL」）
  icon.png            アプリアイコン（flash_card リポジトリの Tools/draw_app_icon.swift で作ったもの）
```

| ページ | URL |
|---|---|
| アプリ一覧 | https://kage367.github.io/pages/ |
| ぴよカード | https://kage367.github.io/pages/flashcard/ |
| プライバシーポリシー | https://kage367.github.io/pages/flashcard/privacy.html |

## 公開のしかた

1. 変更を `main` に入れて push する
2. 初回だけ: リポジトリの Settings > Pages で
   「Source: Deploy from a branch」→ ブランチ `main` / フォルダ `/ (root)` を選んで保存する
3. 数分で上の URL に反映される

## アプリを増やすとき

1. `flashcard/` と同じ形でアプリごとのフォルダを作る（`index.html` と `privacy.html`）
2. ルートの `index.html` のアプリ一覧に1行足す
3. リンクは相対パスで書く（`../style.css` など）

## 注意

- App Store に出しているあいだ、プライバシーポリシーの URL は生きている必要がある。
  このリポジトリを非公開にしたり、名前を変えたり、ファイルを移動したりすると URL が切れる
- ポリシーの内容を変えたら、ページ内の「最終更新日」も更新する
