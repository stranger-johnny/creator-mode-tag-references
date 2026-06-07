# 商品詳細

公式リファレンス: https://reference.makeshop.jp/creator-mode/contents/detail/index.html

⚠️ 推測サンプル: 公式リファレンス上でサンプルコードが確認できないタグは、タグ名と概要から使用例を推測して補完しています。
商品一覧系タグは `$item.group` のあとに `.list[i]` をつけて使用します。例: `$item.group.list[i].name`

# パンくず

## $item.breadcrumb_list_group.has_item

### 概要
パンくずリストが複数あるかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.breadcrumb_list_group.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.breadcrumb_list_group.has_item: true / false -->
```

## $item.breadcrumb_list_group.list[i].list[j].name

### 概要
ページ名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.breadcrumb_list_group.list[i].list[j].name}></p>
```

#### HTML変換後
```html
<p>ページ名</p>
```

## $item.breadcrumb_list_group.list[i].list[j].url

### 概要
ページURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.breadcrumb_list_group.list[i].list[j].url}></p>
```

#### HTML変換後
```html
<p>ページURL</p>
```

## $item.breadcrumb_list_group.list[i].is_base_category

### 概要
パンくずリストが基本カテゴリーかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.breadcrumb_list_group.list[i].is_base_category}></p>
```

#### HTML変換後
```html
<!-- $item.breadcrumb_list_group.list[i].is_base_category: true / false -->
```

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

## $item.base_category.code

### 概要
カテゴリー識別コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.base_category.code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $item.original_code

### 概要
独自商品コード（初期設定は非表示）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.original_code}></p>
```

#### HTML変換後
```html
<p>独自商品コード（初期設定は非表示）</p>
```

## $item.system_code

### 概要
システム商品コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## $item.point_html

### 概要
獲得ポイント

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.point_html}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $item.point

### 概要
獲得ポイント（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント（値のみ・金額連動なし）</p>
```

## $item.description

### 概要
商品説明

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.description}></p>
```

#### HTML変換後
```html
<p>商品説明</p>
```

## $item.description2

### 概要
商品説明2

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.description2}></p>
```

#### HTML変換後
```html
<p>商品説明2</p>
```

## $item.description3

### 概要
商品説明3

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.description3}></p>
```

#### HTML変換後
```html
<p>商品説明3</p>
```

## $item.description4

### 概要
商品説明4

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.description4}></p>
```

#### HTML変換後
```html
<p>商品説明4</p>
```

## $item.manufacturer

### 概要
製造元

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.manufacturer}></p>
```

#### HTML変換後
```html
<p>製造元</p>
```

## $item.origin_country

### 概要
原産地

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.origin_country}></p>
```

#### HTML変換後
```html
<p>原産地</p>
```

## $item.special_display

### 概要
商品別特殊表示

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## $item.quantity_id

### 概要
数量入力フォーム用データID

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<div><{$item.quantity_id}></div>
```

#### HTML変換後
```html
<!-- $item.quantity_id: 数量入力フォーム用データID -->
```

## $item.is_sell_start

### 概要
販売開始日時が設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_sell_start}></p>
```

#### HTML変換後
```html
<!-- $item.is_sell_start: true / false -->
```

## $item.sell_start.year

### 概要
販売開始日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_start.year}></p>
```

#### HTML変換後
```html
<p>販売開始日時（年）</p>
```

## $item.sell_start.month

### 概要
販売開始日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_start.month}></p>
```

#### HTML変換後
```html
<p>販売開始日時（月）</p>
```

## $item.sell_start.day

### 概要
販売開始日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_start.day}></p>
```

#### HTML変換後
```html
<p>販売開始日時（日）</p>
```

## $item.sell_start.hour

### 概要
販売開始日時（時）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_start.hour}></p>
```

#### HTML変換後
```html
<p>販売開始日時（時）</p>
```

## $item.sell_start.minute

### 概要
販売開始日時（分）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_start.minute}></p>
```

#### HTML変換後
```html
<p>販売開始日時（分）</p>
```

## $item.is_sell_end

### 概要
販売終了日時が設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_sell_end}></p>
```

