# 応用数学
## 情報量
### エントロピー
あるできごと（事象）が起きた際, それがどれほど起こりにくいかを表す尺度である。
あくまでそのできごとの起こりにくさ（確率）だけによって決まる数学的な量でしかなく, 個人・社会における有用性とは無関係である。
事象Eが起こる確率をP(E)とするとき, 事象Eが起こったことを知らされたとき受け取る（選択）情報量I(E) を
```
I(E) = log(1 / P(E)) = -logP(E)
```
たいてい, 対数の底は2で、自然対数であることが多い.

### シャノンエントロピー
シャノンエントロピーとはエントロピーの期待値であり, 加重平均である.
シャノンエントロピーとは`P(E) * I(E)`の総和である.

### KLダイバージェンス
 [生成モデルで語られる Kullback-Leibler を理解する](https://qiita.com/TomokIshii/items/b9a11c19bd5c36ad0287)
 
確率分布の差異を表す事から、カルバック・ライブラー距離 と呼ばれる事もあるが、距離の公理を満たさないので、数学的な意味での距離ではない。
具体的に言うと, *非負性*は満たすものの, *対称性*`KL(P(x)|Q(x)) = KL(Q(x)|P(x))`は満たさない.

確率分布がほとんど同じところで一致する場合は, KLダイバージェンスの値が0に近づき, 一致しなければしないほど値が大きくなる.