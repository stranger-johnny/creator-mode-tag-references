# カテゴリー情報

## $category.name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $category.code

### 概要
カテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $category.image_url

### 概要
カテゴリー画像URL

### サンプルコード

#### クリエーターモード
```php
<img src="<{$category.image_url}>" alt="<{$category.name}>">
```

#### HTML変換後
```html
<img src="カテゴリー画像URL" alt="カテゴリー名">
```

## $category.total_count

### 概要
総商品数

### サンプルコード

#### クリエーターモード
```php
<p>（全<span><{$category.total_count}></span>件）<{$category.display_count}>件表示</p>
```

#### HTML変換後
```html
<p>（全<span>総商品数</span>件）表示商品数件表示</p>
```

## $category.display_count

### 概要
表示商品数

### サンプルコード

#### クリエーターモード
```php
<p>（全<span><{$category.total_count}></span>件）<{$category.display_count}>件表示</p>
```

#### HTML変換後
```html
<p>（全<span>総商品数</span>件）表示商品数件表示</p>
```

# パンくず

## $category.breadcrumb_list.list[i].name

### 概要
ページ名

### サンプルコード

#### クリエーターモード
```php
<span>
    <a href="<{$category.breadcrumb_list.list[i].url}>"><{$category.breadcrumb_list.list[i].name}></a>
 </span>
```

#### HTML変換後
```html
<span>
    <a href="/view/category/カテゴリーURL">ページ名</a>
</span>
```

## $category.breadcrumb_list.list[i].url

### 概要
ページURL

### サンプルコード

#### クリエーターモード
```php
<span>
    <a href="<{$category.breadcrumb_list.list[i].url}>"><{$category.breadcrumb_list.list[i].name}></a>
 </span>
```

#### HTML変換後
```html
<span>
    <a href="/view/category/カテゴリーURL">ページ名</a>
</span>
```

## $category.breadcrumb_list.list[i].is_current

### 概要
現在地かどうか

### サンプルコード

#### クリエーターモード
```php
<span class="<{if $category.breadcrumb_list.list[i].is_current}>current<{/if}>">
    <a href="<{$category.breadcrumb_list.list[i].url}>"><{$category.breadcrumb_list.list[i].name}></a>
 </span>
```

#### HTML変換後
```html
<span class="current">
    <a href="/view/category/カテゴリーURL">ページ名</a>
</span>
```

# 並び替え

## $category.sort_recommend_url

### 概要
並び替えURL（おすすめ順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$category.sort_recommend_url}>">おすすめ順</a></dd>
```

#### HTML変換後
```html
<dd><a href="/view/category/カテゴリーURL?sort=recommend">おすすめ順</a></dd>
```

## $category.sort_new_url

### 概要
並び替えURL（新着順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$category.sort_new_url}>">新着順</a></dd>
```

#### HTML変換後
```html
<dd><a href="/view/category/カテゴリーURL?sort=order">新着順</a></dd>
```

## $category.sort_high_price_url

### 概要
並び替えURL（価格が高い順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$category.sort_high_price_url}>">価格の高い順</a></dd>
```

#### HTML変換後
```html
<dd><a href="/view/category/カテゴリーURL?sort=price_high">価格の高い順</a></dd>
```

## $category.sort_low_price_url

### 概要
並び替えURL（価格が低い順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$category.sort_low_price_url}>">価格の低い順</a></dd>
```

#### HTML変換後
```html
<dd><a href="/view/category/カテゴリーURL?sort=price">価格の低い順</a></dd>
```

## $category.is_sort_recommend_selected

### 概要
おすすめ順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_recommend_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_recommend_selected -->
```

## $category.is_sort_new_selected

### 概要
新着順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_new_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_new_selected -->
```

## $category.sort_name_url

### 概要
並び替えURL（商品名順）

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.sort_name_url -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.sort_name_url -->
```

## $category.is_sort_name_selected

### 概要
商品名順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_name_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_name_selected -->
```

## $category.sort_manufacturer_url

### 概要
並び替えURL（製造元順）

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.sort_manufacturer_url -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.sort_manufacturer_url -->
```

## $category.sort_manufacturer_selected

### 概要
製造元順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.sort_manufacturer_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.sort_manufacturer_selected -->
```

## $category.is_sort_high_price_selected

### 概要
高価格順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_high_price_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_high_price_selected -->
```

## $category.is_sort_low_price_selected

### 概要
低価格順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_low_price_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.is_sort_low_price_selected -->
```

# 商品一覧

## $category.item.has_item

### 概要
商品が登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.has_item}>
    <ul>
      <{section name=i loop=$category.item.list}>
      <li>
        <div>
          <{if $category.item.list[i].is_soldout}>
          <p>SOLD OUT</p>
          <{elseif $category.item.list[i].is_sale}>
          <p>SALE</p>
          <{/if}>
        </div>
        <div>
          <a href="<{$category.item.list[i].url}>">
            <img src="<{$category.item.list[i].image_L}>" alt="">
          </a>
        </div>
        <{if $category.item.list[i].base_category.url}>
        <p>
          <a href="<{$category.item.list[i].base_category.url}>">
            <{$category.item.list[i].base_category.name}>
          </a>
        </p>
        <{/if}>
        <p>
          <a href="<{$category.item.list[i].url}>">
            <{$category.item.list[i].name}>
          </a>
        </p>
        <{if $category.item.list[i].is_sale}>
        <p>￥<{$category.item.list[i].original_price|number_format}><span>（税込）</span>
        </p>
        <p>￥<{$category.item.list[i].price|number_format}><span>（税込）</span>
          <span>[<{$category.item.list[i].sale_rate}>%OFF</span>]
        </p>
        <{else}>
        <p>￥<{$category.item.list[i].price|number_format}><span>（税込）</span></p>
        <{/if}>
        <{if $category.item.list[i].has_review}>
        <div>
          <{$category.item.list[i].review.star_html}>
          <p><{$category.item.list[i].review.average}></p>
          <p>[<{$category.item.list[i].review.total_count}>件]
          </p>
        </div>
        <{/if}>
        <div>
          <{if $category.item.list[i].is_soldout}>
          <div>売り切れ</div>
          <{else}>
          <a href="<{$category.item.list[i].cart_entry_url}>">カートに入れる</a>
          <{/if}>
          <div class="<{if $category.item.list[i].is_favorite}>favorite-on<{/if}>">
            <a href="<{$category.item.list[i].favorite_entry_url}>"></a>
          </div>
        </div>
      </li>
      <{/section}>
    </ul>
    <{else}>
    <p>このカテゴリーには商品がありません</p>
<{/if}>
```

#### HTML変換後
```html
<ul>
    <li>
      <div>
        <a href="/view/item/商品URL"><img src="商品画像パス.jpg" alt="商品名"></a>
      </div>
      <p><a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a></p>
      <p><a href="/view/item/商品URL">商品名</a></p>
      <p>通常価格<span>（税込）</span></p>
      <div>
        <a href="#makeshop-common-cart-entry-url">カートに入れる</a>
        <div class="favorite">
          <a href="お気に入りに追加URL"></a>
        </div>
      </div>
    </li>
</ul>
```

## $category.item.list[i].num

### 概要
番号

### サンプルコード

#### クリエーターモード
```php
<div><{$category.item.list[i].num}></div>
```

#### HTML変換後
```html
<div>番号</div>
```

## $category.item.list[i].name

### 概要
商品名

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$category.item.list[i].url}>"><{$category.item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品URL">商品名</a></p>
```

## $category.item.list[i].price

### 概要
販売価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.item.list[i].price}>（税込）</p>
```

#### HTML変換後
```html
<p>￥販売価格（税込）</p>
```

## $category.item.list[i].price_excluded_tax

### 概要
税抜き価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.item.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き価格</p>
```

## $category.item.list[i].tax

### 概要
税

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].tax}></p>
```

#### HTML変換後
```html
<p>消費税額</p>
```

## $category.item.list[i].tax_rate

### 概要
消費税率

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].tax_rate}>%</p>
```

#### HTML変換後
```html
<p>10%</p>
```

## $category.item.list[i].is_reduced_tax_rate

### 概要
軽減税率対象商品かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.item.list[i].is_reduced_tax_rate -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.item.list[i].is_reduced_tax_rate -->
```

## $category.item.list[i].fixed_price

### 概要
定価

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.item.list[i].fixed_price}></p>
```

#### HTML変換後
```html
<p>￥定価</p>
```

## $category.item.list[i].original_price

