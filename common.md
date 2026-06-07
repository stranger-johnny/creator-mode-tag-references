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
<body>
    <!-- 事前に定義したbodyタグ上部の定義が出力 -->
</body>
```

## $makeshop.body_bottom

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
<body>
    <!-- 事前に定義したbodyタグ下部の定義が出力 -->
</body>
```

# ページ情報

## $page.type

### 概要
ページタイプ

- ページタイプ一覧
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
<div class="<{$page.type}>">〜</div>
```

#### HTML変換後
```html
<div class="category">〜</div>
```

## $page.id

### 概要
ページID

- ページID一覧
  - カテゴリー：カテゴリー識別コード
  - 商品詳細：システム商品コード
  - 商品レビュー一覧：システム商品コード
  - 商品レビュー投稿：システム商品コード
  - お知らせ詳細：お知らせ詳細URL末尾
  - まとめ買い割引：まとめ買い割引URL末尾
  - フリーページ：フリーページURL末尾
  - 上記以外は空になります

### サンプルコード

#### クリエーターモード
```php
<div id="<{$page.id}>">〜</div>
```

#### HTML変換後
```html
<div id="ct1">〜</div>
```

## $page.title

### 概要
ページタイトル

### サンプルコード

#### クリエーターモード
```php
<meta property="og:title" content="<{$page.title}>">
```

#### HTML変換後
```html
<meta property="og:title" content="雑貨を取り扱うオンラインショップ">
```

## $page.description

### 概要
ページdescription

### サンプルコード

#### クリエーターモード
```php
<meta property="og:description" content="<{$page.description}>">
```

#### HTML変換後
```html
<meta property="og:description" content="当店は豊富な品揃えの雑貨ショップです。おしゃれで実用的なアイテムを取り揃えており、お客様のライフスタイルに合ったアイテムを見つけていただけます。">
```

## $page.canonical_url

### 概要
canonicalURL

### サンプルコード

#### クリエーターモード
```php
<link rel="canonical" href="<{$page.canonical_url}>">
```

#### HTML変換後
```html
<link rel="canonical" href="https://www.example.com/">
```

## $page.css

### 概要
CSSファイルURL

### サンプルコード

#### クリエーターモード
```php
<link rel="stylesheet" href="<{$page.css}>">
```

#### HTML変換後
```html
<link rel="stylesheet" href="/view/asset/sample.css">
```

## $page.javascript

### 概要
JavaScriptファイルURL

### サンプルコード

#### クリエーターモード
```php
<script src="<{$page.javascript}>"></script>
```

#### HTML変換後
```html
<script src="/view/asset/sample.js"></script>
```

# ショップ情報

## $shop.name

### 概要
ショップ名

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$url.top}>"><{$shop.name}></a></p>
```

#### HTML変換後
```html
<p><a href="/">ショップの名前</a></p>
```

## $shop.logo_url

### 概要
ショップロゴ画像URL

### サンプルコード

#### クリエーターモード
```php
<img src="<{$shop.logo_url}>" alt="<{$shop.name}>">
```

#### HTML変換後
```html
<img src="画像パス" alt="ショップの名前">
```

## $shop.favicon_url

### 概要
ファビコン画像URL

### サンプルコード

#### クリエーターモード
```php
<link rel="shortcut icon" type="image/ico" href="<{$shop.favicon_url}>">
```

#### HTML変換後
```html
<link rel="shortcut icon" type="image/ico" href="/favicon.ico">
```

## $shop.mainvisual

### 概要
メインビジュアル（トップページイメージ）

### サンプルコード

#### クリエーターモード
```php
<{if $shop.mainvisual}>
    <section>
        <{$shop.mainvisual}>
    </section>
<{/if}>
```

#### HTML変換後
画像１枚だけの場合
```html
<section>
    <img src="画像パス" class="topImage">
</section>
```

画像が複数枚の場合
```html
<section>
    <ul id="M_slider">
        <li class="M_sliderFirstImage"><img src="画像パス"></li>
        <li style="display:none;"><img src="画像パス"></li>
        <li style="display:none;"><img src="画像パス"></li>
        <li style="display:none;"><img src="画像パス"></li>
        <li style="display:none;"><img src="画像パス"></li>
    </ul>
</section>
```

## $shop.comment

### 概要
ショップコメント（トップページデザイン）

### サンプルコード

#### クリエーターモード
```php
<{if $shop.comment}>
    <p><{$shop.comment}></p>
<{/if}>
```

#### HTML変換後
```html
<p>入力したテキスト</p>
```

## $shop.address

### 概要
ショップ住所

### サンプルコード

#### クリエーターモード
```php
<p><{$shop.address}></p>
```

#### HTML変換後
```html
<p>東京都渋谷区桜丘町26-1セルリアンタワー</p>
```

## $shop.tel

### 概要
お問い合わせ先電話番号

### サンプルコード

#### クリエーターモード
```php
<p><{$shop.tel}></p>
```

#### HTML変換後
```html
<p>03-5728-6236</p>
```

## $shop.copyright

### 概要
ショップコピーライト

### サンプルコード

#### クリエーターモード
```php
<p><{$shop.copyright}></p>
```

#### HTML変換後
```html
<p>©20xx shopname All Rights Reserved.</p>
```

## $shop.is_point_enabled

### 概要
ポイント利用可能なショップかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $shop.is_point_enabled && $item.point !== 0}>
    <p><{$item.point_html}>ポイント獲得</p>
<{/if}>
```

#### HTML変換後
```html
<p>100ポイント獲得</p>
```

## $shop.is_mail_magazine_enabled

### 概要
メールマガジン利用可能なショップかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $shop.is_mail_magazine_enabled}>
    <p><a href="<{$url.mail_magazine}>">メールマガジン登録</a></p>
<{/if}>
```

#### HTML変換後
```html
<p><a href="メールマガジン会員登録用URL">メールマガジン登録</a></p>
```

## $shop.is_member_entry_enabled

### 概要
会員登録画面を表示するかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $shop.is_member_entry_enabled}>
    <p><a href="<{$url.member_entry}>">会員登録</a></p>
<{/if}>
```

#### HTML変換後
```html
<p><a href="会員登録ページURL">会員登録</a></p>
```

## $url.mail_magazine

### 概要
メールマガジン会員登録用URL

### サンプルコード

#### クリエーターモード
```php
<{if $shop.is_mail_magazine_enabled}>
    <p><a href="<{$url.mail_magazine}>">メールマガジン登録</a></p>
<{/if}>
```

#### HTML変換後
```html
<p><a href="メールマガジン会員登録用URL">メールマガジン登録</a></p>
```

## $paid.is_enabled

### 概要
Paid決済を利用中かどうか（真偽値）

### サンプルコード

#### クリエーターモード
```php
<{if $paid.is_enabled}>
    <p><a href="<{$paid.entry_url}>">Paid決済をご利用する</a></p>
<{/if}>
```

#### HTML変換後
```html
<p><a href="Paid会員登録URL">Paid決済をご利用する</a></p>
```

## $paid.entry_url

### 概要
Paid会員登録URL

### サンプルコード

#### クリエーターモード
```php
<{if $paid.is_enabled}>
    <p><a href="<{$paid.entry_url}>">Paid決済をご利用する</a></p>
<{/if}>
```

#### HTML変換後
```html
<p><a href="Paid会員登録URL">Paid決済をご利用する</a></p>
```

# バナー

## $shop.banner.has_item

### 概要
バナー画像が登録されているか

### サンプルコード

#### クリエーターモード
```php
<{if $shop.banner.has_item}>
    <section>
        <{section name=i loop=$shop.banner.list}>
            <a href="<{$shop.banner.list[i].url}>" target="<{$shop.banner.list[i].target}>"><img src="<{$shop.banner.list[i].image_url}>"></a>
        <{/section}>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section class="banner-area">
    <a href="バナーリンクURL" target="_blank"><img src="バナー画像パス">
    <a href="バナーリンクURL" target="_blank"><img src="バナー画像パス">
    <a href="バナーリンクURL" target="_blank"><img src="バナー画像パス">
    <a href="バナーリンクURL" target="_blank"><img src="バナー画像パス">
    <a href="バナーリンクURL" target="_blank"><img src="バナー画像パス">
</section>
```

## $shop.banner.list[i].image_url

### 概要
バナー画像URL

### サンプルコード

#### クリエーターモード
```php
<img src="<{$shop.banner.list[i].image_url}>">
```

#### HTML変換後
```html
<img src="バナー画像パス">
```

## $shop.banner.list[i].url

### 概要
バナーリンク先URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$shop.banner.list[i].url}>"></a>
```

#### HTML変換後
```html
<a href="バナーURL"></a>
```

## $shop.banner.list[i].target

### 概要
バナーリンクターゲット属性

### サンプルコード

#### クリエーターモード
```php
<a href="<{$shop.banner.list[i].url}>" target="<{$shop.banner.list[i].target}>"></a>
```

#### HTML変換後
```html
<a href="バナーリンクURL" target="_blank"></a>
```

# ページリンク

## $url.top

### 概要
ショップトップページURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.top}>"></a>
```

#### HTML変換後
```html
<a href="/"></a>
```

## $url.news

### 概要
お知らせ一覧URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.news}>">お知らせ一覧へ</a>
```

#### HTML変換後
```html
<a href="/view/news/list"></a>
```

## $url.guide

### 概要
利用案内URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.guide}>">ご利用ガイド</a>
```

#### HTML変換後
```html
<a href="/view/guide"></a>
```

## $url.company

### 概要
会社概要URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.company}>">会社概要</a>
```

#### HTML変換後
```html
<a href="/view/company"></a>
```

## $url.contract

### 概要
特定商取引法URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.contract}>">特定商取引に関する表記</a>
```

#### HTML変換後
```html
<a href="/view/contract"></a>
```

## $url.policy

### 概要
プライバシーポリシーURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.policy}>">プライバシーポリシー</a>
```

#### HTML変換後
```html
<a href="/view/policy"></a>
```

## $url.support

### 概要
お問い合わせURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.support}>">お問い合わせ</a>
```

#### HTML変換後
```html
<a href="#makeshop-common-contact-url"></a>
```

## $url.login

### 概要
ログインURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.login}>">ログイン</a>
```