#### HTML変換後
```html
<!-- $item.is_sell_end: true / false -->
```

## $item.sell_end.year

### 概要
販売終了日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_end.year}></p>
```

#### HTML変換後
```html
<p>販売終了日時（年）</p>
```

## $item.sell_end.month

### 概要
販売終了日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_end.month}></p>
```

#### HTML変換後
```html
<p>販売終了日時（月）</p>
```

## $item.sell_end.day

### 概要
販売終了日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_end.day}></p>
```

#### HTML変換後
```html
<p>販売終了日時（日）</p>
```

## $item.sell_end.hour

### 概要
販売終了日時（時）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_end.hour}></p>
```

#### HTML変換後
```html
<p>販売終了日時（時）</p>
```

## $item.sell_end.minute

### 概要
販売終了日時（分）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sell_end.minute}></p>
```

#### HTML変換後
```html
<p>販売終了日時（分）</p>
```

## $item.is_within_sell_period

### 概要
販売期間中かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_within_sell_period}></p>
```

#### HTML変換後
```html
<!-- $item.is_within_sell_period: true / false -->
```

## $item.order_quantity_min

### 概要
最小注文限度

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.order_quantity_min}></p>
```

#### HTML変換後
```html
<p>最小注文限度</p>
```

## $item.order_quantity_max

### 概要
最大注文限度

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.order_quantity_max}></p>
```

#### HTML変換後
```html
<p>最大注文限度</p>
```

## $item.contact_url

### 概要
商品に対するお問い合わせURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.contact_url}></p>
```

#### HTML変換後
```html
<p>商品に対するお問い合わせURL</p>
```

## $item.icon.has_item

### 概要
アイコンが設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.icon.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.icon.has_item: true / false -->
```

## $item.icon.list[i].image_url

### 概要
アイコン画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.icon.list[i].image_url}></p>
```

#### HTML変換後
```html
<p>アイコン画像URL</p>
```

# 価格

## $item.price_html

### 概要
販売価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.price_html}></p>
```

#### HTML変換後
```html
<p>販売価格</p>
```

## $item.price

### 概要
販売価格（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.price}></p>
```

#### HTML変換後
```html
<p>販売価格（値のみ・金額連動なし）</p>
```

## $item.original_price

### 概要
通常価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.original_price}></p>
```

#### HTML変換後
```html
<p>通常価格</p>
```

## $item.original_price_excluded_tax

### 概要
税抜き通常価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.original_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き通常価格</p>
```

## $item.original_tax

### 概要
通常価格の税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.original_tax}></p>
```

#### HTML変換後
```html
<p>通常価格の税</p>
```

## $item.fixed_price

### 概要
定価

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.fixed_price}></p>
```

#### HTML変換後
```html
<p>定価</p>
```

## $item.fixed_price_name

### 概要
定価名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.fixed_price_name}></p>
```

#### HTML変換後
```html
<p>定価名</p>
```

## $item.price_excluded_tax_html

### 概要
税抜き価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.price_excluded_tax_html}></p>
```

#### HTML変換後
```html
<p>税抜き価格</p>
```

## $item.price_excluded_tax

### 概要
税抜き価格（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き価格（値のみ・金額連動なし）</p>
```

## $item.tax_html

### 概要
税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.tax_html}></p>
```

#### HTML変換後
```html
<p>税</p>
```

## $item.tax

### 概要
税（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.tax}></p>
```

#### HTML変換後
```html
<p>税（値のみ・金額連動なし）</p>
```

## $item.tax_rate

### 概要
消費税率

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.tax_rate}></p>
```

#### HTML変換後
```html
<p>消費税率</p>
```

## $item.is_reduced_tax_rate

### 概要
軽減税率対象商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_reduced_tax_rate}></p>
```

#### HTML変換後
```html
<!-- $item.is_reduced_tax_rate: true / false -->
```

## $item.is_member_price

### 概要
会員専用価格かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_member_price}></p>
```

#### HTML変換後
```html
<!-- $item.is_member_price: true / false -->
```

# 商品画像

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

# 複数商品画像

## $item.multi_image.has_item

### 概要
複数商品画像が登録されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.multi_image.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.multi_image.has_item: true / false -->
```