### 概要
通常価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.item.list[i].original_price}></p>
```

#### HTML変換後
```html
<p>￥通常価格</p>
```

## $category.item.list[i].original_price_excluded_tax

### 概要
税抜き通常価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.item.list[i].original_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き通常価格</p>
```

## $category.item.list[i].original_tax

### 概要
通常価格の税

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].original_tax}></p>
```

#### HTML変換後
```html
<p>通常価格の税</p>
```

## $category.item.list[i].url

### 概要
商品URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$category.item.list[i].url}>"><{$category.item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品URL">商品名</a></p>
```

## $category.item.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.item.list[i].image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="商品縮小画像パス.jpg"></div>
```

## $category.item.list[i].image_M

### 概要
商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.item.list[i].image_M}>"></div>
```

#### HTML変換後
```html
<div><img src="商品普通画像パス.jpg"></div>
```

## $category.item.list[i].image_L

### 概要
商品画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.item.list[i].image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="商品画像パス.jpg"></div>
```

## $category.item.list[i].is_stock_display

### 概要
在庫表示可かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_stock_display}>
    <{if $category.item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $category.item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$category.item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$category.item.list[i].stock_quantity}>個</span></p>
        <{/if}>
    <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## $category.item.list[i].is_stock_unlimited

### 概要
在庫無制限かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $category.item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$category.item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$category.item.list[i].stock_quantity}>個</span></p>
        <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## $category.item.list[i].is_soldout

### 概要
売り切れかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_soldout}>
    <p>SOLD OUT</p>
<{elseif $category.item.list[i].is_sale}>
    <p>SALE</p>
<{/if}>
```

#### HTML変換後
```html
<p>SOLD OUT</p>
```

## $category.item.list[i].is_small_stock

### 概要
在庫が指定された数以下かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_small_stock}>
        <p>△残りわずか<span>あと<{$category.item.list[i].stock_quantity}>個</span></p>
    <{else}>
        <p>〇在庫あり<span>あと●●個</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり<span>あと●●個</span></p>
```

## $category.item.list[i].stock_quantity

### 概要
在庫数

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## $category.item.list[i].is_sale

### 概要
セール商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_sale}>
    <p>￥<{$category.item.list[i].original_price|number_format}><span>（税込）</span></p>
    <p>￥<{$category.item.list[i].price|number_format}><span>（税込）</span>
    <span>[<{$category.item.list[i].sale_rate}>%OFF</span>]</p>
<{else}>
    <p>￥<{$category.item.list[i].price|number_format}><span>（税込）</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>￥通常価格<span>（税込）</span></p>
<p>￥セール価格<span>（税込）</span><span>[●●%OFF</span>]</p>
```

## $category.item.list[i].sale_rate

### 概要
割引率

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item$category.item.list[i].sale_rate}>%OFF</p>
```

#### HTML変換後
```html
<p>●●%OFF</p>
```

## $category.item.list[i].has_review

### 概要
旧レビューが投稿されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].has_review}>
    <div>
        <{$category.item.list[i].review.star_html}>
        <p><{$category.item.list[i].review.average}></p>
        <p>[<{$category.item.list[i].review.total_count}>件]</p>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <div class="reviewRate">
        <div class="reviewRateStar starOn">評価1</div>
        <div class="reviewRateStar starOn">評価2</div>
        <div class="reviewRateStar staron">評価3</div>
        <div class="reviewRateStar starOff">評価4</div>
        <div class="reviewRateStar starOff">評価5</div>
    </div>
    <p>平均レビュー点数</p>
    <p>[●●件]</p>
</div>
```

## $category.item.list[i].review.star_html

### 概要
旧レビュー評価（星）

### サンプルコード

#### クリエーターモード
```php
<div><{$category.item.list[i].review.star_html}></div>
```

#### HTML変換後
```html
<div class="reviewRate">
    <div class="reviewRateStar starOn">評価1</div>
    <div class="reviewRateStar starOn">評価2</div>
    <div class="reviewRateStar staron">評価3</div>
    <div class="reviewRateStar starOff">評価4</div>
    <div class="reviewRateStar starOff">評価5</div>
</div>
```

## $category.item.list[i].review.average

### 概要
平均旧レビュー点数

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].review.average}></p>
```

#### HTML変換後
```html
<p>平均レビュー点数</p>
```

## $category.item.list[i].review.total_count

### 概要
旧レビュー投稿数

### サンプルコード

#### クリエーターモード
```php
<p>[<{$category.item.list[i].review.total_count}>件]</p>
```

#### HTML変換後
```html
<p>[●●件]</p>
```

## $category.item.list[i].review.url

### 概要
旧レビュー一覧URL

### サンプルコード

#### クリエーターモード
```php
<p>[<a href="<{$category.item.list[i].review.url}>"><{$category.item.list[i].review.total_count}>件</a>]</p>
```

#### HTML変換後
```html
<p>[<a href="/view/review/レビュー一覧URL">●●件</a>]</p>
```

## $category.item.list[i].child_category.has_item

### 概要
サブカテゴリーを持っているかどうか

### サンプルコード

#### クリエーターモード
```php
<{section name=i loop=$category.item.list}>
<ul>
    <!--1階層目-->
    <li><a href="<{$category.item.list[i].url}>"><{$category.item.list[i].name}><{$category.item.list[i].code}></a></li>
        <!--2階層目-->
        <{if $category.item.list[i].child_category.has_item}>
        <ul>
            <{section name=j loop=$category.item.list[i].child_category.list}>
            <li><a href="<{$category.item.list[i].child_category.list[j].url}>"><{$category.item.list[i].child_category.list[j].name}><{$category.item.list[i].child_category.list[j].code}></a>
                <!--3階層目-->
                <{if $category.item.list[i].child_category.list[j].child_category.has_item}>
                <ul>
                    <{section name=k loop=$category.item.list[i].child_category.list[j].child_category.list}>
                    <li><a href="<{$category.item.list[i].child_category.list[j].child_category.list[k].url}>"><{$category.item.list[i].child_category.list[j].child_category.list[k].name}><{$category.item.list[i].child_category.list[j].child_category.list[k].code}></a>
                        <!--4階層目-->
                        <{if $category.item.list[i].child_category.list[j].child_category.list[k].child_category.has_item}>
                        <ul>
                            <{section name=l loop=$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list}>
                            <li><a href="<{$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].url}>"><{$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].name}><{$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].code}></a>
                                <!--5階層目-->
                                <{if $category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.has_item}>
                                <ul>
                                    <{section name=m loop=$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list}>
                                    <li><a href="<{$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].url}>"><{$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].name}><{$category.item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].code}></a></li>
                                    <{/section}>
                                </ul>
                                <{/if}>
                            </li>
                            <{/section}>
                        </ul>
                        <{/if}>
                    </li>
                    <{/section}>
                </ul>
                <{/if}>
            </li>
            <{/section}>
        </ul>
        <{/if}>
</ul>
<{/section}>
```

#### HTML変換後
```html
<ul>
    <!--1階層目-->
    <li><a href="カテゴリーURL">カテゴリー名ct0</a></li>
        <!--2階層目-->
        <ul>
            <li><a href="サブカテゴリー（2階層目）URL">サブカテゴリー（2階層目）名ct00</a>
                <!--3階層目-->
                <ul>
                    <li><a href="サブカテゴリー（3階層目）URL">サブカテゴリー（3階層目）名ct000</a>
                        <!--4階層目-->
                        <ul>
                            <li><a href="サブカテゴリー（4階層目）URL">サブカテゴリー（4階層目）名ct0000</a>
                                <!--5階層目-->
                                <ul>
                                    <li><a href="サブカテゴリー（5階層目）URL">サブカテゴリー（5階層目）名ct00000</a></li>
                                </ul>
                            </li>
                        </ul>
                    </li>
                </ul>
            </li>
        </ul>
</ul>
```

## $category.item.list[i].original_code

### 概要
独自商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].original_code}></p>
```

#### HTML変換後
```html
<p>独自商品コード</p>
```

## $category.item.list[i].system_code

### 概要
システム商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## $category.item.list[i].point

### 概要
獲得ポイント

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $category.item.list[i].is_member_price

### 概要
会員割引商品かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.item.list[i].is_member_price -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.item.list[i].is_member_price -->
```

## $category.item.list[i].base_category.name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].base_category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $category.item.list[i].base_category.url

### 概要
カテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$category.item.list[i].base_category.url}"></a></p>
```