#### HTML変換後
```html
<a href="/view/member/login"></a>
```

## $url.member_entry

### 概要
会員登録URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.member_entry}>">新規会員登録</a>
```

#### HTML変換後
```html
<a href="https://www.makeshop.jp/ssl/?ssltype=ssl_shop_member_entry&k=●●●●●●●"></a>
```

## $url.mypage

### 概要
マイページURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.mypage}>">マイページ</a>
```

#### HTML変換後
```html
<a href="/view/member/mypage"></a>
```

## $url.order_history

### 概要
購入履歴URL（非会員の場合も同じ）

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.order_history}>">購入履歴</a>
```

#### HTML変換後
```html
<a href="/view/member/order-history"></a>
```

## $url.member_edit

### 概要
会員情報変更URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.member_edit}>">会員情報変更</a>
```

#### HTML変換後
```html
<a href="/view/member/member-edit"></a>
```

## $url.point

### 概要
ポイント照会URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.point}>">ポイント照会</a>
```

#### HTML変換後
```html
<a href="/view/member/point"></a>
```

## $url.logout

### 概要
ログアウトURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.logout}>">ログアウト</a>
```

#### HTML変換後
```html
<a href="/shop/logout.html"></a>
```

## $url.catalog

### 概要
カタログURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.catalog}>">カタログ注文</a>
```

#### HTML変換後
```html
<a href="/view/catalog"></a>
```

## $url.cart

### 概要
買い物カゴURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.cart}>">カートを見る</a>
```

#### HTML変換後
```html
<a href="/view/cart"></a>
```

## $url.favorite

### 概要
お気に入りURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.favorite}>">お気に入り</a>
```

#### HTML変換後
```html
<a href="/view/member/favorite"></a>
```

# 会員情報

## $member.is_logged_in

### 概要
ログインしているかどうか

### サンプルコード

#### クリエーターモード
```php
<ul>
    <{if $member.is_logged_in}>
        <li><a href="<{$url.logout}>">ログアウト</a></li>
    <{else}>
        <li><a href="<{$url.member_entry}>">新規会員登録</a></li>
        <li><a href="<{$url.login}>">ログイン</a></li>
    <{/if}>
</ul>
```

#### HTML変換後
```html
<ul>
    <li><a href="/shop/logout.html">ログアウト</a></li>
</ul>
```

## $member.name

### 概要
会員氏名

### サンプルコード

#### クリエーターモード
```php
<p><{$member.name}>様</p>
```

#### HTML変換後
```html
<p>●●●●様</p>
```

## $member.id

### 概要
会員ID

### サンプルコード

#### クリエーターモード
```php
<p>会員ID：<{$member.id}></p>
```

#### HTML変換後
```html
<p>会員ID：000000000000</p>
```

## $member.point

### 概要
所有ポイント

### サンプルコード

#### クリエーターモード
```php
<a href="<{$url.point}>">
    <span><{$member.point}> ポイント</span>
</a>
```

#### HTML変換後
```html
<a href="/view/member/point">
    <span>●●● ポイント</span>
</a>
```

## $member.group_name

### 概要
会員グループ名

### サンプルコード

#### クリエーターモード
```php
<p><{$member.group_name}>会員</p>
```

#### HTML変換後
```html
<p>●●●●会員</p>
```

## $member.group_id

### 概要
会員グループID

### サンプルコード

#### クリエーターモード
```php
<p>会員グループID：<{$member.group_id}></p>
```

#### HTML変換後
```html
<p>会員グループID：000</p>
```

# 商品一覧系

## $new_item

### 概要
新商品

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.has_item}>
    <section>
        <h2>新商品</h2>
        <ul>
            <{section name=i loop=$new_item.list max=10}>
                <li>
                    <a href="<{$new_item.list[i].url}>">
                        <{if $new_item.list[i].is_soldout}>
                            <p>Soldout</p>
                        <{/if}>
                        <img src="<{$new_item.list[i].image_M}>" alt="<{$new_item.list[i].name}>">
                        <p><{$new_item.list[i].name}></p>
                    </a>
                    <p>
                        <a href="<{$new_item.list[i].base_category.url}>">
                            <{$new_item.list[i].base_category.name}>
                        </a>
                    </p>
                    <{if $new_item.list[i].is_sale}>
                        <p><{$new_item.list[i].sale_rate}>%OFF</p>
                        <p>￥<{$new_item.list[i].price|number_format}>(税込)</p>
                    <{else}>
                        <p>￥<{$new_item.list[i].price|number_format}>(税込)</p>
                    <{/if}>
                </li>
            <{/section}>
        </ul>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>新商品</h2>
    <ul>
        <!--出力はMAX10個まで-->
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>￥8,000(税込)</p>
        </li>
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <p>Soldout</p>
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>￥8,000(税込)</p>
        </li>
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>10%OFF</p>
            <p>￥7,200(税込)</p>
        </li>
    </ul>
</section>
```

## $new_item.has_item

### 概要
新商品が登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.has_item}>
  <div>新商品が登録されています</div>
<{/if}>
```

#### HTML変換後
```html
<div>新商品が登録されています</div>
```

## $recommend_item

### 概要
おすすめ商品

### サンプルコード

#### クリエーターモード
```php
<{if $recommend_item.has_item}>
    <section>
        <h2>おすすめ商品</h2>
        <ul>
            <{section name=i loop=$recommend_item.list max=10}>
                <li>
                    <a href="<{$recommend_item.list[i].url}>">
                        <{if $recommend_item.list[i].is_soldout}>
                            <p>Soldout</p>
                        <{/if}>
                        <img src="<{$recommend_item.list[i].image_M}>" alt="<{$recommend_item.list[i].name}>">
                        <p><{$recommend_item.list[i].name}></p>
                    </a>
                    <p>
                        <a href="<{$recommend_item.list[i].base_category.url}>">
                            <{$recommend_item.list[i].base_category.name}>
                        </a>
                    </p>
                    <{if $recommend_item.list[i].is_sale}>
                        <p><{$recommend_item.list[i].sale_rate}>%OFF</p>
                        <p>￥<{$recommend_item.list[i].price|number_format}>(税込)</p>
                    <{else}>
                        <p>￥<{$recommend_item.list[i].price|number_format}>(税込)</p>
                    <{/if}>
                </li>
            <{/section}>
        </ul>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>おすすめ商品</h2>
    <ul>
        <!--出力はMAX10個まで-->
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>￥8,000(税込)</p>
        </li>
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <p>Soldout</p>
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>￥8,000(税込)</p>
        </li>
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>10%OFF</p>
            <p>￥7,200(税込)</p>
        </li>
    </ul>
</section>
```

## $recommend_item.has_item

### 概要
おすすめ商品が登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $recommend_item.has_item}>
  <div>おすすめ商品が登録されています</div>
<{/if}>
```

#### HTML変換後
```html
<div>おすすめ商品が登録されています</div>
```

## $special_item

### 概要
スペシャル商品

### サンプルコード

#### クリエーターモード
```php
<{if $special_item.has_item}>
    <section>
        <h2>スペシャル商品</h2>
        <ul>
            <{section name=i loop=$special_item.list max=10}>
                <li>
                    <a href="<{$special_item.list[i].url}>">
                        <{if $special_item.list[i].is_soldout}>
                            <p>Soldout</p>
                        <{/if}>
                        <img src="<{$special_item.list[i].image_M}>" alt="<{$special_item.list[i].name}>">
                        <p><{$special_item.list[i].name}></p>
                    </a>
                    <p>
                        <a href="<{$special_item.list[i].base_category.url}>">
                            <{$special_item.list[i].base_category.name}>
                        </a>
                    </p>
                    <{if $special_item.list[i].is_sale}>
                        <p><{$special_item.list[i].sale_rate}>%OFF</p>
                        <p>￥<{$special_item.list[i].price|number_format}>(税込)</p>
                    <{else}>
                        <p>￥<{$special_item.list[i].price|number_format}>(税込)</p>
                    <{/if}>
                </li>
            <{/section}>
        </ul>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>スペシャル商品</h2>
    <ul>
        <!--出力はMAX10個まで-->
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>￥8,000(税込)</p>
        </li>
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <p>Soldout</p>
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>￥8,000(税込)</p>
        </li>
        <li>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <p>商品名</p>
            </a>
            <p>
                <a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a>
            </p>
            <p>10%OFF</p>
            <p>￥7,200(税込)</p>
        </li>
    </ul>
</section>
```

## $special_item.has_item

### 概要
スペシャル商品が登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $special_item.has_item}>
  <div>スペシャル商品が登録されています</div>
<{/if}>
```

#### HTML変換後
```html
<div>スペシャル商品が登録されています</div>
```

## $ranking_item

### 概要
ランキング

### サンプルコード

#### クリエーターモード
```php
<{if $ranking_item.has_item}>
    <section>
        <h2>ランキング</h2>
        <ul>
        <{section name=i loop=$ranking_item.list max=8}>
            <li>
                <div>
                    <{if $ranking_item.list[i].is_soldout}>
                        <p>SOLD OUT</p>
                    <{elseif $ranking_item.list[i].is_sale}>
                        <p>SALE</p>
                    <{/if}>
                </div>
        
                <div>
                    <a href="<{$ranking_item.list[i].url}>">
                        <img src="<{$ranking_item.list[i].image_L}>" alt="商品画像">
                        <div class="<{$ranking_item.list[i].num}>">
                            <{$ranking_item.list[i].num}>
                        </div>
                    </a>
                </div>
                <{if $ranking_item.list[i].base_category.url}>
                    <p><a href="<{$ranking_item.list[i].base_category.url}>"><{$ranking_item.list[i].base_category.name}></a></p>
                <{/if}>
                    <p><a href="<{$ranking_item.list[i].url}>"><{$ranking_item.list[i].name}></a></p>
                    <{if $ranking_item.list[i].is_sale}>
                        <p>￥<{$ranking_item.list[i].original_price|number_format}><span>(税込)</span></p>
                        <p>￥<{$ranking_item.list[i].price|number_format}><span>(税込)</span>
                        <span>[<{$ranking_item.list[i].sale_rate}>%OFF</span>]</p>
                    <{else}>
                    <p>￥<{$ranking_item.list[i].price|number_format}><span>(税込)</span></p>
                <{/if}>
                <{if $ranking_item.list[i].has_review}>
                    <div>
                        <{$ranking_item.list[i].review.star_html}>
                        <p><{$ranking_item.list[i].review.average}></p>
                        <p>[<a href="<{$ranking_item.list[i].review.url}>"><{$ranking_item.list[i].review.total_count}>件</a>]</p>
                    </div>
                <{/if}>
                <div>
                    <{if $ranking_item.list[i].is_soldout}>
                        <div>売り切れ</div>
                    <{else}>
                        <a href="<{$ranking_item.list[i].cart_entry_url}>">カートに入れる</a>
                    <{/if}>
                </div>
            </li>
        <{/section}>
        </ul>
    </section>
    <{/if}>
