# WooCommerce-Mr-Tailor-Chinese-Translation
[WooCommerce](http://www.woothemes.com/woocommerce/) [Mr. Tailor Theme](http://themeforest.net/item/mr-tailor-responsive-woocommerce-theme/7292110?ref=arthurkao) Traditional Chinese (Taiwan) Translation

## [WooCommerce](http://www.woothemes.com/woocommerce/) [Mr. Tailor 佈景主題](http://themeforest.net/item/mr-tailor-responsive-woocommerce-theme/7292110?ref=arthurkao) 繁體中文翻譯檔
[Mr. Tailor](http://themeforest.net/item/mr-tailor-responsive-woocommerce-theme/7292110?ref=arthurkao) 是由 [getbowtied](http://themeforest.net/user/getbowtied?ref=arthurkao) 所製作發佈的 WooCommerce 收費佈景主題.
中文化翻譯檔由 [Arthur C. Kao](http://github.com/arthurkao) 編譯, 免費發佈.

## 系統要求
* [WooCommerce](http://www.woothemes.com/woocommerce/) 版本 2.3.11 或以上, 安裝於相容之 WordPress 系統上.
* Mr. Tailor Theme 版本 1.5 或以上
* 啟用 Mr. Tailor Child Theme. 如果不知道什麼是Child Theme(子佈景主題), 請參考[本教學](http://codex.wordpress.org/Child_Themes).

## 安裝
* 下載並解壓縮檔案
* 用[Poedit](http://poedit.net)開啟`zh_TW.po`, 再直接儲存檔案. [Poedit](http://poedit.net) 會自動在同一個資料夾生成`zh_TW.mo`.
* 把 `zh_TW.po` 及 `zh_TW.mo` 上傳到 `wp-content/themes/mrtailor-child/` 目錄.
* 複製下方的程式碼貼在`wp-content/themes/mrtailor-child/functions.php`
```php
/**
 * load mr tailor child theme translation file (zh_TW.mo)
 */
add_action( 'after_setup_theme', 'my_child_theme_setup' );
function my_child_theme_setup() {
    load_child_theme_textdomain( 'mr_tailor' );
}
```
* 搞定

## 更新
使用 [Poedit](http://poedit.net) 開啟目前使用的翻譯檔, ie. `zh_TW.po`.
點選 Catalog > Update from POT File > 選取對應的更新版翻譯檔 > 存檔

## 發現Bug或譯文錯誤
請編輯`zh_TW.po`後以github pull request 通知作者.

## 版權資訊

MIT