# php-mtn-v03-update-insert-sqlite

![image](https://github.com/winofsql/php-mtn-v03-update-insert-sqlite/assets/1501327/f883da16-f57c-4f99-8ffb-bb30ff25489f)

## 新規登録を追加

```php
if ( $_POST["btn"] == "更新" ) {

    $row = check( $sqlite );
    // 社員コードが存在する
    if ( $row ) {
        update( $sqlite );
    }
    // 社員コードが存在しない
    else{
        insert( $sqlite );
    }

    $_POST["scode"] = "";
    $_POST["sname"] = "";
    $_POST["fname"] = "";
    $_POST["syozoku"] = "";
    $_POST["seibetsu"] = "";
    $_POST["kyuyo"] = "";
    $_POST["teate"] = "";
    $_POST["kanri"] = "";
    $_POST["birth"] = "";
}```