```

#### HTML変換後
```html
<section>
    <h2>ランキング</h2>
    <ul>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <div class="1">1</div>
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div>
          <div>
            <div>評価1</div>
            <div>評価2</div>
            <div>評価3</div>
            <div>評価4</div>
            <div>評価5</div>
          </div>
          <p>5.0</p>
          <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        </div>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <div class="2">2</div>
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <div class="3">3</div>
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <div class="4">4</div>
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
                <div class="5">5</div>
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
    </ul>
  </section>
```

## $ranking_item.has_item

### 概要
ランキング商品が登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $ranking_item.has_item}>
  <div>ランキング商品が登録されています</div>
<{/if}>
```

#### HTML変換後
```html
<div>ランキング商品が登録されています</div>
```

## $recently_item

### 概要
最近チェックした商品

### サンプルコード

#### クリエーターモード
```php
<{if $recently_item.has_item}>
    <section>
        <h2>最近チェックしたアイテム</h2>
        <ul>
        <{section name=i loop=$recently_item.list max=6}>
            <li>
                <div>
                <{if $recently_item.list[i].is_soldout}>
                    <p>SOLD OUT</p>
                <{elseif $recently_item.list[i].is_sale}>
                    <p>SALE</p>
                <{/if}>
                </div>
    
                <div>
                    <a href="<{$recently_item.list[i].url}>"><img src="<{$recently_item.list[i].image_L}>" alt=""></a>
                </div>
                <{if $recently_item.list[i].base_category.url}>
                    <p><a href="<{$recently_item.list[i].base_category.url}>"><{$recently_item.list[i].base_category.name}></a></p>
                <{/if}>
                    <p><a href="<{$recently_item.list[i].url}>"><{$recently_item.list[i].name}></a></p>
                <{if $recently_item.list[i].is_sale}>
                    <p>￥<{$recently_item.list[i].original_price|number_format}><span>（税込）</span></p>
                    <p>￥<{$recently_item.list[i].price|number_format}><span>（税込）</span>
                    <span>[<{$recently_item.list[i].sale_rate}>%OFF</span>]</p>
                <{else}>
                    <p>￥<{$recently_item.list[i].price|number_format}><span>（税込）</span></p>
                <{/if}>
                <div>
                    <{if $recently_item.list[i].is_soldout}>
                        <div>売り切れ</div>
                    <{else}>
                        <a href="<{$recently_item.list[i].cart_entry_url}>">カートに入れる</a>
                    <{/if}>
                </div>
            </li>
        <{/section}>
        </ul>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>最近チェックしたアイテム</h2>
    <ul>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
      <li>
        <div>
            <a href="/view/item/商品詳細ページリンク">
                <img src="商品画像パス.jpg" alt="商品画像">
            </a>
        </div>
        <p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
        <p>￥8,000<span>(税込)</span></p>
        <div><a href="カートに入れる">カートに入れる</a></div>
      </li>
    </ul>
</section>
```

## $recently_item.has_item

### 概要
最近チェックした商品が登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $recently_item.has_item}>
  <div>最近チェックした商品があります</div>
<{/if}>
```

#### HTML変換後
```html
<div>最近チェックした商品があります</div>
```

## .list[i].num

### 概要
番号

### サンプルコード

#### クリエーターモード
```php
<div><{$ranking_item.list[i].num}></div>
```

#### HTML変換後
```html
<div>番号</div>
```

## .list[i].name

### 概要
商品名

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].name}></p>
```

#### HTML変換後
```html
<p>商品名</p>
```

## .list[i].price

### 概要
販売価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$new_item.list[i].price}></p>
```

#### HTML変換後
```html
<p>￥7,200</p>
```

## .list[i].price_excluded_tax

### 概要
税抜き価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$new_item.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き価格</p>
```

## .list[i].tax

### 概要
税

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].tax}></p>
```

#### HTML変換後
```html
<p>消費税額</p>
```

## .list[i].tax_rate

### 概要
消費税率

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].tax_rate}>%</p>
```

#### HTML変換後
```html
<p>10%</p>
```

## .list[i].is_reduced_tax_rate

### 概要
軽減税率対象商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].is_reduced_tax_rate}>
  <div>軽減税率対象商品です</div>
<{/if}>
```

#### HTML変換後
```html
<div>軽減税率対象商品です</div>
```

## .list[i].fixed_price

### 概要
定価

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$new_item.list[i].fixed_price}></p>
```

#### HTML変換後
```html
<p>￥定価</p>
```

## .list[i].original_price

### 概要
通常価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$new_item.list[i].original_price}></p>
```

#### HTML変換後
```html
<p>￥通常価格</p>
```

## .list[i].original_price_excluded_tax

### 概要
税抜き通常価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$new.item.list[i].original_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き通常価格</p>
```

## .list[i].original_tax

### 概要
通常価格の税

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].original_tax}></p>
```

#### HTML変換後
```html
<p>通常価格の税</p>
```

## .list[i].url

### 概要
商品URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$new_item.list[i].url}>"><{$new_item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
```

## .list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$new_item.list[i].image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="商品縮小画像パス.jpg"></div>
```

## .list[i].image_M

### 概要
商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$new_item.list[i].image_M}>"></div>
```

#### HTML変換後
```html
<div><img src="商品普通画像パス.jpg"></div>
```

## .list[i].image_L

### 概要
商品画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$new_item.list[i].image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="商品画像パス.jpg"></div>
```

## .list[i].is_stock_display

### 概要
在庫表示可かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].is_stock_display}>
    <{if $new_item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $new_item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$new_item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$new_item.list[i].stock_quantity}>個</span></p>
        <{/if}>
    <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## .list[i].is_stock_unlimited

### 概要
在庫無制限かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].is_stock_unlimited}>
        <p>〇在庫あり</p>
    <{else}>
        <{if $new_item.list[i].is_small_stock}>
            <p>△残りわずか<span>あと<{$new_item.list[i].stock_quantity}>個</span></p>
        <{else}>
            <p>〇在庫あり<span>あと<{$new_item.list[i].stock_quantity}>個</span></p>
        <{/if}>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり</p>
```

## .list[i].is_soldout

### 概要
売り切れかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $new_item.list[i].is_soldout}>
        <div>売り切れ</div>
    <{else}>
        <a href="<{$new_item.list[i].cart_entry_url}>">カートに入れる</a>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <div>売り切れ</div>
</div>
```

## .list[i].is_small_stock

### 概要
在庫が指定された数以下かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].is_small_stock}>
        <p>△残りわずか<span>あと<{$new_item.list[i].stock_quantity}>個</span></p>
    <{else}>
        <p>〇在庫あり<span>あと●●個</span></p>
<{/if}>
```

#### HTML変換後
```html
<p>〇在庫あり<span>あと●●個</span></p>
```

## .list[i].stock_quantity

### 概要
在庫数

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].stock_quantity}></p>
```

#### HTML変換後
```html
<p>在庫数</p>
```

## .list[i].is_sale

### 概要
セール商品かどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $new_item.list[i].is_sale}>
        <p><{$new_item.list[i].original_price}><span>（税込）</span></p>
        <p><{$new_item.list[i].price}><span>（税込）</span>
        <span>[<{$new_item.list[i].sale_rate}>%OFF</span>]</p>
    <{else}>
        <p><{$new_item.list[i].price}><span>（税込）</span></p>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <p>通常価格<span>（税込）</span></p>
    <p>販売価格<span>（税込）</span>
    <span>[割引率 %OFF</span>]</p>
</div>
```

## .list[i].sale_rate

### 概要
割引率

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].sale_rate}>%OFF</p>
```

#### HTML変換後
```html
<p>●●%OFF</p>
```

## .list[i].has_review

### 概要
旧レビューが投稿されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].has_review}>
    <div>
        <{$new_item.list[i].review.star_html}>
        <p><{$new_item.list[i].review.average}></p>
        <p>[<a href="<{$new_item.list[i].review.url}>"><{$new_item.list[i].review.total_count}>件</a>]</p>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    レビュー評価（星）
    <p>★★★★★</p>
    <p>[<a href="レビュー一覧URL">レビュー投稿数 件</a>]</p>
</div>
```

## .list[i].review.star_html

### 概要
旧レビュー評価（星）

### サンプルコード

#### クリエーターモード
```php
<div><{$new_item.list[i].review.star_html}></div>
```

#### HTML変換後
```html
<div>★★★★★</div>
```

## .list[i].review.average

### 概要
平均旧レビュー点数

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].review.average}></p>
```

#### HTML変換後
```html
<p>平均レビュー点数</p>
```

## .list[i].review.total_count

### 概要
旧レビュー投稿数

### サンプルコード

#### クリエーターモード
```php
<p>[<{$new_item.list[i].review.total_count}>件]</p>
```

#### HTML変換後
```html
<p>[●●件]</p>
```

## .list[i].review.url

### 概要
旧レビュー一覧URL

### サンプルコード

#### クリエーターモード
```php
<p>[<a href="<{$new_item.list[i].review.url}>"><{$new_item.list[i].review.total_count}>件</a>]</p>
```

#### HTML変換後
```html
<p>[<a href="/view/review/レビュー一覧URL">●●件</a>]</p>
```

## .list[i].original_code

### 概要
独自商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].original_code}></p>
```

#### HTML変換後
```html
<p>独自商品コード</p>
```

## .list[i].system_code

### 概要
システム商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## .list[i].point

### 概要
獲得ポイント

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## .list[i].is_member_price

### 概要
会員割引商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].is_member_price}>
  <div>会員割引商品です</div>
