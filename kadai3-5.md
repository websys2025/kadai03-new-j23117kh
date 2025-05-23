## 自動販売機（データ構造と各種処理）のミニレポート
### Q5-1. 自動販売機の商品データついて説明せよ。
* データ構造（各項目とその説明）
* ①：配列 items：商品の一覧を記録する連想配列の配列
* ②：関数 showItemList：商品の一覧を表示する関数
* ③：関数 buyItem:商品を購入する関数
* 連想配列の配列として定義するメリット：キーと値のペアでデータを管理できる。つまり、よりわかりやすくデータを管理できる
### Q5-2. showItemListの処理内容について説明せよ。
* 配列の繰り返し処理：
  itemsは商品情報の入った配列。
  iは配列の位置番号で、0からitems.length-1まで繰り返す。
  items[i]で、現在のインデックスにある商品オブジェクトを取得。
* 連想配列の参照方法：
  item.idは商品番号。
  item.nameは商品名。
  item.priceは価格。
  item.stockは在庫数。
### Q5-3. buyItemの処理内容について説明せよ。
* 商品購入の可否判定:item.stock>0ならば購入できる。
* 商品在庫を減らす処理：item.stock=item.stock-1で在庫を1つ減らす。
* 商品番号のエラー処理：1~8ではない番号を入力すると警告文を出す
### Q5-4. プログラムの考察
* データ構造について：
  配列を使うことによって、追加の入力や削除ができやすくなっている。
  関数を使うことで、何回も使う処理を簡単に実行できる
* 商品一覧表示と購入処理を関数化したメリット：
  何回も同じ処理を書かなくて済む。
  コードの追加や削除がしやすくなる
### Q5-5. 感想
* 今回の課題で苦労したこと：
  プログラム独自の書き方を調べること。
  連想配列の使い方。
  エラーが出る場所が毎回変わったこと。
* 演習を通して理解できたこと：
  if文や繰り返しなど今まで習ったプログラムの知識がここでも生かされること。
  関数の便利さ。
* この自動販売機プログラムの追加機能や課題など：
  値段があるのにお金を入れる操作がない。
  まとめて商品を買えるようにする。
