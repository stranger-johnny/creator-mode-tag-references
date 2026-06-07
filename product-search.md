# 商品検索結果

公式リファレンス: https://reference.makeshop.jp/creator-mode/contents/search/index.html

⚠️ 推測サンプル: 公式リファレンス上でサンプルコードが確認できないタグは、タグ名と概要から使用例を推測して補完しています。

# 検索情報

## $search.keyword

### 概要
検索したキーワード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.keyword}></p>
```

#### HTML変換後
```html
<p>検索したキーワード</p>
```

## $search.name

### 概要
検索した商品名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.name}></p>
```

#### HTML変換後
```html
<p>検索した商品名</p>
```

## $search.category.code

### 概要
検索したカテゴリー識別コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.category.code}></p>
```

#### HTML変換後
```html
<p>検索したカテゴリー識別コード</p>
```

## $search.price_low

### 概要
検索した価格帯（低）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.price_low}></p>
```

#### HTML変換後
```html
<p>検索した価格帯（低）</p>
```

## $search.price_high

### 概要
検索した価格帯（高）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.price_high}></p>
```

#### HTML変換後
```html
<p>検索した価格帯（高）</p>
```

## $search.total_count

### 概要
総商品数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.total_count}></p>
```

#### HTML変換後
```html
<p>総商品数</p>
```

## $search.display_count

### 概要
表示商品数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.display_count}></p>
```

#### HTML変換後
```html
<p>表示商品数</p>
```

## $search.original_code

### 概要
検索した独自商品コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.original_code}></p>
```

#### HTML変換後
```html
<p>検索した独自商品コード</p>
```

## $search.display_count_from

### 概要
ページ内最小表示商品数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.display_count_from}></p>
```

#### HTML変換後
```html
<p>ページ内最小表示商品数</p>
```

## $search.display_count_to

### 概要
ページ内最大表示商品数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.display_count_to}></p>
```

#### HTML変換後
```html
<p>ページ内最大表示商品数</p>
```

# パンくず

## $search.breadcrumb_list.list[i].name

### 概要
ページ名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.breadcrumb_list.list[i].name}></p>
```

#### HTML変換後
```html
<p>ページ名</p>
```

## $search.breadcrumb_list.list[i].url

### 概要
ページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.breadcrumb_list.list[i].url}></p>
```

#### HTML変換後
```html
<p>ページURL</p>
```

## $search.breadcrumb_list.list[i].is_current

### 概要
現在地かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.breadcrumb_list.list[i].is_current}></p>
```

#### HTML変換後
```html
<!-- $search.breadcrumb_list.list[i].is_current: true / false -->
```

# 並び替え

## $search.sort_recommend_url

### 概要
並び替えURL（おすすめ順）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.sort_recommend_url}></p>
```

#### HTML変換後
```html
<p>並び替えURL（おすすめ順）</p>
```

## $search.sort_new_url

### 概要
並び替えURL（新着順）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.sort_new_url}></p>
```

#### HTML変換後
```html
<p>並び替えURL（新着順）</p>
```

## $search.sort_high_price_url

### 概要
並び替えURL（価格が高い順）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.sort_high_price_url}></p>
```

#### HTML変換後
```html
<p>並び替えURL（価格が高い順）</p>
```

## $search.sort_low_price_url

### 概要
並び替えURL（価格が低い順）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.sort_low_price_url}></p>
```

#### HTML変換後
```html
<p>並び替えURL（価格が低い順）</p>
```

## $search.is_sort_recommend_selected

### 概要
おすすめ順かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.is_sort_recommend_selected}></p>
```

#### HTML変換後
```html
<!-- $search.is_sort_recommend_selected: true / false -->
```

## $search.is_sort_new_selected

### 概要
新着順かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.is_sort_new_selected}></p>
```

#### HTML変換後
```html
<!-- $search.is_sort_new_selected: true / false -->
```

## $search.sort_name_url

### 概要
並び替えURL（商品名順）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.sort_name_url}></p>
```

#### HTML変換後
```html
<p>並び替えURL（商品名順）</p>
```

## $search.is_sort_name_selected

### 概要
商品名順かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.is_sort_name_selected}></p>
```

#### HTML変換後
```html
<!-- $search.is_sort_name_selected: true / false -->
```

## $search.sort_manufacturer_url

### 概要
並び替えURL（製造元順）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.sort_manufacturer_url}></p>
```

#### HTML変換後
```html
<p>並び替えURL（製造元順）</p>
```

## $search.is_sort_manufacturer_selected

### 概要
並び順が製造元順かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.is_sort_manufacturer_selected}></p>
```

#### HTML変換後
```html
<!-- $search.is_sort_manufacturer_selected: true / false -->
```

## $search.is_sort_high_price_selected

### 概要
高価格順かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.is_sort_high_price_selected}></p>
```

#### HTML変換後
```html
<!-- $search.is_sort_high_price_selected: true / false -->
```

## $search.is_sort_low_price_selected

### 概要
低価格順かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.is_sort_low_price_selected}></p>
```

#### HTML変換後
```html
<!-- $search.is_sort_low_price_selected: true / false -->
```

# 検索結果一覧

## $search.item.has_item

### 概要
検索結果にあてはまる商品があるかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.has_item}></p>
```

