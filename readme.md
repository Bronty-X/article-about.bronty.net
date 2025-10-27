# Aritcle Store
about.bronty.netの記事データ保管用リポジトリです。Nuxt Contentによって参照されます。

## 記事のフォーマット
メタデータ
```md
---
title: めっちゃイカしたシステムについて
created-at: 2025-01-01
updated-at: 2025-01-01
tags: nuxt,node,javascript
---
# Foo

This is Foo blog post.
```
|パラメーター名|備考|
|--|--|
|title|タイトル|
|created-at|作成日 CD/CIパイプラインで自動化するかも（したい）|
|updated-at|最終更新日 自動化したい|
|tags|記事のタグ カンマ区切り|

## ディレクトリ構成
```
-|tags/ タグ
-|works/ ポートフォリオ記事格納用
```

## 今後の展望
- CD/CIパイプラインを構築し、CloudFlareへのビルド命令と一部メタデータの生成を自動化する。
- 記事公開日,公開可否の実装