## $item.multi_image.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.multi_image.list[i].image_S}></p>
```

#### HTML変換後
```html
<p>商品縮小画像URL</p>
```

## $item.multi_image.list[i].image_L

### 概要
商品画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.multi_image.list[i].image_L}></p>
```

#### HTML変換後
```html
<p>商品画像URL</p>
```

# 追加商品画像

## $item.add_image.has_item

### 概要
追加商品画像が登録されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.add_image.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.add_image.has_item: true / false -->
```

## $item.add_image.list[i].image_url

### 概要
追加商品画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.add_image.list[i].image_url}></p>
```

#### HTML変換後
```html
<p>追加商品画像URL</p>
```

## $item.add_image.list[i].description

### 概要
追加商品画像説明文

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.add_image.list[i].description}></p>
```

#### HTML変換後
```html
<p>追加商品画像説明文</p>
```

# セール

## $item.is_sale

### 概要
セール商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_sale}></p>
```

#### HTML変換後
```html
<!-- $item.is_sale: true / false -->
```

## $item.sale_rate

### 概要
割引率

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_rate}></p>
```

#### HTML変換後
```html
<p>割引率</p>
```

## $item.has_sale_period

### 概要
セール期間が設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.has_sale_period}></p>
```

#### HTML変換後
```html
<!-- $item.has_sale_period: true / false -->
```

## $item.sale_start.year

### 概要
セール開始日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_start.year}></p>
```

#### HTML変換後
```html
<p>セール開始日時（年）</p>
```

## $item.sale_start.month

### 概要
セール開始日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_start.month}></p>
```

#### HTML変換後
```html
<p>セール開始日時（月）</p>
```

## $item.sale_start.day

### 概要
セール開始日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_start.day}></p>
```

#### HTML変換後
```html
<p>セール開始日時（日）</p>
```

## $item.sale_start.hour

### 概要
セール開始日時（時）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_start.hour}></p>
```

#### HTML変換後
```html
<p>セール開始日時（時）</p>
```

## $item.sale_start.minute

### 概要
セール開始日時（分）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_start.minute}></p>
```

#### HTML変換後
```html
<p>セール開始日時（分）</p>
```

## $item.sale_end.year

### 概要
セール終了日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_end.year}></p>
```

#### HTML変換後
```html
<p>セール終了日時（年）</p>
```

## $item.sale_end.month

### 概要
セール終了日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_end.month}></p>
```

#### HTML変換後
```html
<p>セール終了日時（月）</p>
```

## $item.sale_end.day

### 概要
セール終了日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_end.day}></p>
```

#### HTML変換後
```html
<p>セール終了日時（日）</p>
```

## $item.sale_end.hour

### 概要
セール終了日時（時）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_end.hour}></p>
```

#### HTML変換後
```html
<p>セール終了日時（時）</p>
```

## $item.sale_end.minute

### 概要
セール終了日時（分）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sale_end.minute}></p>
```

#### HTML変換後
```html
<p>セール終了日時（分）</p>
```

# バリエーション

## $item.has_option

### 概要
バリエーションが設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.has_option}></p>
```

#### HTML変換後
```html
<!-- $item.has_option: true / false -->
```

## $item.option_html

### 概要
バリエーション・カスタムセレクトまたはオプショングループ

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_html}></p>
```

#### HTML変換後
```html
<p>バリエーション・カスタムセレクトまたはオプショングループ</p>
```

# 送料

## $item.is_delivery_price_display

### 概要
送料が設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_delivery_price_display}></p>
```

#### HTML変換後
```html
<!-- $item.is_delivery_price_display: true / false -->
```

## $item.delivery_price

### 概要
送料

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.delivery_price}></p>
```

#### HTML変換後
```html
<p>送料</p>
```

## $item.is_delivery_price_message_display

### 概要
配送料の表示タイプに固定テキストがあるかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_delivery_price_message_display}></p>
```

#### HTML変換後
```html
<!-- $item.is_delivery_price_message_display: true / false -->
```

## $item.delivery_price_message

### 概要
配送料の表示タイプの固定テキスト

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.delivery_price_message}></p>
```