#### HTML変換後
```html
<p><a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a></p>
```

## $category.item.list[i].base_category.code

### 概要
カテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].base_category.code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $category.item.list[i].description

### 概要
商品説明文

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].description}></p>
```

#### HTML変換後
```html
<p>商品説明文</p>
```

## $category.item.list[i].category_description

### 概要
商品カテゴリーページ用の商品説明文

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].category_description}></p>
```

#### HTML変換後
```html
<p>商品カテゴリーページ用の商品説明文</p>
```

## $category.item.list[i].manufacturer

### 概要
製造元

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].manufacturer}></p>
```

#### HTML変換後
```html
<p>製造元</p>
```

## $category.item.list[i].origin_country

### 概要
原産地

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].origin_country}></p>
```

#### HTML変換後
```html
<p>原産地</p>
```

## $category.item.list[i].special_display

### 概要
商品別特殊表示

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## $category.item.list[i].is_reservation_sale

### 概要
予約販売商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_reservation_sale}>
    <div>
        <{if $category.item.list[i].has_release_date}>
            <{if !$category.item.list[i].is_released}>
                <p>販売開始：<{$category.item.list[i].release_date.year}>年<{$category.item.list[i].release_date.month}>月<{$category.item.list[i].release_date.day}>日</p>
            <{/if}>
        <{/if}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $category.item.list[i].reservation_sale_note

### 概要
備考

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].reservation_sale_note}></p>
```

#### HTML変換後
```html
<p>備考</p>
```

## $category.item.list[i].has_release_date

### 概要
発売日が設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $category.item.list[i].has_release_date}>
        <{if !$category.item.list[i].is_released}>
            <p>販売開始：<{$category.item.list[i].release_date.year}>年<{$category.item.list[i].release_date.month}>月<{$category.item.list[i].release_date.day}>日</p>
        <{/if}>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $category.item.list[i].is_released

### 概要
発売済みかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if !$category.item.list[i].is_released}>
        <p>販売開始：<{$category.item.list[i].release_date.year}>年<{$category.item.list[i].release_date.month}>月<{$category.item.list[i].release_date.day}>日</p>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $category.item.list[i].release_date.year

### 概要
発売日時（年）
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].release_date.year}></p>
```

#### HTML変換後
```html
<p>発売日時（年）</p>
```

## $category.item.list[i].release_date.month

### 概要
発売日時（月）
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].release_date.month}></p>
```

#### HTML変換後
```html
<p>発売日時（月）</p>
```

## $category.item.list[i].release_date.day

### 概要
発売日時（日）
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].release_date.day}></p>
```

#### HTML変換後
```html
<p>発売日時（日）</p>
```

## $category.item.list[i].release_date_note

### 概要
発売日備考
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item.list[i].release_date_note}></p>
```

#### HTML変換後
```html
<p>発売日備考</p>
```

## $category.item.list[i].has_option

### 概要
オプションが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.item.list[i].has_option -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.item.list[i].has_option -->
```

## $category.item.list[i].is_favorite

### 概要
お気に入りに追加済みかどうか

### サンプルコード

#### クリエーターモード
```php
<div class="favorite <{if $category.item.list[i].is_favorite}>favorite-on<{/if}>">
    <a href="<{$category.item.list[i].favorite_entry_url}>"></a>
</div>
```

#### HTML変換後
```html
<div class="favorite favorite-on">
    <a href="#makeshop-common-favorite-entry-url:商品URL番号"></a>
</div>
```

## $category.item.list[i].favorite_entry_url

### 概要
お気に入りに追加URL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$category.item.list[i].favorite_entry_url}>"></a></div>
```

#### HTML変換後
```html
<div><a href="#makeshop-common-favorite-entry-url:商品URL番号"></a></div>
```

## $category.item.list[i].favorite_remove_url

### 概要
お気に入りから削除URL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$category.item.list[i].favorite_remove_url}>"></a></div>
```

#### HTML変換後
```html
<div><a href="お気に入りから削除URL"></a></div>
```

## $category.item.list[i].cart_entry_url

### 概要
かごに入れるURL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$category.item.list[i].cart_entry_url}>">カートに入れる</a></div>
```

#### HTML変換後
```html
<div><a href="#makeshop-common-cart-entry-url:商品URL番号">カートに入れる</a></div>
```

## $category.item.list[i].icon.has_item

### 概要
アイコンが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].icon.has_item}>
    <div>
        <ul>
            <{section name=j loop=$category.item.list[i].icon.list}>
                <li>
                    <img src="<{$category.item.list[i].icon.list[j].image_url}>">
                </li>
            <{/section}>
        </ul>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <ul>
        <li>
            <img src="アイコン画像URL">
        </li>
    </ul>
</div>
```

## $category.item.list[i].icon.list[j].image_url

### 概要
アイコン画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.item.list[i].icon.list[j].image_url}>" ></div>
```

#### HTML変換後
```html
<div><img src="アイコン画像URL.jpg" ></div>
```

## $category.item.list[i].is_bulk

### 概要
まとめ買い割引商品化どうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_bulk}>
    <p><a href="<{$category.item.list[i].bulk_url}>"><{$category.item.list[i].bulk_name}></a></p>
<{/if}>
```

#### HTML変換後
```html
<{if $category.item.list[i].is_bulk}>
    <p><a href="/view/bulk/まとめ買い割引商品一覧のURL">まとめ買い割引の名前</a></p>
<{/if}>
```

## $category.item.list[i].bulk_url

### 概要
まとめ買い割引商品一覧のURL

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_bulk}>
    <p><a href="<{$category.item.list[i].bulk_url}>"><{$category.item.list[i].bulk_name}></a></p>
<{/if}>
```

#### HTML変換後
```html
<{if $category.item.list[i].is_bulk}>
    <p><a href="/view/bulk/まとめ買い割引商品一覧のURL">まとめ買い割引の名前</a></p>
<{/if}>
```

## $category.item.list[i].bulk_name

### 概要
まとめ買い割引の名前

### サンプルコード

#### クリエーターモード
```php
<{if $category.item.list[i].is_bulk}>
    <p><a href="<{$category.item.list[i].bulk_url}>"><{$category.item.list[i].bulk_name}></a></p>
<{/if}>
```

#### HTML変換後
```html
<{if $category.item.list[i].is_bulk}>
    <p><a href="/view/bulk/まとめ買い割引商品一覧のURL">まとめ買い割引の名前</a></p>
<{/if}>
```

# カテゴリーおすすめ商品

## $category.recommend_item.has_item

### 概要
カテゴリーおすすめ商品があるかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.has_item}>
    <ul>
      <{section name=i loop=$category.recommend_item.list}>
      <li>
        <div>
          <{if $category.recommend_item.list[i].is_soldout}>
          <p>SOLD OUT</p>
          <{elseif $category.recommend_item.list[i].is_sale}>
          <p>SALE</p>
          <{/if}>
        </div>
        <div>
          <a href="<{$category.recommend_item.list[i].url}>">
            <img src="<{$category.recommend_item.list[i].image_L}>" alt="">
          </a>
        </div>
        <{if $category.recommend_item.list[i].base_category.url}>
        <p>
          <a href="<{$category.recommend_item.list[i].base_category.url}>">
            <{$category.recommend_item.list[i].base_category.name}>
          </a>
        </p>
        <{/if}>
        <p>
          <a href="<{$category.recommend_item.list[i].url}>">
            <{$category.recommend_item.list[i].name}>
          </a>
        </p>
        <{if $category.recommend_item.list[i].is_sale}>
        <p>￥<{$category.recommend_item.list[i].original_price|number_format}><span>（税込）</span>
        </p>
        <p>￥<{$category.recommend_item.list[i].price|number_format}><span>（税込）</span>
          <span>[<{$category.recommend_item.list[i].sale_rate}>%OFF</span>]
        </p>
        <{else}>
        <p>￥<{$category.recommend_item.list[i].price|number_format}><span>（税込）</span></p>
        <{/if}>
        <{if $category.recommend_item.list[i].has_review}>
        <div>
          <{$category.recommend_item.list[i].review.star_html}>
          <p><{$category.recommend_item.list[i].review.average}></p>
          <p>[<{$category.recommend_item.list[i].review.total_count}>件]
          </p>
        </div>
        <{/if}>
        <div>
          <{if $category.recommend_item.list[i].is_soldout}>
          <div>売り切れ</div>
          <{else}>
          <a href="<{$category.recommend_item.list[i].cart_entry_url}>">カートに入れる</a>
          <{/if}>
          <div class="<{if $category.recommend_item.list[i].is_favorite}>favorite-on<{/if}>">
            <a href="<{$category.recommend_item.list[i].favorite_entry_url}>"></a>
          </div>
        </div>
      </li>
      <{/section}>
    </ul>
    <{else}>
    <p>このカテゴリーには商品がありません</p>
<{/if}>
```

