# [川島の自己紹介](kawashimaken_introduction.md)

# ハンズオン参考書籍 

*　[「今すぐ試したい！機械学習・深層学習（ディープラーニング）画像認識プログラミングレシピ」](https://amzn.to/2u1tFBu)強制ではありませんが、こちらの本をお持ちですとスムーズかもしれません。

* https://github.com/Kokensha/book-ml

# 第4回　ハンズオン

前回第3回は[こちら](handson03.md)です。

* 第1回のGoogle Colabの環境を用意して置いてください。会場もWiFiの環境が用意されていますが、可能であれば、ご自身のモバイルWiFiルータもお持ちください！

* [参考 ハンズオン（参考書籍の第４章第５節）](https://github.com/Kokensha/book-ml/blob/master/Colaboratory/04_05(Chainer_MNIST).ipynb)

## ニューラルネットワーク及びニューラルネットワークの学習についての詳説(第３回の内容復習：10分)

* [参考 概念説明](./../04_artificial_neural_network.md)

## Chainerの簡単な紹介（5分）

* 日本のプリファードネットワークス（Preffered Networks）さんが主導で開発したPythonベースオープンソース深層学習フレームワークである。

* 2015年6月にオープンソース化されました。（TensorFlowが2015年11月9日にベータ版がが公開され、2017年2月15日には正式版となるTensorFlow 1.0がリリースされた。PyTorchは Facebookが2017年公開）

* Chainerは深層学習のフレームワークの先駆けでもある

* 2019年12月5日　プリファードネットワークス、以下、PFN）は、研究開発の基盤技術である深層学習フレームワークを、自社開発のChainer™から、PyTorchに順次移行する発表された。https://preferred.jp/ja/news/pr20191205/


## MNIST手書き数字データの説明（5分）

* MNIST(Mixed National Institute of Standards and Technology database) 

* 直接ダウンロードすることも可能 http://yann.lecun.com/exdb/mnist/

* 手書き数字画像60,000枚と、テスト画像10,000枚、合わせて70,000枚の画像のデータセット

* 28ピクセルx28ピクセル　-> 784ピクセル (scikit-learnの手書き数字データ：8ピクセルx8ピクセル -> 64ピクセル)

* 人工知能(AI)の勉強を始める入り口としてMNISTはよく使われるデータセット

## プログラムの解説（30分）

* Chainerのインストール

* MNISTデータのダウンロード

* 数字画像を見る

* 学習用データセットと検証用データセットの数の確認

* ニューラルネットワークの定義（今回は、DeepLearningではない）

* b(バイアス)とw(重み付け)の変化を確認する

* iterators

* optimizerの設定

* 検証処理ブロック（ソースコードの修正あり）

* 学習と検証

* 学習モデルのダウンロードと利用

## 犬と猫の分類（学習済みモデルの生成のみ実施：10分）

* 参考書籍の第４章第６節

* https://github.com/Kokensha/book-ml/blob/master/Colaboratory/04_06(Chainer_dogs_and_cats).ipynb

* 犬と猫の写真データを取得する```!wget files.fast.ai/data/dogscats.zip``` 
まず、プログラムを実行して、学習済みモデルを取得するまでやります。時間があったら、内容を説明する

* 画像データ形式の整備

* 画像の前処理

* データセットの作成

* 学習データと検証データを分ける

* CNN設定(畳み込みニューラルネットワークの学習については次回詳説する)

* 反復子

* optimizerの設定

* updaterの設定

* extensionsの設定

* 学習及び学習結果の確認

* 検証

* 学習済みモデルの取得（Google Driveに保存する）

* 手書き犬と猫の判別（ウェブアプリ）

* 写真をアップロードして認識させる


## Dockerを使ったFlaskウェブアプリの起動方法（30分）

* https://github.com/Kokensha/book-ml/tree/master/docker-python3-flask-ml-app

* 画像データの送信

* サーバサイド画像データの受け取り

* データの処理

* 学習済みモデルを使って推論

# 質疑応用（10分）

# [今後の予定](handson_plan.md)

# アンケート回収

# スタッフ片付け、解散
