# 03 機械学習（machine learning）　

機械学習とは！

機械学習は人間が明示的にプログラミングせずに、コンピュタがデータから学習できるためのプログラミングの手法です。

## 学習データについて

<img src="assets/03-01-data.png" alt="データセットの分け方" width="400">

## 学習の種類

### 主に三種類

<img src="assets/03-3_types_ml.png" alt="データセットの分け方" width="400">

### 教師あり学習(supervised learning)

<img src="assets/03-supervised_learning.png" alt="教師あり学習" width="400">

フォルダの名称が「正解教師ラベル」になる場合もあります。

<img src="assets/03-supervised_learning_folder_label.png" alt="教師あり学習" width="600">

教師あり学習が向いているタスク

#### 分類(classification)

* 決定木(decision tree)

* ランダムフォレスト(random forest)

* SVM(support vector machine) 

  - 超平面（hyper plane）
  <img src="assets/03-hyper_plane.jpg" alt="hyper plane" width="800">

* k-平均法（k-means）

もっともよく知られているクラスタリングアルゴリズムの１つです。

* [ニューラルネットワーク](https://github.com/Kokensha/machine_learning_deep_learning_lessons/blob/master/04_artificial_neural_network.md)


#### 回帰(regression)

* ロジスティック回帰

* k-近傍法（k-nearest neighbor algorithm, k-NN）

* ランダムフォレスト回帰(random forest)

* SVM回帰

* [ニューラルネットワーク](https://github.com/Kokensha/machine_learning_deep_learning_lessons/blob/master/04_artificial_neural_network.md)


### 教師なし学習(unsupervised learning)

教師なし学習が向いているタスク

#### クラスタリング(clustering)

* k-平均法（k-means）

もっともよく知られているクラスタリングアルゴリズムの１つです。

#### 相関ルール学習

#### 異常検知

#### 次元削減

* PCA

  - <img src="assets/03-pca.jpg" alt="PCA" width="800">


### 強化学習

## scikit-learn

* [scikit-learn url](https://scikit-learn.org/stable/)

* scikit-learnの実戦