#### HTML変換後
```html
<ul>
    <li>
      <div>
        <a href="/view/item/商品URL"><img src="商品画像パス.jpg" alt="商品名"></a>
      </div>
      <p><a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a></p>
      <p><a href="/view/item/商品URL">商品名</a></p>
      <p>通常価格<span>（税込）</span></p>
      <div>
        <a href="#makeshop-common-cart-entry-url">カートに入れる</a>
        <div class="favorite">
          <a href="お気に入りに追加URL"></a>
        </div>
      </div>
    </li>
</ul>
```

## $category.recommend_item.list[i].num

### 概要
番号

### サンプルコード

#### クリエーターモード
```php
<div><{$category.recommend_item.list[i].num}></div>
```

#### HTML変換後
```html
<div>番号</div>
```

## $category.recommend_item.list[i].name

### 概要
商品名

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$category.recommend_item.list[i].url}>"><{$category.recommend_item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品URL">商品名</a></p>
```

## $category.recommend_item.list[i].price

### 概要
販売価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.recommend_item.list[i].price}>（税込）</p>
```

#### HTML変換後
```html
<p>￥販売価格（税込）</p>
```

## $category.recommend_item.list[i].price_excluded_tax

### 概要
税抜き価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.recommend_item.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き価格</p>
```

## $category.recommend_item.list[i].tax

### 概要
税

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].tax}></p>
```

#### HTML変換後
```html
<p>消費税額</p>
```

## $category.recommend_item.list[i].fixed_price

### 概要
定価

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.recommend_item.list[i].fixed_price}></p>
```

#### HTML変換後
```html
<p>￥定価</p>
```

## $category.recommend_item.list[i].original_price

### 概要
通常価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$category.recommend_item.list[i].original_price}></p>
```

#### HTML変換後
```html
<p>￥通常価格</p>
```

## $category.recommend_item.list[i].url

### 概要
商品URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$category.recommend_item.list[i].url}>"><{$category.recommend_item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品URL">商品名</a></p>
```

## $category.recommend_item.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.recommend_item.list[i].image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="商品縮小画像パス.jpg"></div>
```

## $category.recommend_item.list[i].image_M

### 概要
商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.recommend_item.list[i].image_M}>"></div>
```

#### HTML変換後
```html
<div><img src="商品普通画像パス.jpg"></div>
```

## $category.recommend_item.list[i].image_L

### 概要
商品画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.recommend_item.list[i].image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="商品画像パス.jpg"></div>
```

## $category.recommend_item.list[i].is_stock_display

### 概要
在庫表示可かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].is_stock_display}>
    <{if $category.recommend_item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $category.recommend_item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$category.recommend_item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$category.recommend_item.list[i].stock_quantity}>個</span></p>
        <{/if}>
    <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## $category.recommend_item.list[i].is_stock_unlimited

### 概要
在庫無制限かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $category.recommend_item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$category.recommend_item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$category.recommend_item.list[i].stock_quantity}>個</span></p>
        <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## $category.recommend_item.list[i].is_soldout

### 概要
売り切れかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].is_soldout}>
    <div>売り切れ</div>
<{else}>
    <a href="<{$category.recommend_item.list[i].cart_entry_url}>">カートに入れる</a>
<{/if}>
```

#### HTML変換後
```html
<div>売り切れ</div>
```

## $category.recommend_item.list[i].is_small_stock

### 概要
在庫が指定された数以下かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].is_small_stock}>
        <p>△残りわずか<span>あと<{$category.recommend_item.list[i].stock_quantity}>個</span></p>
    <{else}>
        <p>〇在庫あり<span>あと●●個</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり<span>あと●●個</span></p>
```

## $category.recommend_item.list[i].stock_quantity

### 概要
在庫数

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## $category.recommend_item.list[i].is_sale

### 概要
セール商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].is_sale}>
    <p>￥<{$category.recommend_item.list[i].original_price|number_format}><span>（税込）</span></p>
    <p>￥<{$category.recommend_item.list[i].price|number_format}><span>（税込）</span>
    <span>[<{$category.recommend_item.list[i].sale_rate}>%OFF</span>]</p>
<{else}>
    <p>￥<{$category.recommend_item.list[i].price|number_format}><span>（税込）</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>￥通常価格<span>（税込）</span></p>
<p>￥セール価格<span>（税込）</span><span>[●●%OFF</span>]</p>
```

## $category.recommend_item.list[i].sale_rate

### 概要
割引率

### サンプルコード

#### クリエーターモード
```php
<p><{$category.itemcategory-recommend-item-list-sale-rate}>%OFF</p>
```

#### HTML変換後
```html
<p>●●%OFF</p>
```

## $category.recommend_item.list[i].has_review

### 概要
旧レビューが投稿されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].has_review}>
    <div>
        <{$category.recommend_item.list[i].review.star_html}>
        <p><{$category.recommend_item.list[i].review.average}></p>
        <p>[<{$category.recommend_item.list[i].review.total_count}>件]</p>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <div class="reviewRate">
        <div class="reviewRateStar starOn">評価1</div>
        <div class="reviewRateStar starOn">評価2</div>
        <div class="reviewRateStar staron">評価3</div>
        <div class="reviewRateStar starOff">評価4</div>
        <div class="reviewRateStar starOff">評価5</div>
    </div>
    <p>平均レビュー点数</p>
    <p>[●●件]</p>
</div>
```

## $category.recommend_item.list[i].review.star_html

### 概要
旧レビュー評価（星）

### サンプルコード

#### クリエーターモード
```php
<div><{$category.recommend_item.list[i].review.star_html}></div>
```

#### HTML変換後
```html
<div class="reviewRate">
    <div class="reviewRateStar starOn">評価1</div>
    <div class="reviewRateStar starOn">評価2</div>
    <div class="reviewRateStar staron">評価3</div>
    <div class="reviewRateStar starOff">評価4</div>
    <div class="reviewRateStar starOff">評価5</div>
</div>
```

## $category.recommend_item.list[i].review.average

### 概要
旧平均レビュー点数

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].review.average}></p>
```

#### HTML変換後
```html
<p>平均レビュー点数</p>
```

## $category.recommend_item.list[i].review.total_count

### 概要
旧レビュー投稿数

### サンプルコード

#### クリエーターモード
```php
<p>[<{$category.recommend_item.list[i].review.total_count}>件]</p>
```

#### HTML変換後
```html
<p>[●●件]</p>
```

## $category.recommend_item.list[i].review.url

### 概要
旧レビュー一覧URL

### サンプルコード

#### クリエーターモード
```php
<p>[<a href="<{$category.recommend_item.list[i].review.url}>"><{$category.item.list[i].review.total_count}>件</a>]</p>
```

#### HTML変換後
```html
<p>[<a href="/view/review/レビュー一覧URL">●●件</a>]</p>
```

## $category.recommend_item.list[i].child_category.has_item

### 概要
サブカテゴリーを持っているかどうか

### サンプルコード

#### クリエーターモード
```php
<{section name=i loop=$category.recommend_item.list}>
<ul>
    <!--1階層目-->
    <li><a href="<{$category.recommend_item.list[i].url}>"><{$category.recommend_item.list[i].name}><{$category.recommend_item.list[i].code}></a></li>
        <!--2階層目-->
        <{if $category.recommend_item.list[i].child_category.has_item}>
        <ul>
            <{section name=j loop=$category.recommend_item.list[i].child_category.list}>
            <li><a href="<{$category.recommend_item.list[i].child_category.list[j].url}>"><{$category.recommend_item.list[i].child_category.list[j].name}><{$category.recommend_item.list[i].child_category.list[j].code}></a>
                <!--3階層目-->
                <{if $category.recommend_item.list[i].child_category.list[j].child_category.has_item}>
                <ul>
                    <{section name=k loop=$category.recommend_item.list[i].child_category.list[j].child_category.list}>
                    <li><a href="<{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].url}>"><{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].name}><{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].code}></a>
                        <!--4階層目-->
                        <{if $category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.has_item}>
                        <ul>
                            <{section name=l loop=$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list}>
                            <li><a href="<{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].url}>"><{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].name}><{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].code}></a>
                                <!--5階層目-->
                                <{if $category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.has_item}>
                                <ul>
                                    <{section name=m loop=$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list}>
                                    <li><a href="<{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].url}>"><{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].name}><{$category.recommend_item.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].code}></a></li>
                                    <{/section}>
                                </ul>
                                <{/if}>
                            </li>
                            <{/section}>
                        </ul>
                        <{/if}>
                    </li>
                    <{/section}>
                </ul>
                <{/if}>
            </li>
            <{/section}>
        </ul>
        <{/if}>
