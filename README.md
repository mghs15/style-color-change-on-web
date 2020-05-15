# style-color-change-on-web
バイナリベクトルタイルのスタイル（色）をウェブサイト上で動的に変えてみる試験

[gsi-style-color-analysis](https://github.com/mghs15/gsi-style-color-analysis)での検討をJavascriptで実装したものです。

## サンプル
### メインカラーとアクセントカラーで指定 
https://mghs15.github.io/style-color-change-on-web/main.html

プログラムの内容についてメモ程度ですが、`test.md`に記述しています。

### 色相を一定間隔で変更
https://mghs15.github.io/style-color-change-on-web/index2.html

* 単純に、色相（H）を一定値ずつ変化させます。
* ベースとなるスタイルは地理院地図Vectorの標準地図（手を入れています）。

## 利用したライブラリやコード、参考文献
* Pickr https://github.com/Simonwep/pickr
* Mapbox GL JS https://docs.mapbox.com/mapbox-gl-js/overview/
* 地理院地図Vector https://github.com/gsi-cyberjapan/gsimaps-vector-experiment
* HSL and HSV (Wikipedia) https://en.wikipedia.org/wiki/HSL_and_HSV
* gsi-vector-style-converter https://github.com/mghs15/gsi-vector-style-converter
* ベクトルタイルカラーデザイン変更ツール https://github.com/gsi-cyberjapan/gsivectortile-color-design

## 備考
タイトルは ~ on the web　が正しいのだろうけど、長くなるので、theはとった。 

