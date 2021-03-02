# style-color-change-on-web
バイナリベクトルタイルのスタイル（色）をウェブサイト上で動的に変えてみる試験

[gsi-style-color-analysis](https://github.com/mghs15/gsi-style-color-analysis)での検討をJavascriptで実装したものです。

## サンプル
### メインカラーとアクセントカラーで指定 
https://mghs15.github.io/style-color-change-on-web/main.html

* プログラムの内容についてメモ程度ですが、`test.md`に記述しています。
* ベースとなるスタイルは地理院地図Vectorの淡色地図。RGBの微調整のほか、[railway-map-style](https://github.com/mghs15/railway-map-style)をベースに、鉄道・道路・境界の太さを調整しています。
* 配色の設計方針は`color-design.md`に記述しています。

#### ToDo
* SやLの値を工夫することで、可逆的に変換できないかといろいろ試行錯誤しているが、適当にプログラムを増築したために、相当複雑になってしまった。
* 今は、色のH,S,Lを見て、色を変換しているが、将来的には、背景色と同化させるべき色（paleでRGBが255,255,255のもの）は、metadata等で明示的に示しておいた方が、プログラムはシンプルになるはず。
* 現状、高速道路・国道の分別にmetadataのpathを利用しているので、もはや色だけで複雑な色の制御を可逆的に行うのは（作者にとっては）困難な気がする。


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
タイトルは ~ on the web が正しいのだろうけど、長くなるので、theはとった。 