<{/if}>
```

#### HTML変換後
```html
<div>会員割引商品です</div>
```

## .list[i].base_category.name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].base_category.name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## .list[i].base_category.url

### 概要
カテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$new_item.list[i].base_category.url}>"><{$new_item.list[i].base_category.name}></a></p>
```

#### HTML変換後
```html
<p><a href="/view/category/商品カテゴリーページリンク">カテゴリー名</a></p>
```

## .list[i].base_category.code

### 概要
カテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].base_category.code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## .list[i].description

### 概要
商品説明文

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].description}></p>
```

#### HTML変換後
```html
<p>商品説明文</p>
```

## .list[i].manufacturer

### 概要
製造元

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].manufacturer}></p>
```

#### HTML変換後
```html
<p>製造元</p>
```

## .list[i].origin_country

### 概要
原産地

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].origin_country}></p>
```

#### HTML変換後
```html
<p>原産地</p>
```

## .list[i].special_display

### 概要
商品別特殊表示

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## .list[i].is_reservation_sale

### 概要
予約販売商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.is_reservation_sale}>
    <div>
        <{if $new_item.has_release_date}>
            <{if !$new_item.is_released}>
                <p>販売開始：<{$new_item.release_date.year}>年<{$new_item.release_date.month}>月<{$new_item.release_date.day}>日</p>
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

## .list[i].reservation_sale_note

### 概要
備考

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].reservation_sale_note}></p>
```

#### HTML変換後
```html
<p>備考</p>
```

## .list[i].has_release_date

### 概要
発売日が設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $new_item.has_release_date}>
        <{if !$new_item.is_released}>
            <p>販売開始：<{$new_item.release_date.year}>年<{$new_item.release_date.month}>月<{$new_item.release_date.day}>日</p>
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

## .list[i].release_date.year

### 概要
発売日時（年）

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].release_date.year}></p>
```

#### HTML変換後
```html
<p>発売日時（年）</p>
```

## .list[i].release_date.month

### 概要
発売日時（月）

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].release_date.month}></p>
```

#### HTML変換後
```html
<p>発売日時（月）</p>
```

## .list[i].release_date.day

### 概要
発売日時（日）

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].release_date.day}></p>
```

#### HTML変換後
```html
<p>発売日時（日）</p>
```

## .list[i].release_date_note

### 概要
発売日備考

### サンプルコード

#### クリエーターモード
```php
<p><{$new_item.list[i].release_date_note}></p>
```

#### HTML変換後
```html
<p>発売日備考</p>
```

## .list[i].has_option

### 概要
オプションが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].has_option}>
  <div>オプションが設定されています</div>
<{/if}>
```

#### HTML変換後
```html
<div>オプションが設定されています</div>
```

## .list[i].cart_entry_url

### 概要
かごに入れるURL

### サンプルコード

#### クリエーターモード
```php
<div><a href="<{$new_item.list[i].cart_entry_url}>">カートに入れる</a></div>
```

#### HTML変換後
```html
<div><a href="かごに入れるURL">カートに入れる</a></div>
```

## .list[i].icon.has_item

### 概要
アイコンが設定されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $new_item.list[i].icon.has_item}>
    <div>
        <ul>
            <{section name=j loop=$new_item.list[i].icon.list}>
                <li>
                    <img src="<{$new_item.list[i].icon.list[j].image_url}>">
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

## .list[i].icon.list[j].image_url

### 概要
アイコン画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$new_item.list[i].icon.list[j].image_url}>" ></div>
```

#### HTML変換後
```html
<div><img src="アイコン画像URL.jpg" ></div>
```

# 旧新着レビュー一覧

## $review_item.is_enabled

### 概要
旧レビュー機能が有効かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $review_item.is_enabled}>
    <{if $review_item.has_item}>
    <section>
        <h2>新着レビュー</h2>
        <ul>
            <{section name=i loop=$review_item.list}>
            <li>
                <a href="<{$review_item.list[i].url}>">
                    <img src="<{$review_item.list[i].image_S}>" alt="<{$review_item.list[i].name}>">
                </a>
                <p><a href="<{$review_item.list[i].base_category.url}>"><{$review_item.list[i].base_category.name}></a></p>
                <p><a href="<{$review_item.list[i].url}>"><{$review_item.list[i].name}></a></p>
                <p><{$review_item.list[i].reviewer_name}></p>
                <div><{$review_item.list[i].star_html}></div>
                <p><{$review_item.list[i].score}></p>
                <p><{$review_item.list[i].date.year}>/<{$review_item.list[i].date.month}>/<{$review_item.list[i].date.day}> <{$review_item.list[i].date.hour}>:<{$review_item.list[i].date.minute}></p>
                <div><{$review_item.list[i].content}></div>
            </li>
            <{/section}>
        </ul>
    </section>
    <{/if}>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>新着レビュー</h2>
    <ul>
        <li>
            <a href="商品URL">
                <img src="商品画像パス" alt="商品名">
            </a>
            <p><a href="商品カテゴリーURL">商品カテゴリー名</a></p>
            <p><a href="商品URL">商品名</a></p>
            <p>投稿者名</p>
            <div>レビュー評価（星）</div>
            <p>レビュー点数</p>
            <p>投稿日時（年）/投稿日時（月）/投稿日時（日） 投稿日時（時）:投稿日時（分）</p>
            <div>レビュー内容</div>
        </li>
    </ul>
</section>
```

## $review_item.has_item

### 概要
旧レビューが投稿されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $review_item.has_item}>
    <section>
        <h2>新着レビュー</h2>
        <ul>
            <{section name=i loop=$review_item.list}>
            <li>
                <a href="<{$review_item.list[i].url}>">
                    <img src="<{$review_item.list[i].image_S}>" alt="<{$review_item.list[i].name}>">
                </a>
                <p><a href="<{$review_item.list[i].base_category.url}>"><{$review_item.list[i].base_category.name}></a></p>
                <p><a href="<{$review_item.list[i].url}>"><{$review_item.list[i].name}></a></p>
                <p><{$review_item.list[i].reviewer_name}></p>
                <div><{$review_item.list[i].star_html}></div>
                <p><{$review_item.list[i].score}></p>
                <p><{$review_item.list[i].date.year}>/<{$review_item.list[i].date.month}>/<{$review_item.list[i].date.day}> <{$review_item.list[i].date.hour}>:<{$review_item.list[i].date.minute}></p>
                <div><{$review_item.list[i].content}></div>
            </li>
            <{/section}>
        </ul>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>新着レビュー</h2>
    <ul>
        <li>
            <a href="商品URL">
                <img src="商品画像パス" alt="商品名">
            </a>
            <p><a href="商品カテゴリーURL">商品カテゴリー名</a></p>
            <p><a href="商品URL">商品名</a></p>
            <p>投稿者名</p>
            <div>レビュー評価（星）</div>
            <p>レビュー点数</p>
            <p>投稿日時（年）/投稿日時（月）/投稿日時（日） 投稿日時（時）:投稿日時（分）</p>
            <div>レビュー内容</div>
        </li>
    </ul>
</section>
```

## $review_item.list[i].reviewer_name

### 概要
投稿者名

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].reviewer_name}></p>
```

#### HTML変換後
```html
<p>投稿者名</p>
```

## $review_item.list[i].star_html

### 概要
旧レビュー評価（星）

### サンプルコード

#### クリエーターモード
```php
<div><{$review_item.list[i].star_html}></div>
```

#### HTML変換後
```html
<div>レビュー評価（星）</div>
```

## $review_item.list[i].score

### 概要
旧レビュー点数

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].score}></p>
```

#### HTML変換後
```html
<p>レビュー点数</p>
```

## $review_item.list[i].content

### 概要
旧レビュー内容

### サンプルコード

#### クリエーターモード
```php
<div><{$review_item.list[i].content}></div>
```

#### HTML変換後
```html
<div>レビュー内容</div>
```

## $review_item.list[i].name

### 概要
商品名

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].name}></p>
```

#### HTML変換後
```html
<p>商品名</p>
```

## $review_item.list[i].url

### 概要
商品URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$review_item.list[i].url}>"><{$review_item.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品カテゴリーURL">商品カテゴリー名</a></p>
```

## $review_item.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<!--画像サイズSの場合-->
<img src="<{$review_item.list[i].image_S}>" alt="<{$review_item.list[i].name}>">
```

#### HTML変換後
```html
<!--画像サイズSの場合-->
<img src="商品画像パス" alt="商品名">
```

## $review_item.list[i].image_M

### 概要
商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<!--画像サイズMの場合-->
<img src="<{$review_item.list[i].image_M}>" alt="<{$review_item.list[i].name}>">
```

#### HTML変換後
```html
<!--画像サイズMの場合-->
<img src="商品画像パス" alt="商品名">
```

## $review_item.list[i].image_L

### 概要
商品画像URL

### サンプルコード

#### クリエーターモード
```php
<!--画像サイズLの場合-->
<img src="<{$review_item.list[i].image_L}>" alt="<{$review_item.list[i].name}>">
```

#### HTML変換後
```html
<!--画像サイズLの場合-->
<img src="商品画像パス" alt="商品名">
```

## $review_item.list[i].base_category.name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].base_category.name}></p>
```

#### HTML変換後
```html
<p>商品カテゴリー名</p>
```

## $review_item.list[i].base_category.url

### 概要
カテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$review_item.list[i].base_category.url}>"><{$review_item.list[i].base_category.name}></a></p>
```

#### HTML変換後
```html
<p><a href="商品カテゴリーURL">商品カテゴリー名</a></p>
```

## $review_item.list[i].date.year

### 概要
投稿日時（年）

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].date.year}></p>
```

#### HTML変換後
```html
<p>投稿日時（年）</p>
```

## $review_item.list[i].date.month

### 概要
投稿日時（月）

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].date.month}></p>
```

#### HTML変換後
```html
<p>投稿日時（月）</p>
```

## $review_item.list[i].date.day

### 概要
投稿日時（日）

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].date.day}></p>
```

#### HTML変換後
```html
<p>投稿日時（日）</p>
```

## $review_item.list[i].date.hour

### 概要
投稿日時（時）

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].date.hour}></p>
```

#### HTML変換後
```html
<p>投稿日時（時）</p>
```

## $review_item.list[i].date.minute

### 概要
投稿日時（分）

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].date.minute}></p>
```

