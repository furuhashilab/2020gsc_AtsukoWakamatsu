## 2020年古橋研究室　ゼミ論
３年　若松暖子　ゼミ論用レポジトリになります。
## 日本全国のとんかつ店の位置情報オープン化実践に向けたタグの提案
学籍番号:1A118185  
氏名：若松暖子  
地球社会共生学部3年A組184番  
指導教員：古橋大地教授  
© Furuhashi Laboratory/Taro Aoyama, CC BY 4.0
## 概論

## Introduction
明治時代の文明開化を通して肉食が一般化され、西洋料理が白米に合う形で適応していった。その中の一つに「cutlet」がある。cutletは国産のウスターソースと合わせることによって家庭の味として広く浸透し、カレーライス、コロッケと共にとんかつは三代洋食の一つとして称されるようになり、現在では全国に多くとんかつ店が出店されいる。  
しかし、OSM上ではとんかつ店の位置情報の整理は行われていない。そこで、本研究ではOSMのオープンな地理空間情報プラットフォームを用いて、日本全国の2021年1月時点のとんかつ店のデータを整理し、タグルールの提案によって、今後のOSM上におけるとんかつ店の編集を自由に位置情報データにアクセスできることを試みた。

## Methods
[OSM上に載っているとんかつ店舗情報](https://docs.google.com/spreadsheets/d/1xnWAmlLVDLfa12DDGjNbNfGhFdzVgP8gkxIkSMBPE1U/edit?usp=sharing)をスプレッドシートを使用し、まとめた。  
OSM上のとんかつ店の情報を整理した。2021年1月時点における
* OSM TagInfo内で ”とんかつ” と検索してヒットするnameタグ　48件
* 店舗情報（Node）として既にOSM上に存在していたのが　45件
* 既存の ”とんかつ” POIデータのamenityタグの種類について
  * amenity=fast_food として登録されていた店舗が14店舗
  * amenity=restaurant として登録されていた店舗が32店舗
  * 未記入が2店舗であった
* cuisineの種類について
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
以上を踏まえた上で、OSMwiki上にとんかつ屋のページを作成し、今後のとんかつ店をタグ付けする上での注意点を提示、タグルールの提案を行った。
## Results
現在登録されているとんかつ店情報の整理と、登録情報の確認を行った。 
緊急事態宣言のため、FWをベースとした現地調査を行うことができなかった。
とんかつ店においてタグの統一ルールがなく、cuisine=とんかつ,cuisine=japaneseなどとんかつの定義が登録者によって異なることがわかった。
また「とんかつ」、「豚カツ」「豚かつ」「トンカツ」と日本語だけでも表記の仕方が異なり、OSM上に登録されているすべてのとんかつ店を見つけることが難しい。

## Discussion
上記の結果を踏まえ、今後のOSM上でのとんかつ店の表記、タグルールを提案・検討したものをOSM wiki上の[「とんかつ屋」](https://wiki.openstreetmap.org/wiki/%E3%81%A8%E3%82%93%E3%81%8B%E3%81%A4%E5%B1%8B)ページに記載した。
### ①とんかつの表記はどのようにすべきか。
とんかつ、豚カツ、豚かつ、トンカツに正しい表記は存在しない。
#### とんかつの歴史の観点から
増子（２０１９）によれば、「明治 40 年初頭には、屋台料理の一つとして「ポークカツレツ」が「トンカツ」と呼ばれ定着していた.  
しかし、「トンカツ」という名称は家庭向けの料理書には記載が無く、おそらくスラングとされていて正式名称としては扱われず、公的な場所では使用されなかったと考えられる。
屋台料理の「トンカツ」から「とんかつ」へと何らかの要因によって表記が変化していったとされる。」とある。  
#### 言語表記の観点
国語辞典の表記によれば「豚カツ」として記載されている。これは「とんかつ」の「とん」は漢語「豚（とん）」、「かつ」は外来語「カツ（もとは英語のcutlet）」であることから、「豚カツ」という書き方が正式であると考えられているからとされる。
#### OSMにおけるとんかつ店の情報から
OSM TagInfo内での検索した結果
* ”とんかつ” と検索してヒットするnameタグ　48件
* "豚カツ” と検索してヒットするnameタグ　2件
* ”豚かつ” と検索してヒットするnameタグ　0件
* ”トンカツ” と検索してヒットするnameタグ　4件
* ”tonkatsu” と検索してヒットするnameタグ　24件
であった。
私が実際に行ったことのあるとんかつ店１１店舗のうち全ての店舗ののれんが「とんかつ」と表記していた。  
以上から、**「とんかつ」がもっとも一般的な呼び名として利用されている**と言える。
### ②とんかつ店のamenity=restaurant,amenity=fastfoodの検討 
OSM wiki によるとそれぞれ下記のように定義されている。
#### amenity=restaurant
amenity=restaurant は座席があり、ウェイターが給仕して、一式の食事を提供する、一般的にフォーマルなレストランのためのものです。（許可制の場所では）多くは酒類の販売免許を得ているもの。
* 座席があること
* ウェイターが給仕すること
* 酒類の販売
#### amenity=fast_food
amenity=fast_foodは早いカウンターのみのサービスと、食べ物の持ち帰りに重点を置く場所です。食べ物を食べる前に、カウンターで支払いを済ませます。使い捨ての皿やその他の素材で食べ物を提供し、プラスティックの食器で食べます。たいていは、必ずではありませんが、２～３個以上の、掃除しやすい椅子とテーブルの座席があります。
* カウンター席のみのサービス（支払いも含む）
* 持ち帰り可能
* プラスティックの容器
* ２〜3個以上の掃除しやすい椅子とテーブルの座席
#### 酒類の販売について
松屋フーズが経営する松乃家、とんかつ和幸などのとんかつチェーンでは店舗によるもののビールなどの酒類の販売を行っている。
個人が経営するとんかつ店においてもお酒をおいているお店は多い。
よってrestaurantのタグに当てはまると言える。
#### 持ち帰り制度と座席について
松のやなどのチェーン店では券売機での支払いを先に済ませ、店内で食べる場所と持ち帰りができるようなシステムを採用している。
一方で、チェーン店でない個人経営のとんかつ店ではカウンター席、テーブル席があり、ウェイターが給仕するamenity=restaurantのような仕様である場合が多い。新型コロナウイルスの影響により一部店舗では持ち帰りサービスを開始しているが、多くの店は持ち帰りよりもテーブル席で食事をすることを主としているためrestaurantタグが望ましいと考えられる。
#### JA:Naming sampleにおけるとんかつチェーン店の位置付け
JA:Naming sampleを参考にすると、amenity=restaurantの欄にとんかつチェーンである和幸が存在する。
これらを踏まえて、とんかつ店は基本的に**amenity=restaurant**に統一できるのではないかと考える。
### ③とんかつ店のcuisineタグはどのように統一すべきか。
とんかつは和食、郷土料理、フライ料理、または”とんかつ”として分類できるのかを検討した。  
とんかつ店61店舗の情報のうちcuisineタグは７種類存在した。 
#### とんかつ店におけるcuisineタグの種類
* "japanese"として登録されていたPOIが19店舗
* "japanese;pork cutlet"として登録されていたPOIが1店舗
* "tonkatsu"として登録されていたPOIが９店舗
* "regional"として登録されていたPOIが２店舗
* "fried_food"として登録されていたPOIが１店舗
* "friture"として登録されていたPOIが１店舗
* "friture;japanese"として登録されていたPOIが１店舗
* 未記入が14店舗 であった
#### 使用されたタグの検討
OSM wiki定義によればcuisineは飲食が可能な場所で提供される、料理の種類を記述したものである。 使用されたタグをそれぞれ検討してみる。
* cuisine= japanese　 和食
* cuisine=regional　郷土料理、正確な説明がない場合に使用
* cuisine=fried_food　油で挙げられた食べ物たいていは持ち帰り用
* cuisine=friture　オランダやベルギーのチップ店
* cuisine=tonkatsu　は値としての定義は存在しなかった。  
とんかつはjapaneseの中の一つであるtonkatsuとして定義することができる。  
韓国では日本と同じスタイルのとんかつ店が存在し、韓国語の表記では「돈까스」(ton-kka-ssŭ)となる。 
TagInfo内で ”돈까스” と検索してヒットするnameタグ　3件存在した。  
これは明治維新時に「cutlet」として輸入されたものが、当時日本統治下であった韓国に流れ、洋食としての「cutlet」に似た「とんかつ」であるため、日本のとんかつとは似て非なるものであると捉えることができる。  
和食としてのとんかつを考慮し、**cuisineタグは「japanese;tonkatsu」** を提案する。

## Conculsion
本研究を通してOSM上にある既存のとんかつ店の情報未整備の現状を明らかにし、新たなタグルールの提案を行った。そして今後とんかつ店をOSM上で編集していく上でOSMwikiページを作成した。
課題として、現地調査を元にしたとんかつ店における必要情報は何かを明らかにしタギングルールの統一、また正式にcusineタグ「japanese;tonkatsu」の承認に向けた取り組みが挙げられる。
## 参考文献
[参考文献リスト](https://docs.google.com/spreadsheets/d/1RqsegRZAp1sKmjVZdPUnq_JEwCtUKe6rBDOQLTgyyLk/edit?usp=sharing)
* 渡辺結南　[日本全国のラーメン二郎店舗位置情報オープン化の実践](https://furuhashilab.github.io/www4yunawatanabe/)
* 増子保志　[「とんかつと受容に関するー考察」](https://www.jstage.jst.go.jp/article/gscs/16/1/16_3/_pdf/-char/ja)

## 謝辞
本研究を進めるにあたり地球社会共生学部の古橋大地教授をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

## 進捗管理用プロジェクト
https://github.com/furuhashilab/sotsuron2020/projects/21
## 発表用プレゼンテーション