#### HTML変換後
```html
<!-- $search.item.has_item: true / false -->
```

## $search.item.list[i].num

### 概要
番号

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].num}></p>
```

#### HTML変換後
```html
<p>番号</p>
```

## $search.item.list[i].name

### 概要
商品名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].name}></p>
```

#### HTML変換後
```html
<p>商品名</p>
```

## $search.item.list[i].price

### 概要
販売価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].price}></p>
```

#### HTML変換後
```html
<p>販売価格</p>
```

## $search.item.list[i].price_excluded_tax

### 概要
税抜き価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き価格</p>
```

## $search.item.list[i].tax

### 概要
税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].tax}></p>
```

#### HTML変換後
```html
<p>税</p>
```

## $search.item.list[i].tax_rate

### 概要
消費税率

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].tax_rate}></p>
```

#### HTML変換後
```html
<p>消費税率</p>
```

## $search.item.list[i].is_reduced_tax_rate

### 概要
軽減税率対象商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_reduced_tax_rate}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_reduced_tax_rate: true / false -->
```

## $search.item.list[i].fixed_price

### 概要
定価

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].fixed_price}></p>
```

#### HTML変換後
```html
<p>定価</p>
```

## $search.item.list[i].original_price

### 概要
通常価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].original_price}></p>
```

#### HTML変換後
```html
<p>通常価格</p>
```

## $search.item.list[i].original_price_excluded_tax

### 概要
税抜き通常価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].original_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き通常価格</p>
```

## $search.item.list[i].original_tax

### 概要
通常価格の税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].original_tax}></p>
```

#### HTML変換後
```html
<p>通常価格の税</p>
```

## $search.item.list[i].url

### 概要
商品URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].url}></p>
```

#### HTML変換後
```html
<p>商品URL</p>
```

## $search.item.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].image_S}></p>
```

#### HTML変換後
```html
<p>商品縮小画像URL</p>
```

## $search.item.list[i].image_M

### 概要
商品普通画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].image_M}></p>
```

#### HTML変換後
```html
<p>商品普通画像URL</p>
```

## $search.item.list[i].image_L

### 概要
商品画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].image_L}></p>
```

#### HTML変換後
```html
<p>商品画像URL</p>
```

## $search.item.list[i].is_stock_display

### 概要
在庫表示可かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_stock_display}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_stock_display: true / false -->
```

## $search.item.list[i].is_stock_unlimited

### 概要
在庫無制限かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_stock_unlimited}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_stock_unlimited: true / false -->
```

## $search.item.list[i].is_soldout

### 概要
売り切れかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_soldout}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_soldout: true / false -->
```

## $search.item.list[i].is_small_stock

### 概要
在庫が指定された数以下かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_small_stock}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_small_stock: true / false -->
```

## $search.item.list[i].stock_quantity

### 概要
在庫数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## $search.item.list[i].is_sale

### 概要
セール商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_sale}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_sale: true / false -->
```

## $search.item.list[i].sale_rate

### 概要
割引率

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].sale_rate}></p>
```

#### HTML変換後
```html
<p>割引率</p>
```

## $search.item.list[i].has_review

### 概要
旧レビューが投稿されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].has_review}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].has_review: true / false -->
```

## $search.item.list[i].review.star_html

### 概要
旧レビュー評価（星）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].review.star_html}></p>
```

#### HTML変換後
```html
<p>旧レビュー評価（星）</p>
```

## $search.item.list[i].review.average

### 概要
平均旧レビュー点数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].review.average}></p>
```

#### HTML変換後
```html
<p>平均旧レビュー点数</p>
```

## $search.item.list[i].review.total_count

### 概要
旧レビュー投稿数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].review.total_count}></p>
```

#### HTML変換後
```html
<p>旧レビュー投稿数</p>
```

## $search.item.list[i].review.url

### 概要
旧レビュー一覧URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].review.url}></p>
```

#### HTML変換後
```html
<p>旧レビュー一覧URL</p>
```

## $search.item.list[i].child_category.has_item

### 概要
サブカテゴリーを持っているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].child_category.has_item}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].child_category.has_item: true / false -->
```

## $search.item.list[i].original_code

### 概要
独自商品コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].original_code}></p>
```

#### HTML変換後
```html
<p>独自商品コード</p>
```

## $search.item.list[i].system_code

### 概要
システム商品コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## $search.item.list[i].point

### 概要
獲得ポイント

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $search.item.list[i].is_member_price

### 概要
会員割引商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_member_price}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_member_price: true / false -->
```

## $search.item.list[i].base_category.name

### 概要
カテゴリー名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].base_category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $search.item.list[i].base_category.url

### 概要
カテゴリーURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].base_category.url}></p>
```

#### HTML変換後
```html
<p>カテゴリーURL</p>
```

## $search.item.list[i].base_category.code

### 概要
カテゴリー識別コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].base_category.code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $search.item.list[i].description