#### HTML変換後
```html
<p>配送料の表示タイプの固定テキスト</p>
```

## $item.is_member_delivery_price_display

### 概要
会員グループ別送料があるかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_member_delivery_price_display}></p>
```

#### HTML変換後
```html
<!-- $item.is_member_delivery_price_display: true / false -->
```

## $item.member_delivery_price

### 概要
会員グループ別送料

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.member_delivery_price}></p>
```

#### HTML変換後
```html
<p>会員グループ別送料</p>
```

# 在庫

## $item.is_stock_display

### 概要
在庫表示可かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_stock_display}></p>
```

#### HTML変換後
```html
<!-- $item.is_stock_display: true / false -->
```

## $item.is_stock_unlimited

### 概要
在庫無制限かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_stock_unlimited}></p>
```

#### HTML変換後
```html
<!-- $item.is_stock_unlimited: true / false -->
```

## $item.is_soldout

### 概要
売り切れかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_soldout}></p>
```

#### HTML変換後
```html
<!-- $item.is_soldout: true / false -->
```

## $item.is_small_stock

### 概要
在庫が指定された数以下かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_small_stock}></p>
```

#### HTML変換後
```html
<!-- $item.is_small_stock: true / false -->
```

## $item.small_stock_quantity

### 概要
指定された在庫数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.small_stock_quantity}></p>
```

#### HTML変換後
```html
<p>指定された在庫数</p>
```

## $item.stock_quantity

### 概要
在庫数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## $item.is_restock_enabled

### 概要
再入荷お知らせが利用可能な商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_restock_enabled}></p>
```

#### HTML変換後
```html
<!-- $item.is_restock_enabled: true / false -->
```

## $item.restock_url

### 概要
再入荷お知らせURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.restock_url}></p>
```

#### HTML変換後
```html
<p>再入荷お知らせURL</p>
```

# かごに入れる

## $item.cart_entry_url

### 概要
かごに入れるURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.cart_entry_url}></p>
```

#### HTML変換後
```html
<p>かごに入れるURL</p>
```

# お気に入りに追加

## $item.is_favorite

### 概要
お気に入りに追加済みかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_favorite}></p>
```

#### HTML変換後
```html
<!-- $item.is_favorite: true / false -->
```

## $item.favorite_entry_url

### 概要
お気に入りに追加URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.favorite_entry_url}></p>
```

#### HTML変換後
```html
<p>お気に入りに追加URL</p>
```

## $item.favorite_remove_url

### 概要
お気に入りから削除URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.favorite_remove_url}></p>
```

#### HTML変換後
```html
<p>お気に入りから削除URL</p>
```

# 旧レビュー

## $item.review.is_enabled

### 概要
旧レビュー機能が有効かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.is_enabled}></p>
```

#### HTML変換後
```html
<!-- $item.review.is_enabled: true / false -->
```

## $item.review.has_item

### 概要
旧レビューが投稿されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.review.has_item: true / false -->
```

## $item.review.star_html

### 概要
旧レビュー評価（星）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.star_html}></p>
```

#### HTML変換後
```html
<p>旧レビュー評価（星）</p>
```

## $item.review.average

### 概要
平均旧レビュー点数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.average}></p>
```

#### HTML変換後
```html
<p>平均旧レビュー点数</p>
```

## $item.review.total_count

### 概要
旧レビュー投稿数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.total_count}></p>
```

#### HTML変換後
```html
<p>旧レビュー投稿数</p>
```

## $item.review.list_url

### 概要
旧レビュー一覧URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list_url}></p>
```

#### HTML変換後
```html
<p>旧レビュー一覧URL</p>
```

## $item.review.post_url

### 概要
旧レビュー投稿URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.post_url}></p>
```

#### HTML変換後
```html
<p>旧レビュー投稿URL</p>
```

## $item.review.list[i].reviewer_name

### 概要
投稿者名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].reviewer_name}></p>
```

#### HTML変換後
```html
<p>投稿者名</p>
```

## $item.review.list[i].star_html

### 概要
旧レビュー評価（星）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].star_html}></p>
```

