# FUNC_ARRAY

FANUC KAREL 言語で配列を多少使いやすくできそうなやつ  
配列へ要素の Append や Insert, Delete, Sort などを行うことができます。

## 使い方

ROBOGUIDE、Myworkcell のプロジェクトファルダへ KAREL フォルダをコピーし、  
databox.kl をビルドして下さい。  
また、配列関数を使いたい対象 KAREL プログラムに  
%INCLUDE includes/databox.h  
と追記することで利用できます。

## 関数

他言語とほぼ同様の命令として利用可能。  
詳細な引数・戻り値についてはソースコードを参照してください。  
(あとで追記したい)

## License

Released under the Apache 2.0 License.