</ul>
<{/section}>
```

#### HTML変換後
```html
<ul>
    <!--1階層目-->
    <li><a href="カテゴリーURL">カテゴリー名ct0</a></li>
        <!--2階層目-->
        <ul>
            <li><a href="サブカテゴリー（2階層目）URL">サブカテゴリー（2階層目）名ct00</a>
                <!--3階層目-->
                <ul>
                    <li><a href="サブカテゴリー（3階層目）URL">サブカテゴリー（3階層目）名ct000</a>
                        <!--4階層目-->
                        <ul>
                            <li><a href="サブカテゴリー（4階層目）URL">サブカテゴリー（4階層目）名ct0000</a>
                                <!--5階層目-->
                                <ul>
                                    <li><a href="サブカテゴリー（5階層目）URL">サブカテゴリー（5階層目）名ct00000</a></li>
                                </ul>
                            </li>
                        </ul>
                    </li>
                </ul>
            </li>
        </ul>
</ul>
```

## $category.recommend_item.list[i].original_code

### 概要
独自商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].original_code}></p>
```

#### HTML変換後
```html
<p>独自商品コード</p>
```

## $category.recommend_item.list[i].system_code

### 概要
システム商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## $category.recommend_item.list[i].point

### 概要
獲得ポイント

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $category.recommend_item.list[i].is_member_price

### 概要
会員割引商品かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.recommend_item.list[i].is_member_price -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.recommend_item.list[i].is_member_price -->
```

## $category.recommend_item.list[i].base_category.name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].base_category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $category.recommend_item.list[i].base_category.url

### 概要
カテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$category.recommend_item.list[i].base_category.url}"></a></p>
```

#### HTML変換後
```html
<p><a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a></p>
```

## $category.recommend_item.list[i].base_category.code

### 概要
カテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].base_category.code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $category.recommend_item.list[i].description

### 概要
商品説明文

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].description}></p>
```

#### HTML変換後
```html
<p>商品説明文</p>
```

## $category.recommend_item.list[i].category_description

### 概要
商品カテゴリーページ用の商品説明文

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].category_description}></p>
```

#### HTML変換後
```html
<p>商品カテゴリーページ用の商品説明文</p>
```

## $category.recommend_item.list[i].manufacturer

### 概要
製造元

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].manufacturer}></p>
```

#### HTML変換後
```html
<p>製造元</p>
```

## $category.recommend_item.list[i].origin_country

### 概要
原産地

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].origin_country}></p>
```

#### HTML変換後
```html
<p>原産地</p>
```

## $category.recommend_item.list[i].special_display

### 概要
商品別特殊表示

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## $category.recommend_item.list[i].is_reservation_sale

### 概要
予約販売商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].is_reservation_sale}>
    <div>
        <{if $category.recommend_item.list[i].has_release_date}>
            <{if !$category.recommend_item.list[i].is_released}>
                <p>販売開始：<{$category.recommend_item.list[i].release_date.year}>年<{$category.recommend_item.list[i].release_date.month}>月<{$category.recommend_item.list[i].release_date.day}>日</p>
            <{/if}>
        <{/if}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $category.recommend_item.list[i].reservation_sale_note

### 概要
備考

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].has_release_date}></p>
```

#### HTML変換後
```html
<p>備考</p>
```

## $category.recommend_item.list[i].has_release_date

### 概要
発売日が設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $category.recommend_item.list[i].has_release_date}>
        <{if !$category.recommend_item.list[i].is_released}>
            <p>販売開始：<{$category.recommend_item.list[i].release_date.year}>年<{$category.recommend_item.list[i].release_date.month}>月<{$category.recommend_item.list[i].release_date.day}>日</p>
        <{/if}>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $category.recommend_item.list[i].is_released

### 概要
発売済みかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if !$category.recommend_item.list[i].is_released}>
        <p>販売開始：<{$category.recommend_item.list[i].release_date.year}>年<{$category.recommend_item.list[i].release_date.month}>月<{$category.recommend_item.list[i].release_date.day}>日</p>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $category.recommend_item.list[i].release_date.year

### 概要
発売日時（年）
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].release_date.year}></p>
```

#### HTML変換後
```html
<p>発売日時（年）</p>
```

## $category.recommend_item.list[i].release_date.month

### 概要
発売日時（月）
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].release_date.month}></p>
```

#### HTML変換後
```html
<p>発売日時（月）</p>
```

## $category.recommend_item.list[i].release_date.day

### 概要
発売日時（日）
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].release_date.day}></p>
```

#### HTML変換後
```html
<p>発売日時（日）</p>
```

## $category.recommend_item.list[i].release_date_note

### 概要
発売日備考
※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$category.recommend_item.list[i].release_date_note}></p>
```

#### HTML変換後
```html
<p>発売日備考</p>
```

## $category.recommend_item.list[i].has_option

### 概要
オプションが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.recommend_item.list[i].has_option -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.recommend_item.list[i].has_option -->
```

## $category.recommend_item.list[i].is_favorite

### 概要
お気に入りに追加済みかどうか

### サンプルコード

#### クリエーターモード
```php
<div class="favorite <{if $category.recommend_item.list[i].is_favorite}>favorite-on<{/if}>">
    <a href="<{$category.recommend_item.list[i].favorite_entry_url}>"></a>
</div>
```

#### HTML変換後
```html
<div class="favorite favorite-on">
    <a href="#makeshop-common-favorite-entry-url:商品URL番号"></a>
</div>
```

## $category.recommend_item.list[i].favorite_entry_url

### 概要
お気に入りに追加URL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$category.recommend_item.list[i].favorite_entry_url}>"></a></div>
```

#### HTML変換後
```html
<div><a href="#makeshop-common-favorite-entry-url:商品URL番号"></a></div>
```

## $category.recommend_item.list[i].favorite_remove_url

### 概要
お気に入りから削除URL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$category.item.list[i].favorite_remove_url}>"></a></div>
```

#### HTML変換後
```html
<div><a href="お気に入りから削除URL"></a></div>
```

## $category.recommend_item.list[i].icon.has_item

### 概要
アイコンが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.recommend_item.list[i].icon.has_item}>
    <div>
        <ul>
            <{section name=j loop=$category.recommend_item.list[i].icon.list}>
                <li>
                    <img src="<{$category.recommend_item.list[i].icon.list[j].image_url}>">
                </li>
            <{/section}>
        </ul>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <ul>
        <li>
            <img src="アイコン画像URL">
        </li>
    </ul>
</div>
```

## $category.recommend_item.list[i].icon.list[j].image_url

### 概要
アイコン画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.recommend_item.list[i].icon.list[j].image_url}>" ></div>
```

#### HTML変換後
```html
<div><img src="アイコン画像URL.jpg" ></div>
```

# サブカテゴリー一覧

## $category.child_category.has_item

### 概要
サブカテゴリーがあるかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.child_category.has_item}>
  <ul>
      <{section name=i loop=$category.child_category.list}>
          <li>
              <a href="<{$category.child_category.list[i].url}>"><{$category.child_category.list[i].name}><span>（<{$category.child_category.list[i].item_count}>）</span></a>
          </li>
      <{/section}>
  </ul>
<{/if}>
```

#### HTML変換後
```html
<ul>
  <li>
      <a href="サブカテゴリーURL">サブカテゴリー名<span>（サブカテゴリーの総商品数）</span></a>
  </li>
</ul>
```

## $category.child_category.list[i].name

### 概要
サブカテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$category.child_category.list[i].name}></p>
```

#### HTML変換後
```html
<p>サブカテゴリー名</p>
```

## $category.child_category.list[i].url

### 概要
サブカテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$category.child_category.list[i].url}>"><{$category.child_category.list[i].name}></a>
```

#### HTML変換後
```html
<a href="サブカテゴリーURL">サブカテゴリー名</a>
```

## $category.child_category.list[i].item_count

### 概要
サブカテゴリーの総商品数

### サンプルコード

#### クリエーターモード
```php
<p>
    <a href="<{$category.child_category.list[i].url}>"><{$category.child_category.list[i].name}>
    <span>（<{$category.child_category.list[i].item_count}>）</span></a>