#### HTML変換後
```html
<p>旧レビュー評価（星）</p>
```

## $item.review.list[i].score

### 概要
旧レビュー点数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].score}></p>
```

#### HTML変換後
```html
<p>旧レビュー点数</p>
```

## $item.review.list[i].content

### 概要
旧レビュー内容

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].content}></p>
```

#### HTML変換後
```html
<p>旧レビュー内容</p>
```

## $item.review.list[i].date.year

### 概要
投稿日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].date.year}></p>
```

#### HTML変換後
```html
<p>投稿日時（年）</p>
```

## $item.review.list[i].date.month

### 概要
投稿日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].date.month}></p>
```

#### HTML変換後
```html
<p>投稿日時（月）</p>
```

## $item.review.list[i].date.day

### 概要
投稿日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].date.day}></p>
```

#### HTML変換後
```html
<p>投稿日時（日）</p>
```

## $item.review.list[i].date.hour

### 概要
投稿日時（時）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].date.hour}></p>
```

#### HTML変換後
```html
<p>投稿日時（時）</p>
```

## $item.review.list[i].date.minute

### 概要
投稿日時（分）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.review.list[i].date.minute}></p>
```

#### HTML変換後
```html
<p>投稿日時（分）</p>
```

# SNSシェア

## $item.sns.twitter

### 概要
Twitterボタン

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sns.twitter}></p>
```

#### HTML変換後
```html
<p>Twitterボタン</p>
```

## $item.sns.facebook

### 概要
Facebookボタン

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sns.facebook}></p>
```

#### HTML変換後
```html
<p>Facebookボタン</p>
```

## $item.sns.line

### 概要
LINEボタン

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.sns.line}></p>
```

#### HTML変換後
```html
<p>LINEボタン</p>
```

# 定期購入

## $item.cart_entry_subscription_url

### 概要
定期購入商品をかごに入れるURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.cart_entry_subscription_url}></p>
```

#### HTML変換後
```html
<p>定期購入商品をかごに入れるURL</p>
```

## $item.is_subscription

### 概要
定期購入商品かどうか（通常商品と定期購入商品含む）（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_subscription}></p>
```

#### HTML変換後
```html
<!-- $item.is_subscription: true / false -->
```

## $item.is_subscription_only

### 概要
定期購入商品かどうか（定期購入商品のみ）（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_subscription_only}></p>
```

#### HTML変換後
```html
<!-- $item.is_subscription_only: true / false -->
```

## $item.subscription_price_html

### 概要
定期購入商品の販売価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_price_html}></p>
```

#### HTML変換後
```html
<p>定期購入商品の販売価格</p>
```

## $item.subscription_price

### 概要
定期購入商品の販売価格（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_price}></p>
```

#### HTML変換後
```html
<p>定期購入商品の販売価格（値のみ・金額連動なし）</p>
```

## $item.subscription_price_excluded_tax_html

### 概要
定期購入商品の税抜き販売価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_price_excluded_tax_html}></p>
```

#### HTML変換後
```html
<p>定期購入商品の税抜き販売価格</p>
```

## $item.subscription_price_excluded_tax

### 概要
定期購入商品の税抜き販売価格（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>定期購入商品の税抜き販売価格（値のみ・金額連動なし）</p>
```

## $item.subscription_tax_html

### 概要
定期購入商品の税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_tax_html}></p>
```

#### HTML変換後
```html
<p>定期購入商品の税</p>
```

## $item.subscription_tax

### 概要
定期購入商品の税（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_tax}></p>
```

#### HTML変換後
```html
<p>定期購入商品の税（値のみ・金額連動なし）</p>
```

## $item.subscription_point_html

### 概要
定期購入商品のポイント

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_point_html}></p>
```

#### HTML変換後
```html
<p>定期購入商品のポイント</p>
```

## $item.subscription_point

### 概要
定期購入商品のポイント（値のみ・金額連動なし）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_point}></p>
```

#### HTML変換後
```html
<p>定期購入商品のポイント（値のみ・金額連動なし）</p>
```

## $item.subscription_message

### 概要
定期購入商品のお届けサイクル案内文

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_message}></p>
```

