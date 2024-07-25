# 4d-topic-ios
4D 20以降で4D for Mobile (iOS) をセットアップするには

[4D for Mobile](https://jp.4d.com/4D-for-Mobile)はネイティブモバイルアプリ（AndroidまたはiOS）をノーコードで作成するツール。

ウィザードの指示に従い，項目を選択すると，4DデータベースアプリケーションのREST API（URLが`/MobileApp/`で始まる）と通信するモバイルアプリのソースコードがSwiftまたはKotlinで生成され，XcodeまたはAndroid Studioでビルド＆デプロイする仕組み。

## 変遷

* v17 R2~R6: [4D for iOS (beta)](https://blog.4d.com/ja/its-time-to-fire-up-your-first-4d-for-ios-project/)がMac版のデザインモードに統合される
* v18: [4D for iOS](https://blog.4d.com/ja/4d-v18-is-here/)が正式にリリースされる
* v19: [4D for Android (beta)](https://blog.4d.com/4d-for-android-is-here/)がデザインモードに統合される
* v19 R2: [4D for Android](https://blog.4d.com/ja/go-mobile-with-4d-a-single-project-to-generate-android-and-ios-apps/)が正式にリリースされる
  * 過去の[4D for iOSドキュメント](https://developer.4d.com/4d-for-ios/ja/)がアーカイブされる
* v19 R2~R8: 4D for iOSと4D for Androidの名称が[4D for Mobile](https://developer.4d.com/go-mobile/ja/docs/19-R8/getting-started/introduction/)に統一される
* v20: 4D for Mobileが[追加コンポーネント](https://blog.4d.com/ja/4d-for-mobile-goes-open-source-a-big-step-for-the-community/)となる

4D for Mobileのブログ記事とチュートリアルは[まとめページ](https://blog.4d.com/categories/4d-for-mobile/)を参照

## 注意点

* 新旧のドキュメントが存在する。[旧ページ]は初期の4D for iOSが対象。最新の4D 20, 4D for Mobile, Xcodeには対応していない。
* 4D for iOS（または4D for MobileのiOS部分）はXcodeのバージョンが厳密に合っていないと使えない。

|4D|Swift|iOS|Xcode|macOS|
|-|-|-|-|-|
|20	 |5.8	 |16.0|14.3  |13.0   |
|19R8|5.8  |16.0|14.3  |13.0   |
|19R7|5.7.1|16.0|14.1  |12.5   |
|19R6|5.7  |16.0|14.0  |12.5   |
|19R5|5.6.1|15.5|13.4  |12.5   |
|19R4|5.6  |15.4|13.3  |12.5   |
|19R3|5.5.2|15.2|13.2.1|12.5   |
|19R2|5.5  |15.0|13.1  |12.5   |
|19.2|5.5	 |15.0|13.1  |11.3   |
|19	 |5.4	 |14.6|12.5  |11.0.1 |
|18R6|5.3.2|14.4|12.4  |10.15.4|
|18R5|5.3	 |14.2|12.2  |10.15.4|
|18R4|5.3	 |14.0|12.0  |10.15.2|
|18R3|5.2.4|13.5|11.5  |10.15.2|
|18R2|5.1.3|13.3|11.3.1|10.14.4|
|18.3|5.3	 |14.2|12.2  |10.15.4|
|18.2|5.2  |13.4|11.4  |10.15.2|
|18.1|5.1.3|13.3|11.3.1|10.14.4|
|18  |5.1  |13.2|11.2  |10.14.4|
|17R6|5.0  |12.2|10.2.1|10.14.4|
|17R5|4.2.1|12.2|10.2  |10.14.3|
|17R4|4.2.1|12  |10.1  |10.13.6|
|17R3|4.2  |12  |10.0  |10.13.6|
|17R2|4.1.2|11.4|9.4   |10.13.2|