### 概要
商品説明文

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].description}></p>
```

#### HTML変換後
```html
<p>商品説明文</p>
```

## $search.item.list[i].manufacturer

### 概要
製造元

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].manufacturer}></p>
```

#### HTML変換後
```html
<p>製造元</p>
```

## $search.item.list[i].origin_country

### 概要
原産地

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].origin_country}></p>
```

#### HTML変換後
```html
<p>原産地</p>
```

## $search.item.list[i].special_display

### 概要
商品別特殊表示

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## $search.item.list[i].is_reservation_sale

### 概要
予約販売商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_reservation_sale}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_reservation_sale: true / false -->
```

## $search.item.list[i].reservation_sale_note

### 概要
備考

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].reservation_sale_note}></p>
```

#### HTML変換後
```html
<p>備考</p>
```

## $search.item.list[i].has_release_date

### 概要
発売日が設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].has_release_date}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].has_release_date: true / false -->
```

## $search.item.list[i].is_released

### 概要
発売済みかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_released}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_released: true / false -->
```

## $search.item.list[i].release_date.year

### 概要
発売日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].release_date.year}></p>
```

#### HTML変換後
```html
<p>発売日時（年）</p>
```

## $search.item.list[i].release_date.month

### 概要
発売日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].release_date.month}></p>
```

#### HTML変換後
```html
<p>発売日時（月）</p>
```

## $search.item.list[i].release_date.day

### 概要
発売日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].release_date.day}></p>
```

#### HTML変換後
```html
<p>発売日時（日）</p>
```

## $search.item.list[i].release_date_note

### 概要
発売日備考

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].release_date_note}></p>
```

#### HTML変換後
```html
<p>発売日備考</p>
```

## $search.item.list[i].has_option

### 概要
オプションが設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].has_option}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].has_option: true / false -->
```

## $search.item.list[i].is_favorite

### 概要
お気に入りに追加済みかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_favorite}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_favorite: true / false -->
```

## $search.item.list[i].favorite_entry_url

### 概要
お気に入りに追加URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].favorite_entry_url}></p>
```

#### HTML変換後
```html
<p>お気に入りに追加URL</p>
```

## $search.item.list[i].favorite_remove_url

### 概要
お気に入りから削除URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].favorite_remove_url}></p>
```

#### HTML変換後
```html
<p>お気に入りから削除URL</p>
```

## $search.item.list[i].cart_entry_url

### 概要
かごに入れるURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].cart_entry_url}></p>
```

#### HTML変換後
```html
<p>かごに入れるURL</p>
```

## $search.item.list[i].icon.has_item

### 概要
アイコンが設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].icon.has_item}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].icon.has_item: true / false -->
```

## $search.item.list[i].icon.list[j].image_url

### 概要
アイコン画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].icon.list[j].image_url}></p>
```

#### HTML変換後
```html
<p>アイコン画像URL</p>
```

## $search.item.list[i].is_bulk

### 概要
まとめ買い割引商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].is_bulk}></p>
```

#### HTML変換後
```html
<!-- $search.item.list[i].is_bulk: true / false -->
```

## $search.item.list[i].bulk_url

### 概要
まとめ買い割引商品一覧のURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].bulk_url}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引商品一覧のURL</p>
```

## $search.item.list[i].bulk_name

### 概要
まとめ買い割引の名前

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.item.list[i].bulk_name}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の名前</p>
```

# ページャー

## $search.pager.is_first

### 概要
表示中のページが最初のページかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.is_first}></p>
```

#### HTML変換後
```html
<!-- $search.pager.is_first: true / false -->
```

## $search.pager.is_first_display

### 概要
最初のページ番号が表示されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.is_first_display}></p>
```

#### HTML変換後
```html
<!-- $search.pager.is_first_display: true / false -->
```

## $search.pager.first_url

### 概要
最初のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.first_url}></p>
```

#### HTML変換後
```html
<p>最初のページURL</p>
```

## $search.pager.prev_url

### 概要
前のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.prev_url}></p>
```

#### HTML変換後
```html
<p>前のページURL</p>
```

## $search.pager.is_last

### 概要
表示中のページが最後のページかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.is_last}></p>
```

#### HTML変換後
```html
<!-- $search.pager.is_last: true / false -->
```

## $search.pager.is_last_display

### 概要
最後のページ番号が表示されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.is_last_display}></p>
```

#### HTML変換後
```html
<!-- $search.pager.is_last_display: true / false -->
```

## $search.pager.last_url

### 概要
最後のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.last_url}></p>
```

#### HTML変換後
```html
<p>最後のページURL</p>
```

## $search.pager.last_number

### 概要
最終ページ数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.last_number}></p>
```

#### HTML変換後
```html
<p>最終ページ数</p>
```

## $search.pager.next_url

### 概要
次のページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.next_url}></p>
```

#### HTML変換後
```html
<p>次のページURL</p>
```

## $search.pager.list[i].number

### 概要
ページ番号

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.list[i].number}></p>
```

#### HTML変換後
```html
<p>ページ番号</p>
```

## $search.pager.list[i].url

### 概要
ページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$search.pager.list[i].url}></p>
```

#### HTML変換後
```html
<p>ページURL</p>
```
