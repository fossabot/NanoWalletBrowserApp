# NanoWalletBrowserApp

# **注意 これは開発版です。開発者は、このプログラム、また関連するもので生じた一切の責任を負いません。完全な自己責任で使用してください。**

**English doc is README-en.md**

## これは何？
New Economy Movementの総合管理ソフト「Nano Wallet」を、様々なブラウザでアプリ・アドオンとして動作させるためのものです。
## 対応ブラウザ


|ブラウザ        |状況                  |
|:-------------:|:--------------------:|
|Chrome アプリ   |一応動く               |
|Chrome 拡張機能|一応動く               |
|Firefox アドオン|作成中                 |

## ビルドの仕方
※ビルドには、GNU make、npm、nodejs、gulpが必要です。

ダウンロードしたら、makeしてください。何も指定せずにmakeすると、dist/にブラウザアプリ・アドオンのインストール形式のファイルが生成されます。

```
$ make
```

もし特定のブラウザアプリ・アドオンだけをビルドしたいときは、以下のように入力してください。
```
$ make chrome_app         #chromeアプリ版
$ make chrome_extension   #chrome拡張機能版
$ make firefox            #firefoxアドオン版
```
## インストールの仕方
### Chrome アプリ
1. chrome://extensions/ をブラウザで開いてください。
2. その画面に、dist/chrome_app.crxをドラッグ・アンド・ドロップしてください。
3. ダイアログ通りに進めれば完了です。 chrome://apps/ から起動することができます。またパソコンのスタートメニューやDashにも自動的に追加されます。

### Chrome 拡張機能
1. chrome://extensions/ をブラウザで開いてください。
2. その画面に、dist/chrome_extension.crxをドラッグ・アンド・ドロップしてください。
3. ダイアログ通りに進めれば完了です。 アドレスバーの横から起動することができます。通常はポップアップで表示されますが、右クリック->オプションを選択することで、新しいタブで起動することができます。

※なお、Chrome拡張機能はMicrosoft Edge,Opera,Vivaldiで、開発中ですが動作するとの報告があります。
### Firefox アドオン
作成中