#### HTML変換後
```html
<p>定期購入商品のお届けサイクル案内文</p>
```

## $item.subscription_discount.has_item

### 概要
定期購入商品が回数割引設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.subscription_discount.has_item: true / false -->
```

## $item.subscription_discount.list[i].times

### 概要
回数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.list[i].times}></p>
```

#### HTML変換後
```html
<p>回数</p>
```

## $item.subscription_discount.list[i].quantity

### 概要
数量

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.list[i].quantity}></p>
```

#### HTML変換後
```html
<p>数量</p>
```

## $item.subscription_discount.list[i].point

### 概要
獲得ポイント

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.list[i].point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $item.subscription_discount.list[i].price

### 概要
税込価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.list[i].price}></p>
```

#### HTML変換後
```html
<p>税込価格</p>
```

## $item.subscription_discount.list[i].price_excluded_tax

### 概要
税抜き価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き価格</p>
```

## $item.subscription_discount.list[i].tax

### 概要
税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_discount.list[i].tax}></p>
```

#### HTML変換後
```html
<p>税</p>
```

## $item.subscription_gift.has_item

### 概要
定期購入商品が景品設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_gift.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.subscription_gift.has_item: true / false -->
```

## $item.subscription_gift.list[i].times

### 概要
回数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_gift.list[i].times}></p>
```

#### HTML変換後
```html
<p>回数</p>
```

## $item.subscription_gift.list[i].name

### 概要
景品名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_gift.list[i].name}></p>
```

#### HTML変換後
```html
<p>景品名</p>
```

## $item.subscription_gift.list[i].image_url

### 概要
画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_gift.list[i].image_url}></p>
```

#### HTML変換後
```html
<p>画像URL</p>
```

## $item.subscription_gift.list[i].description

### 概要
詳細情報

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.subscription_gift.list[i].description}></p>
```

#### HTML変換後
```html
<p>詳細情報</p>
```

# 商品一覧系

## $item.group.name

### 概要
商品グループ名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.group.name}></p>
```

#### HTML変換後
```html
<p>商品グループ名</p>
```

## $item.group.has_item

### 概要
商品グループが登録されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.group.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.group.has_item: true / false -->
```

## $item.group

### 概要
商品グループ（配下に .list[i] をつけて商品一覧系タグとして使用）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.group}></p>
```

#### HTML変換後
```html
<p>商品グループ（配下に .list[i] をつけて商品一覧系タグとして使用）</p>
```

# 予約販売

## $item.is_reservation_sale

### 概要
予約販売商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_reservation_sale}></p>
```

#### HTML変換後
```html
<!-- $item.is_reservation_sale: true / false -->
```

## $item.reservation_sale_note

### 概要
予約商品備考

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.reservation_sale_note}></p>
```

#### HTML変換後
```html
<p>予約商品備考</p>
```

## $item.has_release_date

### 概要
発売日が設定されているかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.has_release_date}></p>
```

#### HTML変換後
```html
<!-- $item.has_release_date: true / false -->
```

## $item.is_released

### 概要
発売済みかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_released}></p>
```

#### HTML変換後
```html
<!-- $item.is_released: true / false -->
```

## $item.release_date.year

### 概要
発売日時（年）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.release_date.year}></p>
```

#### HTML変換後
```html
<p>発売日時（年）</p>
```

## $item.release_date.month

### 概要
発売日時（月）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.release_date.month}></p>
```

#### HTML変換後
```html
<p>発売日時（月）</p>
```

## $item.release_date.day

### 概要
発売日時（日）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.release_date.day}></p>
```

#### HTML変換後
```html
<p>発売日時（日）</p>
```

## $item.release_date_note

### 概要
発売日備考・お届け目安

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.release_date_note}></p>
```

#### HTML変換後
```html
<p>発売日備考・お届け目安</p>
```

# SKU

## $item.is_option_sku

### 概要
SKUごとに表示するかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_option_sku}></p>
```

#### HTML変換後
```html
<!-- $item.is_option_sku: true / false -->
```

## $item.is_option_image

### 概要
バリエーション専用画像を表示するかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_option_image}></p>
```

