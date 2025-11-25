
# Jekyll サイトマップテンプレート

GitHub Pages（Jekyll）向けの **HTMLサイトマップ**テンプレートです。HTMLを書かずに、Liquidでページ・投稿・コレクションを自動列挙します。

## 同梱ファイル
- `sitemap-basic.md` … Markdownベースのシンプルな自動サイトマップ
- `sitemap-advanced.html` … コレクションにも対応した汎用テンプレート
- `_config-addons.yml` … 除外設定のサンプル（既存の`_config.yml`に追記）

## 使い方
1. このZIPを展開し、`sitemap-basic.md` または `sitemap-advanced.html` を **リポジトリのルート**に置きます。
2. そのままコミット＆Push。
3. 公開URLは `https://<username>.github.io/sitemap/` （ユーザーサイト）または `https://<username>.github.io/<repo>/sitemap/`（プロジェクトサイト）。
4. 必要に応じて `_config.yml` に、`_config-addons.yml` の `defaults` をマージして、特定パスをサイトマップから除外します。

### 任意設定（各ページ／投稿）
- サイトマップから除外したい場合：
  ```yaml
  ---
  title: 非公開ページ
  sitemap: false
  ---
  ```

### ナビゲーションにリンクを追加
テーマのヘッダー／フッター等に：
```html
<a href="{{ '/sitemap/' | relative_url }}">サイトマップ</a>
```

### 注意
- `relative_url` を使っているため、ユーザーサイト／プロジェクトサイトのどちらでも正しいリンクになります。
- `title` が未設定のページはURLを表示します。見栄えを整える場合は各ページの Front Matter に `title:` を追加してください。