#### HTML変換後
```html
<p>投稿日時（分）</p>
```

# お知らせ一覧

## $latest_news.has_item

### 概要
お知らせが登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $latest_news.has_item}>
    <section>
        <h2>ショップからのお知らせ</h2>
        <ul>
            <{section name=i loop=$latest_news.list max=5}>
            <li>
                <div class="news-wrap">
                    <p class="news-date"><{$latest_news.list[i].date.year}>/<{$latest_news.list[i].date.month}>/<{$latest_news.list[i].date.day}> <{$latest_news.list[i].date.hour}>:<{$latest_news.list[i].date.minute}></p>
                    <dl>
                        <dt class="news-title"><a href="<{$latest_news.list[i].url}>"><{$latest_news.list[i].title}></a></dt>
                        <dd class="news-content"><{$latest_news.list[i].content|cut_html:100}></dd>
                    </dl>
                </div>
            </li>
            <{/section}>
        </ul>
        <p class="news-more"><a href="<{$url.news}>">お知らせ一覧へ</a></p>
    </section>
<{/if}>
```

#### HTML変換後
```html
<section>
    <h2>ショップからのお知らせ</h2>
    <ul>
        <li>
            <div class="news-wrap">
                <p class="news-list-date">投稿日時（年）/投稿日時（月）/投稿日時（日） 投稿日時（時）:投稿日時（分）</p>
                <dl>
                    <dt class="news-title"><a href="お知らせURL">お知らせタイトル</a></dt>
                    <dd class="news-content">お知らせ内容</dd>
                </dl>
            </div>
        </li>
    </ul>
    <p class="news-more"><a href="お知らせ一覧URL">お知らせ一覧へ</a></p>
</section>
```

## $latest_news.list[i].title

### 概要
お知らせタイトル

### サンプルコード

#### クリエーターモード
```php
<p><{$latest_news.list[i].title}></p>
```

#### HTML変換後
```html
<p>お知らせタイトル</p>
```

## $latest_news.list[i].url

### 概要
お知らせ詳細URL。公式詳細ページが取得不可（HTTP 404）

### サンプルコード

#### クリエーターモード
```php
<a href="<{$latest_news.list[i].url}>">お知らせ詳細</a>
```

#### HTML変換後
```html
<a href="お知らせ詳細URL">お知らせ詳細</a>
```

## $latest_news.list[i].content

### 概要
お知らせ内容

### サンプルコード

#### クリエーターモード
```php
<p><{$latest_news.list[i].content}></p>
```

#### HTML変換後
```html
<p>お知らせ内容</p>
```

## $latest_news.list[i].date.year

### 概要
投稿日時（年）

### サンプルコード

#### クリエーターモード
```php
<p><{$review_item.list[i].date.year}></p>
```

#### HTML変換後
```html
<p>投稿日時（年）</p>
```

## $latest_news.list[i].date.month

### 概要
投稿日時（月）

### サンプルコード

#### クリエーターモード
```php
<p><{$news.list[i].date.month}></p>
```

#### HTML変換後
```html
<p>投稿日時（月）</p>
```

## $latest_news.list[i].date.day

### 概要
投稿日時（日）

### サンプルコード

#### クリエーターモード
```php
<p><{$news.list[i].date.day}></p>
```

#### HTML変換後
```html
<p>投稿日時（日）</p>
```

## $latest_news.list[i].date.hour

### 概要
投稿日時（時）

### サンプルコード

#### クリエーターモード
```php
<p><{$news.list[i].date.hour}></p>
```

#### HTML変換後
```html
<p>投稿日時（時）</p>
```

## $latest_news.list[i].date.minute

### 概要
投稿日時（分）

### サンプルコード

#### クリエーターモード
```php
<p><{$news.list[i].date.minute}></p>
```

#### HTML変換後
```html
<p>投稿日時（分）</p>
```

# カテゴリー一覧

## $category_menu.has_item

### 概要
カテゴリーが登録されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $category_menu.has_item}>
    <{section name=i loop=$category_menu.list}>
    <ul>
        <!--1階層目-->
        <li><a href="<{$category_menu.list[i].url}>"><{$category_menu.list[i].name}><{$category_menu.list[i].code}></a></li>
            <!--2階層目-->
            <{if $category_menu.list[i].child_category.has_item}>
            <ul>
                <{section name=j loop=$category_menu.list[i].child_category.list}>
                <li><a href="<{$category_menu.list[i].child_category.list[j].url}>"><{$category_menu.list[i].child_category.list[j].name}><{$category_menu.list[i].child_category.list[j].code}></a>
                    <!--3階層目-->
                    <{if $category_menu.list[i].child_category.list[j].child_category.has_item}>
                    <ul>
                        <{section name=k loop=$category_menu.list[i].child_category.list[j].child_category.list}>
                        <li><a href="<{$category_menu.list[i].child_category.list[j].child_category.list[k].url}>"><{$category_menu.list[i].child_category.list[j].child_category.list[k].name}><{$category_menu.list[i].child_category.list[j].child_category.list[k].code}></a>
                            <!--4階層目-->
                            <{if $category_menu.list[i].child_category.list[j].child_category.list[k].child_category.has_item}>
                            <ul>
                                <{section name=l loop=$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list}>
                                <li><a href="<{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].url}>"><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].name}><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].code}></a>
                                    <!--5階層目-->
                                    <{if $category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.has_item}>
                                    <ul>
                                        <{section name=m loop=$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list}>
                                        <li><a href="<{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].url}>"><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].name}><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].code}></a></li>
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
<{/if}>
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

## $category_menu.list[i].name

### 概要
カテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$category_menu.list[i].name}></p>
```

#### HTML変換後
```html
<p>カテゴリー名</p>
```

## $category_menu.list[i].url

### 概要
カテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$category_menu.list[i].url}>"><{$category_menu.list[i].name}></a>
```

#### HTML変換後
```html
<a href="カテゴリーURL">カテゴリー名</a>
```

## $category_menu.list[i].code

### 概要
カテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category_menu.list[i].code}></p>
```

#### HTML変換後
```html
<p>カテゴリー識別コード</p>
```

## $category_menu.list[i].child_category.has_item

### 概要
サブカテゴリーを持っているかどうか

### サンプルコード

#### クリエーターモード
```php
<{section name=i loop=$category_menu.list}>
<ul>
    <!--1階層目-->
    <li><a href="<{$category_menu.list[i].url}>"><{$category_menu.list[i].name}><{$category_menu.list[i].code}></a></li>
        <!--2階層目-->
        <{if $category_menu.list[i].child_category.has_item}>
        <ul>
            <{section name=j loop=$category_menu.list[i].child_category.list}>
            <li><a href="<{$category_menu.list[i].child_category.list[j].url}>"><{$category_menu.list[i].child_category.list[j].name}><{$category_menu.list[i].child_category.list[j].code}></a>
                <!--3階層目-->
                <{if $category_menu.list[i].child_category.list[j].child_category.has_item}>
                <ul>
                    <{section name=k loop=$category_menu.list[i].child_category.list[j].child_category.list}>
                    <li><a href="<{$category_menu.list[i].child_category.list[j].child_category.list[k].url}>"><{$category_menu.list[i].child_category.list[j].child_category.list[k].name}><{$category_menu.list[i].child_category.list[j].child_category.list[k].code}></a>
                        <!--4階層目-->
                        <{if $category_menu.list[i].child_category.list[j].child_category.list[k].child_category.has_item}>
                        <ul>
                            <{section name=l loop=$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list}>
                            <li><a href="<{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].url}>"><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].name}><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].code}></a>
                                <!--5階層目-->
                                <{if $category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.has_item}>
                                <ul>
                                    <{section name=m loop=$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list}>
                                    <li><a href="<{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].url}>"><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].name}><{$category_menu.list[i].child_category.list[j].child_category.list[k].child_category.list[l].child_category.list[m].code}></a></li>
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

## $category_menu.list[i].child_category.list[j].name

### 概要
サブカテゴリー名

### サンプルコード

#### クリエーターモード
```php
<p><{$category_menu.list[i].child_category.list[j].name}></p>
```

#### HTML変換後
```html
<p>サブカテゴリー名</p>
```

## $category_menu.list[i].child_category.list[j].url

### 概要
サブカテゴリーURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$category_menu.list[i].child_category.list[j].url}>"><{$category_menu.list[i].child_category.list[j].name}></a>
```

#### HTML変換後
```html
<a href="サブカテゴリーURL">サブカテゴリー名</a>
```

## $category_menu.list[i].child_category.list[j].code

### 概要
サブカテゴリー識別コード

### サンプルコード

#### クリエーターモード
```php
<p><{$category_menu.list[i].child_category.list[j].code}></p>
```

#### HTML変換後
```html
<p>サブカテゴリー識別コード</p>
```

# 商品検索

## $search_form.keyword_id

### 概要
キーワードフォーム用データID

### サンプルコード

#### クリエーターモード
```php
<label>キーワードで探す</label>
<input type="text" data-id="<{$search_form.keyword_id}>" value="<{$search.keyword}>">
```

#### HTML変換後
```html
<label>キーワードで探す</label>
<input type="text" data-id="makeshop-search-keyword" value="入力されたキーワード">
```

## $search_form.name_id

### 概要
商品名フォーム用データID

### サンプルコード

#### クリエーターモード
```php
<label>商品名で探す</label>
<input type="text" data-id="<{$search_form.name_id}>" value="<{$search.name}>">
```

#### HTML変換後
```html
<label>商品名で探す</label>
<input type="text" data-id="makeshop-search-name" value="入力された商品名">
```

## $search_form.category_id

### 概要
カテゴリー選択フォーム用データID

### サンプルコード

#### クリエーターモード
```php
<select data-id="<{$search_form.category_id}>">
    <{section name=i loop=$search_form.category_list}>
        <option value="<{$search_form.category_list[i].code}>" <{if $search.category.code == $search_form.category_list[i].code}>selected<{/if}>><{$search_form.category_list[i].name}></option>
    <{/section}>
</select>
```

#### HTML変換後
```html
<select data-id="makeshop-search-category">
    <option value="ct10">カテゴリー名</option>
</select>
```

## $search_form.category_list[i].name

### 概要
カテゴリ名

### サンプルコード

