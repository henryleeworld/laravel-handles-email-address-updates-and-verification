# Laravel 12 處理電子郵件地址更新和驗證

引入 protonemedia 的 laravel-verify-new-email 套件來擴增處理電子郵件地址更新和驗證，當使用者更新其電子郵件地址時，在驗證新電子郵件地址之前，不會取代舊電子郵件地址。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移。
```sh
$ php artisan migrate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/register` 來進行註冊。

----

## 畫面截圖
![](https://i.imgur.com/Y7tH57I.png)
> 建立新的帳號

![](https://i.imgur.com/PTBgnBc.png)
> 到註冊填寫的電子郵件地址收信，並啟動註冊的帳號，才算開通帳號