#### HTML変換後
```html
<!-- $item.is_option_image: true / false -->
```

## $item.option_sku.option1_label

### 概要
バリエーション1

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.option1_label}></p>
```

#### HTML変換後
```html
<p>バリエーション1</p>
```

## $item.option_sku.option2_label

### 概要
バリエーション2

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.option2_label}></p>
```

#### HTML変換後
```html
<p>バリエーション2</p>
```

## $item.option_sku.has_option2

### 概要
バリエーション2があるかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.has_option2}></p>
```

#### HTML変換後
```html
<!-- $item.option_sku.has_option2: true / false -->
```

## $item.option_sku.has_item

### 概要
SKUリストが要素を持つかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.option_sku.has_item: true / false -->
```

## $item.option_sku.list[i].name1

### 概要
バリエーション1の項目名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].name1}></p>
```

#### HTML変換後
```html
<p>バリエーション1の項目名</p>
```

## $item.option_sku.list[i].name2

### 概要
バリエーション2の項目名

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].name2}></p>
```

#### HTML変換後
```html
<p>バリエーション2の項目名</p>
```

## $item.option_sku.list[i].image_S

### 概要
バリエーション縮小画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].image_S}></p>
```

#### HTML変換後
```html
<p>バリエーション縮小画像URL</p>
```

## $item.option_sku.list[i].image_L

### 概要
バリエーション画像URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].image_L}></p>
```

#### HTML変換後
```html
<p>バリエーション画像URL</p>
```

## $item.option_sku.list[i].original_code

### 概要
バリエーション独自コード

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].original_code}></p>
```

#### HTML変換後
```html
<p>バリエーション独自コード</p>
```

## $item.option_sku.list[i].price

### 概要
販売価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].price}></p>
```

#### HTML変換後
```html
<p>販売価格</p>
```

## $item.option_sku.list[i].price_excluded_tax

### 概要
税抜き販売価格

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き販売価格</p>
```

## $item.option_sku.list[i].tax

### 概要
税

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].tax}></p>
```

#### HTML変換後
```html
<p>税</p>
```

## $item.option_sku.list[i].point

### 概要
ポイント

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].point}></p>
```

#### HTML変換後
```html
<p>ポイント</p>
```

## $item.option_sku.list[i].subscription_price

### 概要
販売価格（定期購入商品）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].subscription_price}></p>
```

#### HTML変換後
```html
<p>販売価格（定期購入商品）</p>
```

## $item.option_sku.list[i].subscription_price_excluded_tax

### 概要
税抜き販売価格（定期購入商品）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].subscription_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き販売価格（定期購入商品）</p>
```

## $item.option_sku.list[i].subscription_tax

### 概要
税（定期購入商品）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].subscription_tax}></p>
```

#### HTML変換後
```html
<p>税（定期購入商品）</p>
```

## $item.option_sku.list[i].subscription_point

### 概要
ポイント（定期購入商品）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].subscription_point}></p>
```

#### HTML変換後
```html
<p>ポイント（定期購入商品）</p>
```

## $item.option_sku.list[i].small_stock_quantity

### 概要
残りわずかとする数量

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].small_stock_quantity}></p>
```

#### HTML変換後
```html
<p>残りわずかとする数量</p>
```

## $item.option_sku.list[i].is_stock_unlimited

### 概要
在庫無制限商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].is_stock_unlimited}></p>
```

#### HTML変換後
```html
<!-- $item.option_sku.list[i].is_stock_unlimited: true / false -->
```

## $item.option_sku.list[i].stock_quantity

### 概要
在庫数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## $item.option_sku.list[i].is_soldout

### 概要
売り切れかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].is_soldout}></p>
```

#### HTML変換後
```html
<!-- $item.option_sku.list[i].is_soldout: true / false -->
```

## $item.option_sku.list[i].is_small_stock

### 概要
残りわずかかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].is_small_stock}></p>
```

#### HTML変換後
```html
<!-- $item.option_sku.list[i].is_small_stock: true / false -->
```

## $item.option_sku.list[i].cart_entry_url

### 概要
かごに入れるURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].cart_entry_url}></p>
```