#### クリエーターモード
```php
<select data-id="<{$search_form.category_id}>">
    <{section name=i loop=$search_form.category_list}>
        <option value="<{$search_form.category_list[i].code}>" <{if $search.category.code == $search_form.category_list[i].code}>selected<{/if}>><{$search_form.category_list[i].name}></option>
    <{/section}>
</select>
```

#### HTML変換後
```html
<select data-id="makeshop-search-category">
    <option value="ct10">カテゴリー名</option>
</select>
```

## $search_form.category_list[i].code

### 概要
カテゴリ識別コード

### サンプルコード

#### クリエーターモード
```php
<select data-id="<{$search_form.category_id}>">
    <{section name=i loop=$search_form.category_list}>
        <option value="<{$search_form.category_list[i].code}>" <{if $search.category.code == $search_form.category_list[i].code}>selected<{/if}>><{$search_form.category_list[i].name}></option>
    <{/section}>
</select>
```

#### HTML変換後
```html
<select data-id="makeshop-search-category">
    <option value="ct10">カテゴリー名</option>
</select>
```

## $search_form.price_low_id

### 概要
価格帯（低）フォーム用データID

### サンプルコード

#### クリエーターモード
```php
<label>価格帯で絞り込む</label>
<input type="text" data-id="<{$search_form.price_low_id}>" value="<{$search.price_low}>">〜<input type="text" data-id="<{$search_form.price_high_id}>" value="<{$search.price_high}>">円
```

#### HTML変換後
```html
<label>価格帯で絞り込む</label>
<input type="text" data-id="makeshop-search-price-low" value="入力された金額">〜<input type="text" data-id="makeshop-search-price-high" value="入力された金額">円
```

## $search_form.price_high_id

### 概要
価格帯（高）フォーム用データID

### サンプルコード

#### クリエーターモード
```php
<label>価格帯で絞り込む</label>
<input type="text" data-id="<{$search_form.price_low_id}>" value="<{$search.price_low}>">〜<input type="text" data-id="<{$search_form.price_high_id}>" value="<{$search.price_high}>">円
```

#### HTML変換後
```html
<label>価格帯で絞り込む</label>
<input type="text" data-id="makeshop-search-price-low" value="入力された金額">〜<input type="text" data-id="makeshop-search-price-high" value="入力された金額">円
```

## $search_form.original_code_id

### 概要
独自商品コードフォーム用データID

### サンプルコード

#### クリエーターモード
```php
<label>独自商品コードで探す</label>
<input type="text" data-id="<{$search_form.original_code_id}>" value="<{$search.original_code}>" placeholder="独自商品コードを入力">
```

#### HTML変換後
```html
<label>独自商品コードで探す</label>
<input type="text" data-id="makeshop-search-original-code" value="入力された独自商品コード" placeholder="独自商品コードを入力">
```

## $search_form.search_url

### 概要
商品検索用URL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$search_form.search_url}>">検索する</a>
```

#### HTML変換後
```html
<a href="#makeshop-common-search-url">検索する</a>
```

# 買い物かご

## $cart.has_item

### 概要
買い物かごに商品があるかどうか

### サンプルコード

#### クリエーターモード
```php
<div>
    <{if $cart.has_item}>
        <ul>
            <li><a href="<{$cart.order_url}>">ご購入手続きへ進む</a></li>
            <li><a href="<{$url.top}>">買い物を続ける</a></li>
        </ul>
    <{else}>
        <p>カートに商品はありません</p>
    <{/if}>
</div>
```

#### HTML変換後
```html
<div>
    <ul>
        <li><a href="#makeshop-common-order-url">ご購入手続きへ進む</a></li>
        <li><a href="/">買い物を続ける</a></li>
    </ul>
</div>
```

## $cart.list[i].num

### 概要
かご内番号

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].num}></p>
```

#### HTML変換後
```html
<p>かご内番号</p>
```

## $cart.list[i].name

### 概要
商品名

### サンプルコード

#### クリエーターモード
```php
<p><{if $cart.list[i].name}></p>
```

#### HTML変換後
```html
<p>商品名</p>
```

## $cart.list[i].price

### 概要
商品単価

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$cart.list[i].price}></p>
```

#### HTML変換後
```html
<p>￥商品単価</p>
```

## $cart.list[i].price_excluded_tax

### 概要
税抜き商品単価

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$cart.list[i].price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き商品単価</p>
```

## $cart.list[i].total_price

### 概要
商品合計価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$cart.list[i].total_price}></p>
```

#### HTML変換後
```html
<p>￥商品合計価格</p>
```

## $cart.list[i].total_price_excluded_tax

### 概要
税抜き商品合計価格

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$cart.list[i].total_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>￥税抜き商品合計価格</p>
```

## $cart.list[i].tax_rate

### 概要
消費税率

### サンプルコード

#### クリエーターモード
```php
<p>￥<{$cart.list[i].tax_rate}>%</p>
```

#### HTML変換後
```html
<p>10%</p>
```

## $cart.list[i].is_reduced_tax_rate

### 概要
軽減税率対象商品かどうか。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```

## $cart.list[i].tax

### 概要
税単価

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].tax}></p>
```

#### HTML変換後
```html
<p>税単価</p>
```

## $cart.list[i].total_tax

### 概要
税合計

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].total_tax}></p>
```

#### HTML変換後
```html
<p>税合計</p>
```

## $cart.list[i].total_point

### 概要
獲得ポイント

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].total_point}></p>
```

#### HTML変換後
```html
<p>獲得ポイント</p>
```

## $cart.list[i].url

### 概要
商品URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$cart.list[i].url}>"><{$cart.list[i].name}></a></p>
```

#### HTML変換後
```html
<p><a href="/view/item/商品詳細ページリンク">商品名</a></p>
```

## $cart.list[i].image_S

### 概要
商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.list[i].image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="商品縮小画像パス.jpg"></div>
```

## $cart.list[i].image_M

### 概要
商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.list[i].image_M}>"></div>
```

#### HTML変換後
```html
<div><img src="商品普通画像パス.jpg"></div>
```

## $cart.list[i].image_L

### 概要
商品画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.list[i].image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="商品縮画像パス.jpg"></div>
```

## $cart.list[i].special_display

### 概要
商品特殊表示

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].special_display}></p>
```

#### HTML変換後
```html
<p>商品別特殊表示</p>
```

## $cart.list[i].quantity

### 概要
数量

### サンプルコード

#### クリエーターモード
```php
<div>
    <input type="text" data-id="<{$cart.list[i].quantity_id}>" value="<{$cart.list[i].quantity}>" name="item-quantity"><a href="<{$cart.list[i].quantity_url}>">更新</a>
    <span><a href="<{$cart.list[i].remove_url}>">削除</a></span>
</div>
```

#### HTML変換後
```html
<div>
    <input type="text" data-id="数量入力フォーム用データID" value="数量" name="item-quantity"><a> href="数量変更URL">更新</a>
    <spana href="商品削除URL">削除</a></span>
</div>
```

## $cart.list[i].quantity_id

### 概要
数量入力フォーム用データID

### サンプルコード

#### クリエーターモード
```php
<div>
    <input type="text" data-id="<{$cart.list[i].quantity_id}>" value="<{$cart.list[i].quantity}>" name="item-quantity"><a href="<{$cart.list[i].quantity_url}>">更新</a>
    <span><a href="<{$cart.list[i].remove_url}>">削除</a></span>
</div>
```

#### HTML変換後
```html
<div>
    <input type="text" data-id="数量入力フォーム用データID" value="数量" name="item-quantity"><a> href="数量変更URL">更新</a>
    <spana href="商品削除URL">削除</a></span>
</div>
```

## $cart.list[i].quantity_url

### 概要
数量変更URL

### サンプルコード

#### クリエーターモード
```php
<div>
    <input type="text" data-id="<{$cart.list[i].quantity_id}>" value="<{$cart.list[i].quantity}>" name="item-quantity"><a href="<{$cart.list[i].quantity_url}>">更新</a>
    <span><a href="<{$cart.list[i].remove_url}>">削除</a></span>
</div>
```

#### HTML変換後
```html
<div>
    <input type="text" data-id="数量入力フォーム用データID" value="数量" name="item-quantity"><a> href="数量変更URL">更新</a>
    <spana href="商品削除URL">削除</a></span>
</div>
```

## $cart.list[i].remove_url

### 概要
商品削除URL

### サンプルコード

#### クリエーターモード
```php
<div>
    <input type="text" data-id="<{$cart.list[i].remove_url}>" value="<{$cart.list[i].quantity}>" name="item-quantity"><a href="<{$cart.list[i].quantity_url}>">更新</a>
    <span><a href="<{$cart.list[i].remove_url}>">削除</a></span>
</div>
```

#### HTML変換後
```html
<div>
    <input type="text" data-id="数量入力フォーム用データID" value="数量" name="item-quantity"><a> href="数量変更URL">更新</a>
    <spana href="商品削除URL">削除</a></span>
</div>
```

## $cart.list[i].is_subscription

### 概要
定期購入商品かどうか（真偽値）

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].is_subscription}>
    <p>定期購入商品です</p>
<{/if}>
```

#### HTML変換後
```html
<p>定期購入商品です</p>
```

## $cart.list[i].subscription_discount.list[k].times

### 概要
回数

### サンプルコード

#### クリエーターモード
```php
<td><{$cart.list[i].subscription_discount.list[k].times}>回</td>
```

#### HTML変換後
```html
<td>●●●●●回</td>
```

## $cart.list[i].subscription_discount.list[k].price

### 概要
価格

### サンプルコード

#### クリエーターモード
```php
<td>￥<{$cart.list[i].subscription_discount.list[k].price}></td>
```

#### HTML変換後
```html
<td>￥●●●●●</td>
```

## $cart.list[i].subscription_discount.list[k].price_excluded_tax

### 概要
税抜き価格

### サンプルコード

#### クリエーターモード
```php
<td>￥<{$cart.list[i].subscription_discount.list[k].price_excluded_tax}></td>
```

#### HTML変換後
```html
<td>￥●●●●●</td>
```

## $cart.list[i].subscription_discount.list[k].quantity

### 概要
数量

### サンプルコード

#### クリエーターモード
```php
<td><{$cart.list[i].subscription_discount.list[k].quantity}>個</td>
```

