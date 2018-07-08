# postal_codes_search

## 言語
PHP

## 説明
postal_codes_searchディレクトリ配下のapiディレクトリを一式を、
ApacheとPHPがインストールしているWebサーバにアップ頂ければ動作します。
郵便番号のデータ（カスタマイズ版）もソースファイルに含みましたのでDBの設定は不要です。
ローカルではWindowsのXAMPP7.2.6 (PHP 7.2.6)にて確認致しました。

## 例
1.リクエスト
- Apacheのmod_rewriteが有効の場合
```
http://localhost/api/postal_codes/search?code=1010051
```

- Apacheのmod_rewriteが無効の場合
```
http://localhost/api/postal_codes/search.php?code=1010051
```

2.レスポンス
```
{ "prefecture": "東京都", "city": "千代田区", "address_line": "神田神保町" }
```

## 補足
「search.php」と同階層に「debug.html」というファイルがあり、ブラウザからご覧頂けます。
