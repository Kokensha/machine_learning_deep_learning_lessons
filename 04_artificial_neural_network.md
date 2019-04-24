# 04 人工ニューラルネットワーク

## 生物ニューロンからパーセプトロン

[人工知能の歴史のところを参照](https://github.com/Kokensha/machine_learning_deep_learning_lessons/blob/master/01_ai_history.md)

### 生物ニューロン（脳神経細胞・シナプス）　→　生物ニューラルネットワーク（動物や人間の神経ネットワーク、脳）

### 人工ニューロン

### 形式ニューロン

### パーセプトロン 

* ローゼンブラット（RosenBlatt）がパーセプトロンを発表、パーセプトロンは形式ニューロンの実装

### 単層パーセプトロン 

線形分離可能な問題に限られています。 ->多層パーセプトロン

## 多層パーセプトロン（MLP:Multi-layer Perceptron）

* 多層フィードフォーワード人口ニューラルネットワーク（feed forward neural network）ともいう

* 注意：フィードフォーワード人口ニューラルネットワークは、人口ニューラルネットワークのアーキテクチャの話で、層がループせず、次の層へ入力するになる子どです。MLPがそれの典型です。フィードフォーワード人口ニューラルネットワークと対照的なのは、RNNのような、順伝播ではないアーキテクチャです。

* フォーワードプロパーゲーション（forward propagation）の話と混同しないで

### 入力層（input layer）

* 入力層と隠れ層が完全結合

### 隠れ層（hidden layer）

* 隠れ層が１つ以上存在する場合をディープ人口ニューラルネットワークと呼ばれることもある

* 隠れ層と出力層が完全結合

### 出力層（output layer）

## 人工ニューラルネットワーク

* 単層人工ニューラルネットワーク

* 多層人工ニューラルネットワーク

## 人工ニューラルネットワークの構造

### 線形変換

### 非線型変換

### 活性化関数（activation function）

* どうして非線型である必要があるのか？

* 層（layer）ごとに活性化関数を固定するのが一般的

#### 活性化関数種類

* シグモイド関数(sigmoid)

* ReLu（Rectified Linear function:正規化線形関数）

### 損失関数（loss function）/目的関数、コスト関数（cost function）

* 人工ニューラルネットワークの学習で、微分可能な関数なんでも良い

* 決めるもの

#### 損失関数の種類

* 損失関数の場所は？　→　人口ニューラルネットワークの出力層で

* 交差エントロピー誤差(cross entropy error)：回帰問題によく利用される

* 交差エントロピーはどこから来たか？ →　エントロピー　→　交差エントロピー

* 二乗和誤差(mean square error)：分類問題によく利用される

## 人工ニューラルネットワークの学習（損失関数の話）

* 解析的に解く　→　解析解、数値的に解く→数値解

* 損失関数を最小化　→　損失関数のパラメータの微分（勾配）

### ミニバッチ学習

上の交差エントロピーを例にして、データを一個ずつ学習するのが効率がよくない、例えばデータを100個ずつバッチにして、全体の近似として学習する

### 1 エポック（epoch） 学習

* 10000個のデータがあるとする、1ミニバッチに100個のデータがあるとする、学習回数は100回で、全てのデータを使い切ったことになる。100回＝1エポック

### 勾配法

* 微分、偏微分、勾配、勾配法、勾配降下法、勾配上昇法

* 勾配降下法 (GD:Gradient Descent)がある、あとで詳説

* 勾配降下法の課題：谷での振動、プラトー（Plateau：高原）での停止、絶壁での反射

* 学習率（学習係数）:learning rate 一回の学習で、どのだけパラメータを更新すべきか（更新量）を決める

### 誤差逆伝播法（一般的に使われている）

* 損失関数の数値微分の計算は時間がかかる

* （微分するより）損失関数の勾配を計算する良い方法

####  微分の連鎖率（チェインルール）

* 合成関数に関する微分の法則

### 最適化 (optimization)

勾配の計算ができたら、次はそれぞれのパラメータを更新する作戦を考える

* 勾配効果法（GD）

* 確率勾配降下法 (SDG:Stochastic Gradient Descent) 

* モーメンタム（momentum）振動を防ぐ

* ネステロフの加速勾配法（Nestrov's accelerated gradient method）

* AdaGrad

* RMSProp(ヒントンの講義)

* AdaDelta

* Adam

* 自然勾配法

#### 各フレームワークのOptimizer

* (Google)TensorFlow 2 : https://www.tensorflow.org/versions/r2.0/api_docs/python/tf/optimizers

* (Preffered Networks)Chainer : https://docs.chainer.org/en/stable/reference/optimizers.html

* (Facebook)PyTorch : https://pytorch.org/docs/stable/optim.html

* (Microsoft)CNTK : https://cntk.ai/pythondocs/cntk.learners.html
