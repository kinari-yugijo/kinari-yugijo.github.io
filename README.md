# きなりの遊戯場 — 製品説明書

BOOTH 等で頒布している製品の説明書。GitHub Pages で公開している。

**このリポジトリ名は `kinari-yugijo.github.io` にすること。**
GitHub の「ユーザーサイト」扱いになり、URL からリポジトリ名が消える。

| 製品 | URL |
|---|---|
| クロノスレート ChronoSlate | https://kinari-yugijo.github.io/chronoslate/ |

## 中身

```
index.html              ブランドのトップ（製品一覧）
chronoslate/
  index.html            言語振り分け（JS が無くてもリンクで進める）
  manual_jp.html
  manual_en.html
robots.txt              頒布開始まで Disallow: /
.nojekyll               Jekyll を通さず素の HTML をそのまま配信する
```

## 運用

- **編集は開発リポジトリ側**（`vrc-gimmicks/Distribution/<製品名>/`）で行い、
  完成したものをここへコピーして push する。開発の経緯をこちらに持ち込まない
- このリポジトリは public なので、**成果物の HTML 以外を置かない**
- コミットメッセージは「クロノスレート説明書を公開」程度の淡々とした文面に統一する
- 頒布開始したら `robots.txt` の `Disallow: /` と各 HTML の `noindex` を外す

## 初期設定（アカウント作成直後にやること）

1. Settings → Emails → **Keep my email addresses private** を有効化
2. Settings → Pages → Source を `main` ブランチのルートに設定