</p>
```

#### HTML変換後
```html
<p>
    <a href="サブカテゴリーURL">サブカテゴリー名
    <span>（サブカテゴリーの総商品数）</span></a>
</p>
```

# ページャー

## $category.pager.has_item

### 概要
ページャーがあるかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.pager.has_item}>
    <ul>
        <{if !$category.pager.is_first_display}>
            <li><a href="<{$category.pager.first_url}>"><span>一番前へ</span></a></li>
        <{/if}>
            
        <{section name=i loop=$category.pager.list}>
            <{if $category.pager.list[i].is_current_page}>
                <li><span><{$category.pager.list[i].number}></span></li>
            <{else}>
                <li><a href="<{$category.pager.list[i].url}>"><span><{$category.pager.list[i].number}></span></a></li>
            <{/if}>
        <{/section}>
            
        <{if !$category.pager.is_last_display}>
            <li><a href="<{$category.pager.last_url}>"><span>最後へ</span></a></li>
        <{/if}>
    </ul>
 <{/if}>
```

#### HTML変換後
```html
<ul>
    <li><a href="/view/review/0商品URL?page=最初のページ">一番前へ</a></li>
    <li><a href="ページURL">ページ番号</a></li>
    <li><a href="/view/review/0商品URL?page=最後のページ">最後のページへ</a></li>
</ul>
```

## $category.pager.is_first

### 概要
表示中のページが最初のページかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.pager.is_first -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.pager.is_first -->
```

## $category.pager.is_first_display

### 概要
最初のページ番号が表示されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if !$category.pager.is_first_display}>
    <li><a href="<{$category.pager.first_url}>">一番前へ</a></li>
<{/if}>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最初のページ">一番前へ</a></li>
```

## $category.pager.first_url

### 概要
最初のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$category.pager.first_url}>">一番前へ</a></li>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最初のページ">一番前へ</a></li>
```

## $category.pager.prev_url

### 概要
前のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$category.pager.prev_url}>">前のページへ</a></li>
```

#### HTML変換後
```html
<li><a href="前のページURL">前のページへ</a></li>
```

## $category.pager.is_last

### 概要
表示中のページが最後のページかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $category.pager.is_last -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $category.pager.is_last -->
```

## $category.pager.is_last_display

### 概要
最後のページ番号が表示されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if !$category.pager.is_last_display}>
    <li><a href="<{$category.pager.last_url}>">最後へ</a></li>
<{/if}>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最後のページ">最後へ</a></li>
```

## $category.pager.last_url

### 概要
最後のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$category.pager.last_url}>">前のページへ</a></li>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最後のページ">最後のページへ</a></li>
```

## $category.pager.last_number

### 概要
最終ページ数

### サンプルコード

#### クリエーターモード
```php
<p><{$category.pager.last_number}></p>
```

#### HTML変換後
```html
<p>最終ページ数</p>
```

## $category.pager.next_url

### 概要
次のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$category.pager.next_url}>">次のページへ</a></li>
```

#### HTML変換後
```html
<li><a href="次のページURL">次のページへ</a></li>
```

## $category.pager.list[i].number

### 概要
ページ番号

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$category.pager.list[i].url}>"><{$category.pager.list[i].number}></a></li>
```

#### HTML変換後
```html
<li><a href="ページURL">ページ番号</a></li>
```

## $category.pager.list[i].url

### 概要
ページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$category.pager.list[i].url}>"><{$category.pager.list[i].number}></a></li>
```

#### HTML変換後
```html
<li><a href="ページURL">ページ番号</a></li>
```

## $category.pager.list[i].is_current_page

### 概要
表示中のページかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category.pager.list[i].is_current_page}>
    <div><{$category.pager.list[i].number}></div>
<{else}>
    <div><a href="<{$category.pager.list[i].url}>"><{$category.pager.list[i].number}></a></div>
<{/if}>
```

#### HTML変換後
```html
<div>ページ番号</div>
<div><a href="ページURL">ページ番号</a></div>
```

# まとめ買い割引情報

## $bulk.name

### 概要
まとめ買い割引名

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.name}></p>
```

#### HTML変換後
```html
<p>よりどり割引（定額割引）</p>
```

## $bulk.display_count_from

### 概要
一覧に表示する開始商品数

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.display_count_from}></p>
```

#### HTML変換後
```html
<p>一覧に表示する開始商品数</p>
```

## $bulk.display_count_to

### 概要
一覧に表示する終了商品数

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.display_count_to}></p>
```

#### HTML変換後
```html
<p>一覧に表示する終了商品数</p>
```

## $bulk.display_count

### 概要
表示商品数

### サンプルコード

#### クリエーターモード
```php
<p>（全<span><{$bulk.total_count}></span>件）<{$bulk.display_count}>件表示</p>
```

#### HTML変換後
```html
<p>（全<span>総商品数</span>件）表示商品数件表示</p>
```

## $bulk.total_count

### 概要
総商品数

### サンプルコード

#### クリエーターモード
```php
<p>（全<span><{$category.total_count}></span>件）<{$category.display_count}>件表示</p>
```

#### HTML変換後
```html
<p>（全<span>総商品数</span>件）表示商品数件表示</p>
```

## $bulk.is_set_discount

### 概要
セット割引かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.is_set_discount}>
    <div>
        <{if $bulk.is_group1_current}>
            <{$bulk.group1_name}>
        <{else}>
            <a href="<{$bulk.group1_url}>"><{$bulk.group1_name}></a>
        <{/if}>
        ／
        <{if $bulk.is_group2_current}>
            <{$bulk.group2_name}>
        <{else}>
            <a href="<{$bulk.group2_url}>"><{$bulk.group2_name}></a>
        <{/if}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>セット割引のグループAの名前／セット割引のグループBの名前</div>
```

## $bulk.group1_name

### 概要
セット割引のグループAの名前

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.group1_url}>"><{$bulk.group1_name}></a></div>
```

#### HTML変換後
```html
<div><a href="/view/bulk/1-1">セット割引のグループAの名前</a></div>
```

## $bulk.group1_url

### 概要
セット割引のグループAのURL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.group1_url}>"><{$bulk.group1_name}></a></div>
```

#### HTML変換後
```html
<div><a href="/view/bulk/1-1">セット割引のグループAの名前</a></div>
```

## $bulk.is_group1_current

### 概要
セット割引のグループAが表示されているかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $bulk.is_group1_current}>
        <{$bulk.group1_name}>
    <{else}>
        <a href="<{$bulk.group1_url}>"><{$bulk.group1_name}></a>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>セット割引のグループAの名前</div>
```

## $bulk.group2_name

### 概要
セット割引のグループBの名前

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.group2_url}>"><{$bulk.group2_name}></a></div>
```

#### HTML変換後
```html
<div><a href="/view/bulk/1-2">セット割引のグループBの名前</a></div>
```

## $bulk.group2_url

### 概要
セット割引のグループBのURL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.group2_url}>"><{$bulk.group2_name}></a></div>
```

#### HTML変換後
```html
<div><a href="/view/bulk/1-2">セット割引のグループBの名前</a></div>
```

## $bulk.is_group2_current

### 概要
セット割引のグループBが表示されているかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $bulk.is_group2_current}>
        <{$bulk.group2_name}>
    <{else}>
        <a href="<{$bulk.group2_url}>"><{$bulk.group2_name}></a>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>セット割引のグループBの名前</div>
```

# まとめ買い割引一覧

## $bulk.item.list[i].num

### 概要
連番

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].num -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].num -->
```

## $bulk.item.list[i].name

### 概要
商品名

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$bulk.item.list[i].url}>"><{$bulk.item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品URL">商品名</a></p>
```

## $bulk.item.list[i].price

### 概要
商品価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$bulk.item.list[i].price}>（税込）</p>
```

#### HTML変換後
```html
<p>￥販売価格（税込）</p>
```

## $bulk.item.list[i].price_excluded_tax

### 概要
税抜き価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$bulk.item.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き価格</p>
```

## $bulk.item.list[i].tax

### 概要
税

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].tax}></p>
```

#### HTML変換後
```html
<p>消費税額</p>
```

## $bulk.item.list[i].tax_rate

