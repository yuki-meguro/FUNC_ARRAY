# FUNC_ARRAY

FANUC KAREL 言語で配列を多少使いやすくできそうなやつ  
配列へ要素の Append や Insert, Delete, Sort などを行うことができます。

## 使い方

ROBOGUIDE、Myworkcell のプロジェクトファルダへ KAREL フォルダをコピーし、  
databox.kl をビルドして下さい。  
また、配列関数を使いたい対象 KAREL プログラムに  
%INCLUDE includes/databox.h  
と追記することで利用できます。

## 注意

未初期化エラーを回避するために初回実行時には必ず、  
**ListClear**を実行して下さい。

## 関数

### ListClear

配列の要素をすべてクリアします。

- 引数  
  無し
- 戻り値(integer)  
  0: Pass / 1: Error

### ListAppend

配列に要素を追加します。

- 引数(integer)  
  配列に追加したい要素
- 戻り値(integer)  
  0: Pass / 1: Error

### ListDelete

配列のある位置の要素を削除します。

- 引数(integer)  
  配列内の削除したい要素番号
- 戻り値(integer)  
  0: Pass / 1: Error

### ListInsert

配列のある位置に要素を挿入します。

- 引数 1(integer)  
  挿入したい位置

- 引数 2(integer)  
  挿入したい要素

- 戻り値(integer)  
  0: Pass / 1: Error

### ListVal

配列のある位置の要素を返します。

- 引数 1(integer)  
  返したい要素番号
- 戻り値(integer)  
  配列要素

### ListLen

配列の長さを返します。

- 引数  
  無し
- 戻り値(integer)  
  配列の長さ

### ListIn

配列に特定の要素が含まれているか確認し BOOL で返します。

- 引数(integer)  
  確認したい要素

- 戻り値(boolean)  
  True: 含まれている / False: 含まれていない

### ListSort

配列の要素をソートします。

- 引数  
  無し
- 戻り値(integer)  
  0: Pass / 1: Error

## License

Released under the Apache 2.0 License.
