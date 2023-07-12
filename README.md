# 5374について
For English please see [LOCALIZE_en.md](LOCALIZE_en.md).
##「いつ、どのゴミが収集されているのか？」

ゴミの問題はどの地域でも深刻になりつつあります。
 [Code for Kanazawa](http://codeforkanazawa.org/)
では、先ずは正しいゴミの捨て方に注目しました。例えばお引っ越しをされた場合、このアプリを使えばすぐに分かるように、目的と使い方をとてもシンプルにデザインしました。

## ブランチの運用について

* **master**: ローカライズをする場合にはこのブランチをforkしてください (2014/5/7 updated v1.1)
* **kanazawa**: 5374の金沢バージョン
* **gh-pages**: 5374の金沢バージョンリリースブランチ
* **dev**: 今後kanazawaへ適用予定の開発ブランチ

## 使い方について

[HOWTOUSE.md](HOWTOUSE.md)に5374標準の文章を用意してあるので、書き換えて使ってください。

## ローカライズについて

各地域へのローカライズについては[LOCALIZE.md](LOCALIZE.md)を参照するようにしてください。




## 開発チームとライセンスについて
- 小野 祐貴(Yuki ONO)　Developer
- 五十川 員申(Kazunobu IKAGAWA)　Developer
- 高木 志宗(Yukimune TAKAGI)　Developer
- 宮田 人司(Hotoshi MIYATA)　Designer

本アプリ及びソースコードの著作権はCode for Kanazawaに帰属します。
但し、このソースコードは[MPL](http://www.mozilla.org/MPL/2.0/)のもと配布されています。MPLに従えば、どなたでも利用、改変、及び再配布が可能です。

## オープンデータカタログサイトで公開しているデータの自動反映について

オープンデータカタログサイトで公開している[5374アプリ用データセット](https://data.bodik.jp/dataset/262129_5374)内の次のデータを、「data」ディレクトリ内の同ファイルへ自動で上書きします。  
- 地区の収集スケジュール(area_days.csv)
- ごみ区分の対象となるごみ種類(target.csv)
- 収集センターの休止期間(center.csv)
- ごみの区分(description.csv)

更新タイミングは1日1回。更新の有無は関係なく、無条件で上書きされます。  
なお、Google App Scriptを利用して、ファイルの更新をしています。  
