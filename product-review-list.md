# 商品レビュー一覧

公式リファレンス: https://reference.makeshop.jp/creator-mode/contents/review-list/index.html

⚠️ 推測サンプル: 公式リファレンス上でサンプルコードが確認できないタグは、タグ名と概要から使用例を推測して補完しています。

# 商品情報

## $item.name

### 概要
商品名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name}></p>
```

#### HTML変換後
```html
<p>商品名</p>
```

## $item.url

### 概要
商品URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.url}></p>
```

#### HTML変換後
```html
<p>商品URL</p>
```

## $item.image_S

### 概要
商品縮小画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.image_S}></p>
```

#### HTML変換後
```html
<p>商品縮小画像URL</p>
```

## $item.image_M

### 概要
商品普通画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.image_M}></p>
```

#### HTML変換後
```html
<p>商品普通画像URL</p>
```

## $item.image_L

### 概要
商品画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.image_L}></p>
```

#### HTML変換後
```html
<p>商品画像URL</p>
```

## $item.base_category.name

### 概要
カテゴリー名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.base_category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $item.base_category.url

### 概要
カテゴリーURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.base_category.url}></p>
```

#### HTML変換後
```html
<p>カテゴリーURL</p>
```

## $review.star_html

### 概要
レビュー評価（星）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.star_html}></p>
```

#### HTML変換後
```html
<p>レビュー評価（星）</p>
```

## $review.average

### 概要
平均レビュー点数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.average}></p>
```

#### HTML変換後
```html
<p>平均レビュー点数</p>
```

## $review.total_count

### 概要
レビュー総投稿件数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.total_count}></p>
```

#### HTML変換後
```html
<p>レビュー総投稿件数</p>
```

## $review.display_count

### 概要
レビュー表示件数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.display_count}></p>
```

#### HTML変換後
```html
<p>レビュー表示件数</p>
```

## $review.post_url

### 概要
レビュー投稿URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.post_url}></p>
```

#### HTML変換後
```html
<p>レビュー投稿URL</p>
```

# レビュー一覧

## $review.has_item

### 概要
レビューが投稿されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.has_item}></p>
```

#### HTML変換後
```html
<!-- $review.has_item: true / false -->
```

## $review.list[i].reviewer_name

### 概要
投稿者名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].reviewer_name}></p>
```

#### HTML変換後
```html
<p>投稿者名</p>
```

## $review.list[i].star_html

### 概要
レビュー評価（星）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].star_html}></p>
```

#### HTML変換後
```html
<p>レビュー評価（星）</p>
```

## $review.list[i].score

### 概要
レビュー点数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].score}></p>
```

#### HTML変換後
```html
<p>レビュー点数</p>
```

## $review.list[i].content

### 概要
レビュー内容

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].content}></p>
```

#### HTML変換後
```html
<p>レビュー内容</p>
```

## $review.list[i].date.year

### 概要
投稿日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].date.year}></p>
```

#### HTML変換後
```html
<p>投稿日時（年）</p>
```

## $review.list[i].date.month

### 概要
投稿日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].date.month}></p>
```

#### HTML変換後
```html
<p>投稿日時（月）</p>
```

## $review.list[i].date.day

### 概要
投稿日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].date.day}></p>
```

#### HTML変換後
```html
<p>投稿日時（日）</p>
```

## $review.list[i].date.hour

### 概要
投稿日時（時）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].date.hour}></p>
```

#### HTML変換後
```html
<p>投稿日時（時）</p>
```

## $review.list[i].date.minute

### 概要
投稿日時（分）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.list[i].date.minute}></p>
```

#### HTML変換後
```html
<p>投稿日時（分）</p>
```

# ページャー

## $review.pager.is_first

### 概要
表示中のページが最初のページかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.is_first}></p>
```

#### HTML変換後
```html
<!-- $review.pager.is_first: true / false -->
```

## $review.pager.first_url

### 概要
最初のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.first_url}></p>
```

#### HTML変換後
```html
<p>最初のページURL</p>
```

## $review.pager.prev_url

### 概要
前のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.prev_url}></p>
```

#### HTML変換後
```html
<p>前のページURL</p>
```

## $review.pager.is_last

### 概要
表示中のページが最後のページかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.is_last}></p>
```

#### HTML変換後
```html
<!-- $review.pager.is_last: true / false -->
```

## $review.pager.last_url

### 概要
最後のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.last_url}></p>
```

#### HTML変換後
```html
<p>最後のページURL</p>
```

## $review.pager.last_number

### 概要
最終ページ数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.last_number}></p>
```

#### HTML変換後
```html
<p>最終ページ数</p>
```

## $review.pager.next_url

### 概要
次のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.next_url}></p>
```

#### HTML変換後
```html
<p>次のページURL</p>
```

## $review.pager.list[i].number

### 概要
ページ番号

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.list[i].number}></p>
```

#### HTML変換後
```html
<p>ページ番号</p>
```

## $review.pager.list[i].url

### 概要
ページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$review.pager.list[i].url}></p>
```

#### HTML変換後
```html
<p>ページURL</p>
```