#### HTML変換後
```html
<p>かごに入れるURL</p>
```

## $item.option_sku.list[i].cart_entry_subscription_url

### 概要
かごに入れるURL（定期購入商品）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].cart_entry_subscription_url}></p>
```

#### HTML変換後
```html
<p>かごに入れるURL（定期購入商品）</p>
```

## $item.option_sku.list[i].restock_url

### 概要
再入荷お知らせURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].restock_url}></p>
```

#### HTML変換後
```html
<p>再入荷お知らせURL</p>
```

## $item.option_sku.list[i].is_favorite

### 概要
お気に入りに追加済みかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].is_favorite}></p>
```

#### HTML変換後
```html
<!-- $item.option_sku.list[i].is_favorite: true / false -->
```

## $item.option_sku.list[i].favorite_entry_url

### 概要
お気に入りに追加URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].favorite_entry_url}></p>
```

#### HTML変換後
```html
<p>お気に入りに追加URL</p>
```

## $item.option_sku.list[i].favorite_remove_url

### 概要
お気に入りから削除URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.option_sku.list[i].favorite_remove_url}></p>
```

#### HTML変換後
```html
<p>お気に入りから削除URL</p>
```

# まとめ買い割引

## $item.is_bulk

### 概要
まとめ買い割引商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_bulk}></p>
```

#### HTML変換後
```html
<!-- $item.is_bulk: true / false -->
```

## $item.bulk_name

### 概要
この商品が所属するまとめ買い割引の名前

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.bulk_name}></p>
```

#### HTML変換後
```html
<p>この商品が所属するまとめ買い割引の名前</p>
```

## $item.bulk_url

### 概要
この商品が所属するまとめ買い割引商品一覧のURL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.bulk_url}></p>
```

#### HTML変換後
```html
<p>この商品が所属するまとめ買い割引商品一覧のURL</p>
```

# 名入れ

## $item.is_name_print

### 概要
名入れ商品かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.is_name_print}></p>
```

#### HTML変換後
```html
<!-- $item.is_name_print: true / false -->
```

## $item.name_print.description

### 概要
名入れ説明文

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.description}></p>
```

#### HTML変換後
```html
<p>名入れ説明文</p>
```

## $item.name_print.has_item

### 概要
名入れ入力欄があるかどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.has_item}></p>
```

#### HTML変換後
```html
<!-- $item.name_print.has_item: true / false -->
```

## $item.name_print.list[i].title

### 概要
名入れ入力欄のタイトル

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].title}></p>
```

#### HTML変換後
```html
<p>名入れ入力欄のタイトル</p>
```

## $item.name_print.list[i].html

### 概要
名入れ入力欄のHTML

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].html}></p>
```

#### HTML変換後
```html
<p>名入れ入力欄のHTML</p>
```

## $item.name_print.list[i].is_required

### 概要
名入れ入力欄が必須かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].is_required}></p>
```

#### HTML変換後
```html
<!-- $item.name_print.list[i].is_required: true / false -->
```

## $item.name_print.list[i].character_type

### 概要
名入れ入力欄に入力可能な文字種類（/区切り）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].character_type}></p>
```

#### HTML変換後
```html
<p>名入れ入力欄に入力可能な文字種類（/区切り）</p>
```

## $item.name_print.list[i].column_max

### 概要
名入れ入力欄に入力可能な1行の最大文字数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].column_max}></p>
```

#### HTML変換後
```html
<p>名入れ入力欄に入力可能な1行の最大文字数</p>
```

## $item.name_print.list[i].row_max

### 概要
名入れ入力欄に入力可能な最大行数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].row_max}></p>
```

#### HTML変換後
```html
<p>名入れ入力欄に入力可能な最大行数</p>
```

## $item.name_print.list[i].total_max

### 概要
名入れ入力欄に入力可能な全体の最大文字数

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$item.name_print.list[i].total_max}></p>
```

#### HTML変換後
```html
<p>名入れ入力欄に入力可能な全体の最大文字数</p>
```
