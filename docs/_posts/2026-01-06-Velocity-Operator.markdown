---
layout: post
title: "速度演算子の定義って当たり前？"
date:  2026-01-06 00:56:00 +0900
categories: jekyll update
---

[PDFを開く](https://Koichi-Sugihara.github.io/assets/pdf/velocity_operator.pdf){:target="_blank" rel="noopener"}



# PDFの埋め込み（iframe）サンプル

> このページは **iframeでPDFを埋め込み**、さらに **ダウンロードリンク** と **objectタグのフォールバック** を備えています。
> そのまま GitHub Pages の `docs/index.md` として使えます。必要に応じてURLを書き換えてください。

---

## 埋め込み（iframe）

<!-- ✅ 必要に応じて以下のURLを書き換えてください。
 - ユーザーサイトの場合: https://Koichi-Sugihara.github.io/asset/pdf/velocity_operator.pdf
 - プロジェクトサイトの場合: https://Koichi-Sugihara.github.io/asset/pdf/velocity_operator.pdf
 - 相対パスでも可: /asset/pdf/velocity_operator.pdf  （Pagesのルートがdocsの場合）
-->

<iframe src="/asset/pdf/velocity_operator.pdf" width="100%" height="720" style="border:1px solid #ddd; border-radius:8px;" title="PDFプレビュー"></iframe>

---

## フォールバック（PDFが埋め込めない環境向け）

<object data="/asset/pdf/velocity_operator.pdf" type="application/pdf" width="100%" height="720">
  <p>
    お使いの環境ではPDFのプレビューが表示できません。
    <a href="/asset/pdf/velocity_operator.pdf" download>こちらからPDFをダウンロード</a> してください。
  </p>
</object>

---

## ダウンロードリンクのみの表示（任意）

[PDFをダウンロード](/asset/pdf/velocity_operator.pdf)

---

### メモ
- `width` / `height` は任意のサイズに調整できます。
- `src` / `data` のURLは**絶対パス**でも**相対パス**でも構いません。
- GitHub Pagesの公開設定が `master` / `docs` の場合、`docs` がサイトルートになるため、`/asset/pdf/velocity_operator.pdf` のようなルート相対パスで参照できます。
- もしユーザーサイト（`Koichi-Sugihara.github.io`）でリポジトリ直下公開の場合は、`/asset/pdf/…` のままでOKです。

<!-- 例: 絶対パスを使う場合（ユーザー名とリポジトリ名を置き換え）
<iframe src="https://Koichi-Sugihara.github.io/asset/pdf/velocity_operator.pdf" width="100%" height="720"></iframe>
-->