#### HTML変換後
```html
<td>●●●●●個</td>
```

## $cart.list[i].subscription_discount.initial_quantity

### 概要
初回配送数（カート投入数 × 初回数）。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<td><{$cart.list[i].subscription_discount.initial_quantity}>個</td>
```

#### HTML変換後
```html
<td>●●●●●個</td>
```

## $cart.list[i].selected_option.has_item

### 概要
オプションが選択されているかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].selected_option.has_item}>
    <div>
        <{section name=j loop=$cart.list[i].selected_option.list}>
            <p><{$cart.list[i].selected_option.list[j].title}>：<{$cart.list[i].selected_option.list[j].option_name}></p>
        <{/section}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <p>オプション名：オプション項目名</p>
</div>
```

## $cart.list[i].selected_option.image_S

### 概要
オプション縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.list[i].selected_option.image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="オプション縮小画像パス.jpg"></div>
```

## $cart.list[i].selected_option.image_L

### 概要
オプション画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.list[i].selected_option.image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="オプション画像パス.jpg"></div>
```

## $cart.list[i].system_code

### 概要
システム商品コード

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].system_code}></p>
```

#### HTML変換後
```html
<p>システム商品コード</p>
```

## $cart.list[i].is_bulk

### 概要
まとめ買い割引商品かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].is_bulk}>
    <p><a href="<{$cart.list[i].bulk_url}>"><{$cart.list[i].bulk_name}></a></p>
<{/if}>
```

#### HTML変換後
```html
<p><a href="/view/bulk/まとめ買い割引ページURL">まとめ買い割引の名前</a></p>
```

## $cart.list[i].bulk_name

### 概要
まとめ買い割引の名前

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$cart.list[i].bulk_url}>"><{$cart.list[i].bulk_name}></a></p>
```

#### HTML変換後
```html
<p><a href="/view/bulk/まとめ買い割引ページURL">まとめ買い割引の名前</a></p>
```

## $cart.list[i].bulk_url

### 概要
まとめ買い割引ページのURL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$cart.list[i].bulk_url}>"><{$cart.list[i].bulk_name}></a></p>
```

#### HTML変換後
```html
<p><a href="/view/bulk/まとめ買い割引ページURL">まとめ買い割引の名前</a></p>
```

## $cart.list[i].name_print.has_item

### 概要
名入れ項目があるかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].name_print.has_item}>
    <div>
        <{section name=j loop=$cart.list[i].name_print.list}>
        <p><{$cart.list[i].name_print.list[j].title}></p>
        <p><{$cart.list[i].name_print.list[j].name|escape|nl2br}></p>
        <{/section}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <p>名入れタイトル</p>
    <p>名入れ入力値</p>
</div>
```

## $cart.list[i].name_print.list

### 概要
名入れ項目の配列

### サンプルコード

#### クリエーターモード
```php
<div>
    <{section name=j loop=$cart.list[i].name_print.list}>
        <p><{$cart.list[i].name_print.list[j].title}></p>
        <p><{$cart.list[i].name_print.list[j].name|escape|nl2br}></p>
    <{/section}>
</div>
```

#### HTML変換後
```html
<div>
    <p>名入れタイトル</p>
    <p>名入れ入力値</p>
</div>
```

## $cart.list[i].name_print.list[j].title

### 概要
名入れタイトル

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].name_print.list[j].title}></p>
```

#### HTML変換後
```html
<p>名入れタイトル</p>
```

## $cart.list[i].name_print.list[j].name

### 概要
名入れ入力値

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].name_print.list[j].name}></p>
```

#### HTML変換後
```html
<p>名入れ入力値</p>
```

## $cart.list[i].selected_option.list[j].title

### 概要
オプション名

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].selected_option.list[j].title}></p>
```

#### HTML変換後
```html
<p>オプション名</p>
```

## $cart.list[i].selected_option.list[j].option_name

### 概要
オプション項目名

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.list[i].selected_option.list[j].option_name}></p>
```

#### HTML変換後
```html
<p>オプション項目名</p>
```

## $cart.list[i].custom_select_summary

### 概要
カスタム選択項目

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].custom_select_summary}>
    <p><{$cart.list[i].custom_select_summary|escape:html|nl2br}></p>
<{/if}>
```

#### HTML変換後
```html
<p>カスタム選択項目</p>
```

## $cart.list[i].custom_select_price

### 概要
カスタム選択項目の価格

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].custom_select_price}>
    <p><{$cart.list[i].custom_select_price|number_format}>円</p>
<{/if}>
```

#### HTML変換後
```html
<p>〇〇〇〇円</p>
```

## $cart.list[i].custom_select_price_excluded_tax

### 概要
カスタム選択項目の価格（税抜）

### サンプルコード

#### クリエーターモード
```php
<{if $cart.list[i].custom_select_price_excluded_tax}>
    <p><{$cart.list[i].custom_select_price_excluded_tax|number_format}>円</p>
<{/if}>
```

#### HTML変換後
```html
<p>〇〇〇〇円</p>
```

## $cart.total_quantity

### 概要
商品の合計数

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.total_quantity}></p>
```

#### HTML変換後
```html
<p>商品の合計数</p>
```

## $cart.total_price

### 概要
合計金額

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.total_price}></p>
```

#### HTML変換後
```html
<p>合計金額</p>
```

## $cart.total_price_excluded_tax

### 概要
税抜き合計金額

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.total_price_excluded_tax}></p>
```

#### HTML変換後
```html
<p>税抜き合計金額</p>
```

## $cart.total_tax

### 概要
税合計

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.total_tax}></p>
```

#### HTML変換後
```html
<p>税合計</p>
```

## $cart.total_point

### 概要
合計獲得ポイント

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.total_point}></p>
```

#### HTML変換後
```html
<p>合計獲得ポイント</p>
```

## $cart.order_url

### 概要
決済画面URL

### サンプルコード

#### クリエーターモード
```php
<div>
    <a href="<{$cart.order_url}>">ご購入手続きへ進む</a>
</div>
```

#### HTML変換後
```html
<div>
    <a href="#makeshop-common-order-url">ご購入手続きへ進む</a>
</div>
```

## $cart.is_free_shipping_enabled

### 概要
「あと○円で送料無料」設定が有効かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $cart.is_free_shipping_enabled}>
    <div>
        <{if $cart.free_shipping_price == 0}>
            <p>今回のお買い物は送料無料となります</p>
        <{else}>
            <p>あと￥<{$cart.free_shipping_price|number_format}>で送料無料になります</p>
            <p><{$cart.free_shipping_message}></p>
        <{/if}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<p>今回のお買い物は送料無料となります</p>
```

## $cart.free_shipping_price

### 概要
「あと○円」の金額

### サンプルコード

#### クリエーターモード
```php
<p>あと￥<{$cart.free_shipping_price|number_format}>で送料無料になります</p>
```

#### HTML変換後
```html
<p>あと￥●●で送料無料になります</p>
```

## $cart.free_shipping_message

### 概要
「あと○円で送料無料」設定の案内文

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.free_shipping_message}></p>
```

#### HTML変換後
```html
<p>「あと●●円で送料無料」設定の案内文</p>
```

## $cart.is_estimate_enabled

### 概要
見積書発行機能が有効かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $cart.is_estimate_enabled}>
    <div>
        <a href="<{$cart.estimate_url}>">見積書を作成する</a>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <a href="<{$cart.estimate_url}>">見積書を作成する</a>
</div>
```

## $cart.estimate_url

### 概要
見積書発行URL

### サンプルコード

#### クリエーターモード
```php
<{if $cart.is_estimate_enabled}>
    <div>
        <a href="<{$cart.estimate_url}>">見積書を作成する</a>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    <a href="<{$cart.estimate_url}>">見積書を作成する</a>
</div>
```

## $cart.bulk.has_item

### 概要
まとめ買い割引の割引対象があるかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $cart.bulk.has_item}>
    <{section name=i loop=$cart.bulk.list}>
        <p><{$cart.bulk.list[i].name}> 割引額：￥<{$cart.bulk.list[i].discount_price}></p>
    <{/section}>
<{/if}>
```

#### HTML変換後
```html
<p>まとめ買い割引の名前 割引額：￥まとめ買い割引の割引対象の割引額</p>
```

## $cart.bulk.list[i].name

### 概要
まとめ買い割引の名前

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.bulk.list[i].name}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の名前</p>
```

## $cart.bulk.list[i].total_price

### 概要
まとめ買い割引の割引対象の小計

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.bulk.list[i].total_price}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の割引対象の小計</p>
```

## $cart.bulk.list[i].discount_price

### 概要
まとめ買い割引の割引対象の割引額

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.bulk.list[i].discount_price}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の割引対象の割引額</p>
```

## $cart.bulk.list[i].item.has_item

### 概要
まとめ買い割引の割引対象の商品があるかどうか（真偽値）。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```

## $cart.bulk.list[i].item.list[j].name

### 概要
まとめ買い割引の割引対象の商品名

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.bulk.list[i].item.list[j].name}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の割引対象の商品名</p>
```

## $cart.bulk.list[i].item.list[j].special_display

### 概要
まとめ買い割引の割引対象の商品別特殊表示

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.bulk.list[i].item.list[j].special_display}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の割引対象の商品別特殊表示</p>
```

## $cart.bulk.list[i].item.list[j].url

### 概要
まとめ買い割引の割引対象の商品URL

### サンプルコード

#### クリエーターモード
```php
<p><a href="<{$cart.bulk.list[i].item.list[j].url}>"><{$cart.bulk.list[i].item.list[j].name}></a></p>
```

#### HTML変換後
```html
<p><a href="まとめ買い割引の割引対象の商品URL">まとめ買い割引の割引対象の商品名</a></p>
```

## $cart.bulk.list[i].item.list[j].image_S

### 概要
まとめ買い割引の割引対象の商品縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.bulk.list[i].item.list[j].image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="まとめ買い割引の割引対象の商品縮小画像パス.jpg"></div>
```

## $cart.bulk.list[i].item.list[j].image_M

### 概要
まとめ買い割引の割引対象の商品普通画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.bulk.list[i].item.list[j].image_m}>"></div>
```

#### HTML変換後
```html
<div><img src="まとめ買い割引の割引対象の商品普通画像パス.jpg"></div>
```

