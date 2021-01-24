## 2020年古橋研究室　ゼミ論
３年　若松暖子　ゼミ論用レポジトリになります。
## 日本全国のとんかつやの位置情報の整理
学籍番号:1A118185  
氏名：若松暖子  
地球社会共生学部3年A組184番  
指導教員：古橋大地教授

## 概論

## Introduction
明治時代の文明開化を通して肉食が一般化され、西洋料理が白米に合う形で適応していった。その中の一つに「cutlet」がある。cutletは国産のウスターソースと合わせることによって家庭の味として広く浸透し、カレーライス、コロッケと共にとんかつは三代洋食の一つとして称されるようになり、現在では全国に多くとんかつ店が出店されいる。  
しかし、OSM上ではとんかつ店の位置情報の整理は行われていない。そこで、本研究ではOSMのオープンな地理空間情報プラットフォームを用いて、日本全国の2021年1月時点のとんかつ店のデータを整理し、タグルールの提案によって、自由に位置情報データにアクセスできることを試みた。

## Methods
[OSM上に載っているとんかつ店舗情報](https://docs.google.com/spreadsheets/d/1xnWAmlLVDLfa12DDGjNbNfGhFdzVgP8gkxIkSMBPE1U/edit?usp=sharing)をスプレッドシートを使用し、まとめた。  
OSM上のとんかつ店の情報を整理した。2021年1月時点における
* OSM TagInfo内で ”とんかつ” と検索してヒットするnameタグ　48件
* 店舗情報（Node）として既にOSM上に存在していたのが　45件
* 既存の軒の ”とんかつ” POIデータのうち amenity=fast_food として登録されていた店舗が14店舗、amenity=restaurant として登録されていた店舗が32店舗、未記入が2店舗であった
* cuisine=japaneseとして登録されていたPOIが19店舗 
* cuisine=japanese;pork cutletとして登録されていたPOIが1店舗 
* cuisine=tonkatsuとして登録されていたPOIが９店舗 
* cuisine=regionalとして登録されていたPOIが２店舗 
* cuisine=fried_foodとして登録されていたPOIが１店舗 
* cuisine=fritureとして登録されていたPOIが１店舗 
* cuisine=friture;japaneseとして登録されていたPOIが１店舗 
* cuisine＝未記入が14店舗 であった
* OSM TagInfo内で ”豚カツ” と検索してヒットするnameタグ　2件のうち1件が”とんかつ”で検索したうちのものであった。
* OSM TagInfo内で ”tonkatsu” と検索してヒットするnameタグ　24件  
 うち１３件が上記の結果に含まれていないものであった。
* OSM TagInfo内で ”豚かつ” と検索してヒットするnameタグ　0件
* 建物（Node）としてではなく、道路（way）として登録されているものも存在した。
* タグが統一されておらず、64種類のタグが使用されていた。
* 多言語表示に対応しているものとそうでないものが存在した。

## Results
現在登録されているとんかつ店情報の整理と、登録情報の正誤確認を行った。 
緊急事態宣言のため、FWをベースとした現地調査を行うことができなかった。
とんかつ店においてタグの統一ルールがなく、cuisine=とんかつ,cuisine=japaneseなどとんかつの定義が登録者によって異なることがわかった。
また「とんかつ」、「豚カツ」「豚かつ」「トンカツ」と日本語だけでも表記の仕方が異なり、OSM上に登録されているすべてのとんかつ店を見つけることが難しい。
## Discussion
1. とんかつ店としてamenity=restaurant,amenity=fastfoodの違いはどこにあり、どちらのタグがふさわしいのかを検討した。  
1. とんかつ店のcuisineタグはどのように統一すべきか。
とんかつは和食、郷土料理、フライ料理、または”とんかつ”として分類できるのかを検討した。  
1. とんかつ店における必要情報は何か。  
それぞれに異なるタグが使用されていた。一つのNodeに多いもので28個、少ないもので3個のタグが使われていた。



## Conculsion
## 参考文献
* 渡辺結南　[日本全国のラーメン二郎店舗位置情報オープン化の実践](https://furuhashilab.github.io/www4yunawatanabe/)
* 増子保志　[「とんかつと受容に関するー考察」](https://www.jstage.jst.go.jp/article/gscs/16/1/16_3/_pdf/-char/ja)
## 謝辞
本研究を進めるにあたり地球社会共生学部の古橋大地教授をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

## 2020年度卒業論文提出用
## 発表用プレゼンテーション

