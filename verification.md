# 会員制／年齢確認

公式リファレンス: https://reference.makeshop.jp/creator-mode/contents/verification/index.html

⚠️ 推測サンプル: 公式リファレンス上でサンプルコードが確認できないタグは、タグ名と概要から使用例を推測して補完しています。

# 会員制

## $member_only.is_enabled

### 概要
会員制が有効かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$member_only.is_enabled}></p>
```

#### HTML変換後
```html
<!-- $member_only.is_enabled: true / false -->
```

# 年齢確認

## $age_verification.is_enabled

### 概要
年齢確認が有効かどうか（真偽値）

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$age_verification.is_enabled}></p>
```

#### HTML変換後
```html
<!-- $age_verification.is_enabled: true / false -->
```

## $age_verification.age

### 概要
確認対象の年齢

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$age_verification.age}></p>
```

#### HTML変換後
```html
<p>確認対象の年齢</p>
```

## $age_verification.url

### 概要
年齢確認URL

### サンプルコード（⚠️ 推測）

#### クリエーターモード
```php
<p><{$age_verification.url}></p>
```

#### HTML変換後
```html
<p>年齢確認URL</p>
```