### 概要
消費税率

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].tax_rate}>%</p>
```

#### HTML変換後
```html
<p>10%</p>
```

## $bulk.item.list[i].is_reduced_tax_rate

### 概要
軽減税率かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].is_reduced_tax_rate -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].is_reduced_tax_rate -->
```

## $bulk.item.list[i].original_price

### 概要
通常価格（税込）

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$bulk.item.list[i].original_price}></p>
```

#### HTML変換後
```html
<p>￥通常価格</p>
```

## $bulk.item.list[i].original_price_excluded_tax

### 概要
通常価格（税抜）

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$bulk.item.list[i].original_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き通常価格</p>
```

## $bulk.item.list[i].original_tax

### 概要
通常価格の税

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].original_tax}></p>
```

#### HTML変換後
```html
<p>通常価格の税</p>
```

## $bulk.item.list[i].fixed_price

### 概要
定価

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$bulk.item.list[i].fixed_price}></p>
```

#### HTML変換後
```html
<p>￥定価</p>
```

## $bulk.item.list[i].url

### 概要
商品詳細画面URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$bulk.item.list[i].url}>"><{$bulk.item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品URL">商品名</a></p>
```

## $bulk.item.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$bulk.item.list[i].image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="商品縮小画像パス.jpg"></div>
```

## $bulk.item.list[i].image_M

### 概要
商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$bulk.item.list[i].image_M}>"></div>
```

#### HTML変換後
```html
<div><img src="商品普通画像パス.jpg"></div>
```

## $bulk.item.list[i].image_L

### 概要
商品画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$bulk.item.list[i].image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="商品画像パス.jpg"></div>
```

## $bulk.item.list[i].is_stock_display

### 概要
在庫表示可かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].is_stock_display}>
    <{if $bulk.item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $bulk.item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$bulk.item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$bulk.item.list[i].stock_quantity}>個</span></p>
        <{/if}>
    <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## $bulk.item.list[i].is_stock_unlimited

### 概要
在庫無制限商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $bulk.item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$bulk.item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$bulk.item.list[i].stock_quantity}>個</span></p>
        <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## $bulk.item.list[i].is_soldout

### 概要
売り切れかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].is_soldout}>
    <div>売り切れ</div>
<{else}>
    <a href="<{$bulk.item.list[i].cart_entry_url}>">カートに入れる</a>
<{/if}>
```

#### HTML変換後
```html
<div>売り切れ</div>
```

## $bulk.item.list[i].is_small_stock

### 概要
在庫が指定された数以下かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].is_small_stock}>
        <p>△残りわずか<span>あと<{$bulk.item.list[i].stock_quantity}>個</span></p>
    <{else}>
        <p>〇在庫あり<span>あと●●個</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり<span>あと●●個</span></p>
```

## $bulk.item.list[i].stock_quantity

### 概要
在庫数

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## $bulk.item.list[i].is_sale

### 概要
セール商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].is_sale}>
    <p>￥<{$bulk.item.list[i].original_price|number_format}><span>（税込）</span></p>
    <p>￥<{$bulk.item.list[i].price|number_format}><span>（税込）</span>
    <span>[<{$bulk.item.list[i].sale_rate}>%OFF</span>]</p>
<{else}>
    <p>￥<{$bulk.item.list[i].price|number_format}><span>（税込）</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>￥通常価格<span>（税込）</span></p>
<p>￥セール価格<span>（税込）</span><span>[●●%OFF</span>]</p>
```

## $bulk.item.list[i].sale_rate

### 概要
セール割引率

### サンプルコード

#### クリエーターモード
```php
<p><{$category.item$bulk.item.list[i].sale_rate}>%OFF</p>
```

#### HTML変換後
```html
<p>●●%OFF</p>
```

## $bulk.item.list[i].has_reiview

### 概要
旧レビューが投稿されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].has_review}>
    <div>
        <{$bulk.item.list[i].review.star_html}>
        <p><{$bulk.item.list[i].review.average}></p>
        <p>[<{$bulk.item.list[i].review.total_count}>件]</p>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <div class="reviewRate">
        <div class="reviewRateStar starOn">評価1</div>
        <div class="reviewRateStar starOn">評価2</div>
        <div class="reviewRateStar staron">評価3</div>
        <div class="reviewRateStar starOff">評価4</div>
        <div class="reviewRateStar starOff">評価5</div>
    </div>
    <p>平均レビュー点数</p>
    <p>[●●件]</p>
</div>
```

## $bulk.item.list[i].review.star_html

### 概要
旧レビュー評価（星）

### サンプルコード

#### クリエーターモード
```php
<div><{$bulk.item.list[i].review.star_html}></div>
```

#### HTML変換後
```html
<div class="reviewRate">
    <div class="reviewRateStar starOn">評価1</div>
    <div class="reviewRateStar starOn">評価2</div>
    <div class="reviewRateStar staron">評価3</div>
    <div class="reviewRateStar starOff">評価4</div>
    <div class="reviewRateStar starOff">評価5</div>
</div>
```

## $bulk.item.list[i].review.average

### 概要
旧平均レビュー点数

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].review.average}></p>
```

#### HTML変換後
```html
<p>平均レビュー点数</p>
```

## $bulk.item.list[i].review.total_count

### 概要
旧レビュー投稿数

### サンプルコード

#### クリエーターモード
```php
<p>[<{$bulk.item.list[i].review.total_count}>件]</p>
```

#### HTML変換後
```html
<p>[●●件]</p>
```

## $bulk.item.list[i].review.url

### 概要
旧レビュー一覧URL

### サンプルコード

#### クリエーターモード
```php
<p>[<a href="<{$bulk.item.list[i].review.url}>"><{$bulk.item.list[i].review.total_count}>件</a>]</p>
```

#### HTML変換後
```html
<p>[<a href="/view/review/レビュー一覧URL">●●件</a>]</p>
```

## $bulk.item.list[i].icon.has_item

### 概要
アイコンが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].icon.has_item}>
    <div>
        <ul>
            <{section name=j loop=$bulk.item.list[i].icon.list}>
                <li>
                    <img src="<{$bulk.item.list[i].icon.list[j].image_url}>">
                </li>
            <{/section}>
        </ul>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <ul>
        <li>
            <img src="アイコン画像URL">
        </li>
    </ul>
</div>
```

## $bulk.item.list[i].icon.list[j].image_url

### 概要
アイコン画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$category.item.list[i].icon.list[j].image_url}>" ></div>
```

#### HTML変換後
```html
<div><img src="アイコン画像URL.jpg" ></div>
```

## $bulk.item.list[i].original_code

### 概要
独自商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].original_code}></p>
```

#### HTML変換後
```html
<p>独自商品コード</p>
```

## $bulk.item.list[i].system_code

### 概要
システム商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## $bulk.item.list[i].point

### 概要
獲得ポイント

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $bulk.item.list[i].is_member_price

### 概要
会員割引商品かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].is_member_price -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].is_member_price -->
```

## $bulk.item.list[i].base_category.name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].base_category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $bulk.item.list[i].base_category.url

### 概要
カテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$bulk.item.list[i].base_category.url}"></a></p>
```

#### HTML変換後
```html
<p><a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a></p>
```

## $bulk.item.list[i].base_category.code

### 概要
カテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk-item-list-base-category-code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $bulk.item.list[i].description

### 概要
商品説明文（PC）

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].description}></p>
```

#### HTML変換後
```html
<p>商品説明文</p>
```

## $bulk.item.list[i].category_description

### 概要
商品カテゴリーページ用の商品説明文

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].category_description}></p>
```

#### HTML変換後
```html
<p>商品カテゴリーページ用の商品説明文</p>
```

## $bulk.item.list[i].has_option

### 概要
オプションが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].has_option -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.item.list[i].has_option -->
```

## $bulk.item.list[i].manufacturer

### 概要
製造元

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].manufacturer}></p>
```

#### HTML変換後
```html
<p>製造元</p>
```

## $bulk.item.list[i].origin_country

### 概要
原産地

### サンプルコード

#### クリエーターモード
```php
<p><{bulk-item-list-origin-country}></p>
```

#### HTML変換後
```html
<p>原産地</p>
```

## $bulk.item.list[i].special_display

### 概要
商品別特殊表示

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## $bulk.item.list[i].is_reservation_sale

### 概要
予約販売商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.item.list[i].is_reservation_sale}>
    <div>
        <{if $bulk.item.list[i].has_release_date}>
            <{if !$bulk.item.list[i].is_released}>
                <p>販売開始：<{$bulk.item.list[i].release_date.year}>年<{$bulk.item.list[i].release_date.month}>月<{$bulk.item.list[i].release_date.day}>日</p>
            <{/if}>
        <{/if}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $bulk.item.list[i].reservation_sale_note

