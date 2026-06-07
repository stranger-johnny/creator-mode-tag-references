# システムタグ

## $makeshop.head

### 概要
headタグ内に必ず記載

### サンプルコード

#### クリエーターモード
```php
<head>
    <{$makeshop.head}>
</head>
```

#### HTML変換後
```html
<head>
    <!-- 事前に定義したheadタグが出力 -->
</head>
```

## $makeshop.body_top

### 概要
body開始タグ直後に必ず記載

### サンプルコード

#### クリエーターモード
```php
<body>
    <{$makeshop.body_top}>
</body>
```

#### HTML変換後
```html
<head>
    <!-- 事前に定義したbodyタグ上部の定義が出力 -->
</head>
```

## $makeshop.body_top

### 概要
body終了タグ直前に必ず記載

### サンプルコード

#### クリエーターモード
```php
<body>
    <{$makeshop.body_bottom}>
</body>
```

#### HTML変換後
```html
<head>
    <!-- 事前に定義したbodyタグ下部の定義が出力 -->
</head>
```

# ページ情報

## $page.type

### 概要
ページタイプ。ページタイプの一覧は以下の通り。

- トップページ：top
- 商品カテゴリー：category
- 商品検索結果：search
- 商品詳細：item
- 商品レビュー一覧：review-list
- 商品レビュー投稿：review-post
- 買い物カゴ：cart
- お知らせ一覧：news-list
- お知らせ詳細：news-detail
- まとめ買い割引：bulk
- 利用案内：guide
- 会社概要：company
- 特定商取引法：contract
- 会員制/年齢確認：verification
- カタログ：catalog
- プライバシーポリシー：policy

### サンプルコード

#### クリエーターモード
```php
<div class="<{$page.type}>">～</div>
```

#### HTML変換後
```html
<div class="category">～</div>
```
