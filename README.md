# 源氏物語 形態論情報データ (OpenCHJ)

本データは、「源氏物語」の全文に短単位の形態論情報を付与したものです。

## 本文について
本文は、以下のテキストをもとにしています。  
（XML版をもとに、解析対象としないテキストを空要素の属性値にするなどの変更を行ったうえで解析しました。）

- **渋谷栄一氏**による源氏物語テキスト  
  **[源氏物語の世界](http://www.sainet.or.jp/~eshibuya/index.html)**：© 1996, 2014 渋谷栄一  
- **宮脇文経氏**による再編集版（XML版）  
  **[源氏物語の世界 再編集版](https://www.genji-monogatari.net/)**：© 2003, 2024 宮脇文経  

## 形態論情報について
形態論情報は **[中古和文UniDic](https://clrd.ninjal.ac.jp/unidic/download_all.html#unidic_wabun)** を使用して短単位に解析し、エラーを修正したものです。

「桐壺」巻以外の修正は十分ではなく、誤りが含まれていますが、語彙素認定（境界・見出し語・品詞・活用形の全てが正解）のレベルにおいて概ね98～99％以上の精度で解析されています。

## ライセンス
- 形態論情報：**[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)** BY **[小木曽智信](https://researchmap.jp/togiso)**
- 本文自体のライセンスについては上記のオリジナルサイトを参照してください。

## ファイル形式
- UTF-8 (BOMなし) LF改行, タブ区切り
- フィールド（左から）
  - ファイル名（巻名）
  - サブコーパス名
  - 開始文字位置（ファイル頭からのオフセット値*10）
  - 終了文字位置（同上）
  - 文境界（B=文頭）
  - 書字形出現形（=キー, 表層形）
  - 語彙素
  - 語彙素読み
  - 品詞
  - 活用型
  - 活用形
  - 発音形
  - 語種
 
## データサンプル
```
01.01桐壺	OH_OO渋谷源氏	10	40	B	いづれ	何れ	イズレ	代名詞			イズレ	和
01.01桐壺	OH_OO渋谷源氏	40	50	I	の	の	ノ	助詞-格助詞			ノ	和
01.01桐壺	OH_OO渋谷源氏	50	60	I	御	御	オオン	接頭辞			オオン	和
01.01桐壺	OH_OO渋谷源氏	60	70	I	時	時	トキ	名詞-普通名詞-副詞可能			トキ	和
01.01桐壺	OH_OO渋谷源氏	70	80	I	に	に	ニ	助詞-格助詞			ニ	和
01.01桐壺	OH_OO渋谷源氏	80	90	I	か	か	カ	助詞-係助詞			カ	和
01.01桐壺	OH_OO渋谷源氏	90	100	I	、	、		補助記号-読点				記号
01.01桐壺	OH_OO渋谷源氏	100	120	I	女御	女御	ニョウゴ	名詞-普通名詞-一般			ニョーゴ	漢
01.01桐壺	OH_OO渋谷源氏	120	130	I	，	，		補助記号-読点				記号
01.01桐壺	OH_OO渋谷源氏	130	150	I	更衣	更衣	コウイ	名詞-普通名詞-サ変可能			コーイ	漢
01.01桐壺	OH_OO渋谷源氏	150	180	I	あまた	数多	アマタ	名詞-普通名詞-一般			アマタ	和
01.01桐壺	OH_OO渋谷源氏	180	220	I	さぶらひ	侍う	サブラウ	動詞-一般	文語四段-ハ行	連用形-一般	サブライ	和
01.01桐壺	OH_OO渋谷源氏	220	250	I	たまひ	給う	タマウ	動詞-非自立可能	文語四段-ハ行	連用形-一般	タマイ	和
01.01桐壺	OH_OO渋谷源氏	250	270	I	ける	けり	ケリ	助動詞	文語助動詞-ケリ	連体形-一般	ケル	和
01.01桐壺	OH_OO渋谷源氏	270	290	I	なか	中	ナカ	名詞-普通名詞-副詞可能			ナカ	和
01.01桐壺	OH_OO渋谷源氏	290	300	I	に	に	ニ	助詞-格助詞			ニ	和
01.01桐壺	OH_OO渋谷源氏	300	310	I	、	、		補助記号-読点				記号
01.01桐壺	OH_OO渋谷源氏	310	330	I	いと	いと	イト	副詞			イト	和
01.01桐壺	OH_OO渋谷源氏	330	390	I	やむごとなき	やんごとない	ヤンゴトナイ	形容詞-一般	文語形容詞-ク	連体形-一般	ヤンゴトナキ	和
01.01桐壺	OH_OO渋谷源氏	390	400	I	際	際	キワ	名詞-普通名詞-一般			キワ	和
01.01桐壺	OH_OO渋谷源氏	400	410	I	に	に	ニ	助詞-格助詞			ニ	和
01.01桐壺	OH_OO渋谷源氏	410	420	I	は	は	ハ	助詞-係助詞			ワ	和
01.01桐壺	OH_OO渋谷源氏	420	440	I	あら	有る	アル	動詞-非自立可能	文語ラ行変格	未然形-一般	アラ	和
01.01桐壺	OH_OO渋谷源氏	440	450	I	ぬ	ず	ズ	助動詞	文語助動詞-ズ	連体形-一般	ヌ	和
01.01桐壺	OH_OO渋谷源氏	450	460	I	が	が	ガ	助詞-格助詞			ガ	和
01.01桐壺	OH_OO渋谷源氏	460	470	I	、	、		補助記号-読点				記号
01.01桐壺	OH_OO渋谷源氏	470	500	I	すぐれ	優れる	スグレル	動詞-一般	文語下二段-ラ行	連用形-一般	スグレ	和
01.01桐壺	OH_OO渋谷源氏	500	510	I	て	て	テ	助詞-接続助詞			テ	和
01.01桐壺	OH_OO渋谷源氏	510	520	I	時	時	トキ	名詞-普通名詞-副詞可能			トキ	和
01.01桐壺	OH_OO渋谷源氏	520	540	I	めき	めく	メク	接尾辞-動詞的	文語四段-カ行	連用形-一般	メキ	和
01.01桐壺	OH_OO渋谷源氏	540	570	I	たまふ	給う	タマウ	動詞-非自立可能	文語四段-ハ行	連体形-一般	タマウ	和
01.01桐壺	OH_OO渋谷源氏	570	590	I	あり	有る	アル	動詞-非自立可能	文語ラ行変格	連用形-一般	アリ	和
01.01桐壺	OH_OO渋谷源氏	590	610	I	けり	けり	ケリ	助動詞	文語助動詞-ケリ	終止形-一般	ケリ	和
01.01桐壺	OH_OO渋谷源氏	610	620	I	。	。		補助記号-句点				記号
01.01桐壺	OH_OO渋谷源氏	620	650	B	はじめ	始め	ハジメ	名詞-普通名詞-副詞可能			ハジメ	和
01.01桐壺	OH_OO渋谷源氏	650	670	I	より	より	ヨリ	助詞-格助詞			ヨリ	和
01.01桐壺	OH_OO渋谷源氏	670	680	I	我	我	ワレ	代名詞			ワレ	和
01.01桐壺	OH_OO渋谷源氏	680	690	I	は	は	ハ	助詞-係助詞			ワ	和
01.01桐壺	OH_OO渋谷源氏	690	700	I	と	と	ト	助詞-格助詞			ト	和
01.01桐壺	OH_OO渋谷源氏	700	720	I	思ひ	思う	オモウ	動詞-一般	文語四段-ハ行	連用形-一般	オモイ	和
01.01桐壺	OH_OO渋谷源氏	720	750	I	上がり	上がる	アガル	動詞-一般	文語四段-ラ行	連用形-一般	アガリ	和
01.01桐壺	OH_OO渋谷源氏	750	780	I	たまへ	給う	タマウ	動詞-非自立可能	文語四段-ハ行	命令形	タマエ	和
01.01桐壺	OH_OO渋谷源氏	780	790	I	る	り	リ	助動詞	文語助動詞-リ	連体形-一般	ル	和
01.01桐壺	OH_OO渋谷源氏	790	800	I	御	御	オオン	接頭辞			オオン	和
01.01桐壺	OH_OO渋谷源氏	800	830	I	方がた	方々	カタガタ	名詞-普通名詞-一般			カタガタ	和
01.01桐壺	OH_OO渋谷源氏	830	840	I	、	、		補助記号-読点				記号
01.01桐壺	OH_OO渋谷源氏	840	890	I	めざましき	目覚ましい	メザマシイ	形容詞-一般	文語形容詞-シク	連体形-一般	メザマシキ	和
01.01桐壺	OH_OO渋谷源氏	890	910	I	もの	物	モノ	名詞-普通名詞-サ変可能			モノ	和
01.01桐壺	OH_OO渋谷源氏	910	920	I	に	に	ニ	助詞-格助詞			ニ	和
01.01桐壺	OH_OO渋谷源氏	920	960	I	おとしめ	貶める	オトシメル	動詞-一般	文語下二段-マ行	連用形-一般	オトシメ	和
01.01桐壺	OH_OO渋谷源氏	960	980	I	嫉み	嫉む	ソネム	動詞-一般	文語四段-マ行	連用形-一般	ソネミ	和
01.01桐壺	OH_OO渋谷源氏	980	1010	I	たまふ	給う	タマウ	動詞-非自立可能	文語四段-ハ行	終止形-一般	タマウ	和
01.01桐壺	OH_OO渋谷源氏	1010	1020	I	。	。		補助記号-句点				記号
```