### 概要
予約販売商品の備考

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].reservation_sale_note}></p>
```

#### HTML変換後
```html
<p>備考</p>
```

## $bulk.item.list[i].has_release_date

### 概要
発売日が設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $bulk.item.list[i].has_release_date}>
        <{if !$bulk.item.list[i].item.is_released}>
            <p>販売開始：<{$bulk.item.list[i].release_date.year}>年<{$bulk.item.list[i].release_date.month}>月<{$bulk.item.list[i].release_date.day}>日</p>
        <{/if}>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $bulk.item.list[i].item.is_released

### 概要
発売済みかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if !$bulk.item.list[i].item.is_released}>
        <p>販売開始：<{$bulk.item.list[i].release_date.year}>年<{$bulk.item.list[i].release_date.month}>月<{$bulk.item.list[i].release_date.day}>日</p>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>販売開始：●●●●年●●月●●日</p>
</div>
```

## $bulk.item.list[i].release_date.year

### 概要
発売日時（年）※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].release_date.year}></p>
```

#### HTML変換後
```html
<p>発売日時（年）</p>
```

## $bulk.item.list[i].release_date.month

### 概要
発売日時（月）※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].release_date.month}></p>
```

#### HTML変換後
```html
<p>発売日時（月）</p>
```

## $bulk.item.list[i].release_date.day

### 概要
発売日時（日）※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].release_date.day}></p>
```

#### HTML変換後
```html
<p>発売日時（日）</p>
```

## $bulk.item.list[i].release_date_note

### 概要
発売日備考　※予約販売商品のみ表示されます

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.item.list[i].release_date_note}></p>
```

#### HTML変換後
```html
<p>発売日備考</p>
```

## $bulk.item.list[i].is_favorite

### 概要
お気に入りに追加済みかどうか

### サンプルコード

#### クリエーターモード
```php
<div class="favorite <{if $bulk.item.list[i].is_favorite}>favorite-on<{/if}>">
    <a href="<{$bulk.item.list[i].favorite_entry_url}>"></a>
</div>
```

#### HTML変換後
```html
<div class="favorite favorite-on">
    <a href="#makeshop-common-favorite-entry-url:商品URL番号"></a>
</div>
```

## $bulk.item.list[i].favorite_entry_url

### 概要
お気に入りに追加URL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.item.list[i].is_favorite}>"></a></div>
```

#### HTML変換後
```html
<div><a href="#makeshop-common-favorite-entry-url:商品URL番号"></a></div>
```

## $bulk.item.list[i].favorite_remove_url

### 概要
お気に入りから削除URL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.item.list[i].favorite_remove_url}>"></a></div>
```

#### HTML変換後
```html
<div><a href="お気に入りから削除URL"></a></div>
```

## $bulk.item.list[i].cart_entry_url

### 概要
かごに入れるURL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$bulk.item.list[i].cart_entry_url}>">カートに入れる</a></div>
```

#### HTML変換後
```html
<div><a href="かごに入れるURL">カートに入れる</a></div>
```

# 並び替え（まとめ買い）

## $bulk.sort_recommend_url

### 概要
並び替えURL（おすすめ順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$bulk.sort_recommend_url}>">おすすめ順</a></dd>
```

#### HTML変換後
```html
<dd><a href="並び替えURL（おすすめ順）">おすすめ順</a></dd>
```

## $bulk.sort_new_url

### 概要
並び替えURL（新着順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$bulk.sort_new_url}>">新着順</a></dd>
```

#### HTML変換後
```html
<dd><a href="並び替えURL（新着順）">新着順</a></dd>
```

## $bulk.sort_high_price_url

### 概要
並び替えURL（価格が高い順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$bulk.sort_high_price_url}>">価格の高い順</a></dd>
```

#### HTML変換後
```html
<dd><a href="並び替えURL（価格が高い順）">価格の高い順</a></dd>
```

## $bulk.sort_low_price_url

### 概要
並び替えURL（価格が低い順）

### サンプルコード

#### クリエーターモード
```php
<dd><a href="<{$bulk.sort_low_price_url}>">価格の低い順</a></dd>
```

#### HTML変換後
```html
<dd><a href="並び替えURL（価格が低い順）">価格の低い順</a></dd>
```

## $bulk.is_sort_recommend_selected

### 概要
おすすめ順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_recommend_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_recommend_selected -->
```

## $bulk.is_sort_new_selected

### 概要
新着順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_new_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_new_selected -->
```

## $bulk.sort_name_url

### 概要
並び替えURL（商品名順）

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.sort_name_url -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.sort_name_url -->
```

## $bulk.is_sort_name_selected

### 概要
商品名順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_name_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_name_selected -->
```

## $bulk.sort_manufacturer_url

### 概要
並び替えURL（製造元順）

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.sort_manufacturer_url -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.sort_manufacturer_url -->
```

## $bulk.is_sort_manufacturer_selected

### 概要
製造元順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_manufacturer_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_manufacturer_selected -->
```

## $bulk.is_sort_high_price_selected

### 概要
高価格順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_high_price_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_high_price_selected -->
```

## $bulk.is_sort_low_price_selected

### 概要
低価格順かどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_low_price_selected -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.is_sort_low_price_selected -->
```

# ページャー（まとめ買い割引）

## $bulk.pager.is_first

### 概要
表示中のページが最初のページかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.pager.is_first -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.pager.is_first -->
```

## $bulk.pager.is_first_display

### 概要
最初のページ番号が表示されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if !$bulk.pager.is_first_display}>
    <li><a href="<{$bulk.pager.first_url}>">一番前へ</a></li>
<{/if}>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最初のページ">一番前へ</a></li>
```

## $bulk.pager.first_url

### 概要
最初のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$bulk.pager.first_url}>">一番前へ</a></li>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最初のページ">一番前へ</a></li>
```

## $bulk.pager.prev_url

### 概要
前のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$bulk.pager.prev_url}>">前のページへ</a></li>
```

#### HTML変換後
```html
<li><a href="前のページURL">前のページへ</a></li>
```

## $bulk.pager.is_last

### 概要
表示中のページが最後のページかどうか

### サンプルコード

#### クリエーターモード
```php
<!-- 公式一覧に詳細ページリンクなし: $bulk.pager.is_last -->
```

#### HTML変換後
```html
<!-- 公式一覧に詳細ページリンクなし: $bulk.pager.is_last -->
```

## $bulk.pager.is_last_display

### 概要
最後のページ番号が表示されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if !$bulk.pager.is_last_display}>
    <li><a href="<{$bulk.pager.last_url}>">最後へ</a></li>
<{/if}>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最後のページ">最後へ</a></li>
```

## $bulk.pager.last_url

### 概要
最後のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$bulk.pager.last_url}>">前のページへ</a></li>
```

#### HTML変換後
```html
<li><a href="/view/review/0商品URL?page=最後のページ">最後のページへ</a></li>
```

## $bulk.pager.last_number

### 概要
最終ページ数

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk.pager.last_number}></p>
```

#### HTML変換後
```html
<p>最終ページ数</p>
```

## $bulk.pager.next_url

### 概要
次のページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$bulk.pager.next_url}>">次のページへ</a></li>
```

#### HTML変換後
```html
<li><a href="次のページURL">次のページへ</a></li>
```

## $bulk.pager.list[i].number

### 概要
ページ番号

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$bulk.pager.list[i].url}>"><{$bulk.pager.list[i].number}></a></li>
```

#### HTML変換後
```html
<li><a href="ページURL">ページ番号</a></li>
```

## $bulk.pager.list[i].url

### 概要
ページURL

### サンプルコード

#### クリエーターモード
```php
<li><a href="<{$bulk.pager.list[i].url}>"><{$bulk.pager.list[i].number}></a></li>
```

#### HTML変換後
```html
<li><a href="ページURL">ページ番号</a></li>
```

## $bulk.pager.list[i].is_current_page

### 概要
表示中のページかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk.pager.list[i].is_current_page}>
    <div><{$bulk.pager.list[i].number}></div>
<{else}>
    <div><a href="<{$bulk.pager.list[i].url}>"><{$bulk.pager.list[i].number}></a></div>
<{/if}>
```

#### HTML変換後
```html
<div>ページ番号</div>
<div><a href="ページURL">ページ番号</a></div>
```
