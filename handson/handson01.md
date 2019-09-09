# ハンズオン01

## Colaboratoryの使用準備と使い方の説明 (10分)

* Google Colaoratoryの有効化（有効化していない人のみ） (2分)
* Google Colaoratory Notebookの作成 (2分)
* Pythonのバージョンの設定、確認、HelloWorld (2分)
```Python
print "Hello world!"
```
* Google Colaoratory Notebookへのファイルアップロード (2分)
```Python
from google.colab import files
uploaded = files.upload()
```
* Google Colaoratory Notebookでのパッケージのインストール (2分)

  - 例
  ```Python
  !pip install tensorflow
  ```

## 「あやめの分類」にチャレンジしよう (40分)

Pythonプログラムの解説もします。（強制ではありませんが、こちらの本をお持ちですとスムーズかもしれません。https://github.com/Kokensha/book-ml）

* 参考: https://github.com/Kokensha/book-ml/blob/master/Colaboratory/04_03(scikit_learn_iris).ipynb
* 機械学習向けフレームワークscikit-learnの紹介 (5分)
* 機械学習のはじめの第一歩「あやめの分類」の概要 (2分)
  setosa, versicolor, virginica
* アヤメデータの説明(データに慣れる) (10分)
* 分類と回帰 (2分)
  - 分類の例
  - 回帰の例
* サポートベクターマシンの紹介と理論の解説 (2分)
* 超平面（Hyper-plane） (2分)
* 交差検証 (5分)
* 学習と検証 (5分)
* 実際に「あやめの分類」をやってみよう  (2分)


## 今後(5分)

* 今後は「じっくりハンズオンクラス」と「ビジネスオリエントクラス」開講も検討しています。「じっくりハンズオンクラス」は、初心者向けでゆっくりしっかり基礎から、大量のレシピをクリアしていくことで、機械学習と深層学習の重要基本をしっかり身に着けるコースです。「ビジネスオリエントクラス」は機械学習、深層学習の実際の業務をイメージして、特訓する中級学習コースとなります。（内容変更、調整することがあります。）

## 質疑応用（0-30分）

## 片付け、解散