## $cart.bulk.list[i].item.list[j].image_L

### 概要
まとめ買い割引の割引対象の商品画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.bulk.list[i].item.list[j].image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="まとめ買い割引の割引対象の商品画像パス.jpg"></div>
```

## $cart.bulk.list[i].item.list[j].quantity

### 概要
まとめ買い割引の割引対象の商品数量

### サンプルコード

#### クリエーターモード
```php
<p><{$cart.bulk.list[i].item.list[j].quantity}></p>
```

#### HTML変換後
```html
<p>まとめ買い割引の割引対象の商品数量</p>
```

## $cart.bulk.list[i].item.list[j].selected_option

### 概要
まとめ買い割引の割引対象の商品のオプション情報（$cart.list[i].selected_optionと同じデータ）。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```

## $cart.bulk.list[i].item.list[j].selected_option.image_S

### 概要
まとめ買い割引の割引対象のオプション縮小画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.bulk.list[i].item.list[j].selected_option.image_S}>"></div>
```

#### HTML変換後
```html
<div><img src="まとめ買い割引の割引対象のオプション縮小画像パス.jpg"></div>
```

## $cart.bulk.list[i].item.list[j].selected_option.image_L

### 概要
まとめ買い割引の割引対象のオプション画像URL

### サンプルコード

#### クリエーターモード
```php
<div><img src="<{$cart.bulk.list[i].item.list[j].selected_option.image_L}>"></div>
```

#### HTML変換後
```html
<div><img src="まとめ買い割引の割引対象のオプション画像パス.jpg"></div>
```

# Amzon Payボタン

## $amazonpay.is_enabled

### 概要
Amazon Pay利用中かどうか

### サンプルコード

#### クリエーターモード
```php
<{if $amazonpay.is_enabled}>
    <div>
       <{$amazonpay.button_html}>
    </div>
<{/if}>
```

#### HTML変換後
```html
<div>
    Amazon アカウントでお支払い
</div>
```

## $amazonpay.button_html

### 概要
Amazon Payボタン

### サンプルコード

#### クリエーターモード
```php
<div><{$amazonpay.button_html}></div>
```

#### HTML変換後
```html
<div>Amazon アカウントでお支払い</div>
```

# カレンダー

## $calendar1.year

### 概要
今月の年

### サンプルコード

#### クリエーターモード
```php
<p><{$calendar1.year}>年</p>
```

#### HTML変換後
```html
<p>今月の年</p>
```

## $calendar1.month

### 概要
今月の月

### サンプルコード

#### クリエーターモード
```php
<p><{$calendar1.month}>月</p>
```

#### HTML変換後
```html
<p>今月の月</p>
```

## $calendar1.html

### 概要
今月のカレンダーテーブル

### サンプルコード

#### クリエーターモード
```php
<div><{$calendar1.html}></div>
```

#### HTML変換後
```html
<div>
    <table class="makeshop-calendar1">
        <thead>
            <tr>
                <th class="sunday">日</th>
                <th class="monday">月</th>
                <th class="tuesday">火</th>
                <th class="wednesday">水</th>
                <th class="thursday">木</th>
                <th class="friday">金</th>
                <th class="saturday">土</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td></td>
                <td class="monday day1">1</td>
                <td class="tuesday day2">2</td>
                <td class="wednesday day3">3</td>
                <td class="thursday day4">4</td>
                <td class="friday day5">5</td>
                <td class="saturday day6">6</td>
            </tr>
            <tr>
                <td class="sunday day7">7</td>
                <td class="monday day8">8</td>
                <td class="tuesday day9">9</td>
                <td class="wednesday day10">10</td>
                <td class="thursday day11 today">11</td>
                <td class="friday day12">12</td>
                <td class="saturday day13">13</td>
            </tr>
            <tr>
                <td class="sunday day14">14</td>
                <td class="monday day15">15</td>
                <td class="tuesday day16">16</td>
                <td class="wednesday day17">17</td>
                <td class="thursday day18">18</td>
                <td class="friday day19">19</td>
                <td class="saturday day20">20</td>
            </tr>
            <tr>
                <td class="sunday day21">21</td>
                <td class="monday day22">22</td>
                <td class="tuesday day23">23</td>
                <td class="wednesday day24">24</td>
                <td class="thursday day25">25</td>
                <td class="friday day26">26</td>
                <td class="saturday day27">27</td>
            </tr>
            <tr>
                <td class="sunday day28">28</td>
                <td class="monday day29">29</td>
                <td class="tuesday day30">30</td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
        </tbody>
    </table>
</div>
```

## $calendar1.date_list[i].color

### 概要
特定日の背景カラー設定値

### サンプルコード

#### クリエーターモード
```php
<div><span style="color:<{$calendar1.date_list[i].color}>;">■</span></div>
```

#### HTML変換後
```html
<div><span style="指定の色">■</span></div>
```

## $calendar1.date_list[i].day_list

### 概要
特定日一覧。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```

## $calendar1.date_list[i].description

### 概要
特定日の説明文

### サンプルコード

#### クリエーターモード
```php
<div><{$calendar1.date_list[i].description}></div>
```

#### HTML変換後
```html
<div>特定日の説明文</div>
```

## $calendar2.year

### 概要
来月の年

### サンプルコード

#### クリエーターモード
```php
<p><{$calendar2.year}>年</p>
```

#### HTML変換後
```html
<p>来月の年</p>
```

## $calendar2.month

### 概要
来月の月

### サンプルコード

#### クリエーターモード
```php
<p><{$calendar2.month}>月</p>
```

#### HTML変換後
```html
<p>来月の月</p>
```

## $calendar2.html

### 概要
来月のカレンダーテーブル

### サンプルコード

#### クリエーターモード
```php
<div><{$calendar2.html}></div>
```

#### HTML変換後
```html
<div>
    <table class="makeshop-calendar2">
        <thead>
            <tr>
                <th class="sunday">日</th>
                <th class="monday">月</th>
                <th class="tuesday">火</th>
                <th class="wednesday">水</th>
                <th class="thursday">木</th>
                <th class="friday">金</th>
                <th class="saturday">土</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td></td>
                <td></td>
                <td></td>
                <td class="wednesday day1">1</td>
                <td class="thursday day2">2</td>
                <td class="friday day3">3</td>
                <td class="saturday day4">4</td>
            </tr>
            <tr>
                <td class="sunday day5">5</td>
                <td class="monday day6">6</td>
                <td class="tuesday day7">7</td>
                <td class="wednesday day8">8</td>
                <td class="thursday day9">9</td>
                <td class="friday day10">10</td>
                <td class="saturday day11">11</td>
            </tr>
            <tr>
                <td class="sunday day12">12</td>
                <td class="monday day13">13</td>
                <td class="tuesday day14">14</td>
                <td class="wednesday day15">15</td>
                <td class="thursday day16">16</td>
                <td class="friday day17">17</td>
                <td class="saturday day18">18</td>
            </tr>
            <tr>
                <td class="sunday day19">19</td>
                <td class="monday day20">20</td>
                <td class="tuesday day21">21</td>
                <td class="wednesday day22">22</td>
                <td class="thursday day23">23</td>
                <td class="friday day24">24</td>
                <td class="saturday day25">25</td>
            </tr>
            <tr>
                <td class="sunday day26">26</td>
                <td class="monday day27">27</td>
                <td class="tuesday day28">28</td>
                <td class="wednesday day29">29</td>
                <td class="thursday day30">30</td>
                <td class="friday day31">31</td>
                <td></td>
            </tr>
        </tbody>
    </table>
</div>
```

## $calendar2.date_list[i].color

### 概要
特定日の背景カラー設定値

### サンプルコード

#### クリエーターモード
```php
<div><span style="color:<{$calendar2.date_list[i].color}>;">■</span></div>
```

#### HTML変換後
```html
<div><span style="指定の色">■</span></div>
```

## $calendar2.date_list[i].day_list

### 概要
特定日一覧。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```

## $calendar2.date_list[i].description

### 概要
特定日の説明文

### サンプルコード

#### クリエーターモード
```php
<div><{$calendar2.date_list[i].description}></div>
```

#### HTML変換後
```html
<div>特定日の説明文</div>
```

# まとめ買い割引一覧

## $bulk_menu.has_item

### 概要
まとめ買い割引ページがあるかどうか

### サンプルコード

#### クリエーターモード
```php
<{if $bulk_menu.has_item}>
    <{section name=i loop=$bulk_menu.list}>
        <a href="<{$bulk_menu.list[i].url}>"><{$bulk_menu.list[i].name}></a>
    <{/section}>
<{/if}>
```

#### HTML変換後
```html
<a href="/view/bulk/まとめ買い割引ページURL">よりどり割引（定額割引）</a>
```

## $bulk_menu.list[i].name

### 概要
まとめ買い割引名

### サンプルコード

#### クリエーターモード
```php
<p><{$bulk_menu.list[i].name}></p>
```

#### HTML変換後
```html
<p>よりどり割引（定額割引）</p>
```

## $bulk_menu.list[i].url

### 概要
まとめ買い割引ページURL

### サンプルコード

#### クリエーターモード
```php
<a href="<{$bulk_menu.list[i].url}>"><{$bulk_menu.list[i].name}></a>
```

#### HTML変換後
```html
<a href="/view/bulk/まとめ買い割引ページURL">よりどり割引（定額割引）</a>
```

# ContentType設定

## <{insert name="content_type" type="css"}>

### 概要
css

### サンプルコード

#### クリエーターモード
```php
<{insert name="content_type" type="css"}>
```

#### HTML変換後
```html
<link rel="stylesheet" href="/view/page/任意の名前">
```

## <{insert name="content_type" type="javascript"}>

### 概要
javascript

### サンプルコード

#### クリエーターモード
```php
<{insert name="content_type" type="javascript"}>
```

#### HTML変換後
```html
<script src="/view/page/任意の名前"></script>
```

## <{insert name="content_type" type="xml"}>

### 概要
xml。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```

## <{insert name="content_type" type="json"}>

### 概要
json。公式一覧に詳細ページリンクなし

### サンプルコード

#### クリエーターモード
```php
<!-- 公式詳細ページにサンプルコードの掲載なし -->
```

#### HTML変換後
```html
<!-- 公式詳細ページにHTML出力イメージの掲載なし -->
```
