# DCGAN_mnist
Using mnist libray, Deep Convolutional GAN generates fake images

mnist画像を使って、kerasで構築したDeep Convolutional GANを試してみましたよーってリポジトリです。  
[前回のGAN](https://github.com/zashio/GAN_mnist)よりも生成画像にノイズが少ないですね。  
kerasにまだあまり慣れてない方のために、最上位モジュールのみimportする方針で書いてみました。

### Demo
- mnist画像といえば[こんな感じ](https://upload.wikimedia.org/wikipedia/commons/2/27/MnistExamples.png)ですよね。(Wikipediaより)
- 今回はDeep Convolutional GANを用いて、mnistのフェイク画像を生成しました。結果は以下のような感じです。

  - 0回学習 : まだ学習していないので、各ピクセルの出力はほとんどランダムとなっています。
![0回学習画像](https://github.com/zashio/DCGAN_mnist/blob/master/savefig/0.png)

  - 1000回学習 : もうずいぶんと数字ですね。[前回のGAN](https://github.com/zashio/GAN_mnist)よりも学習が早いですね。
![1000回学習画像](https://github.com/zashio/DCGAN_mnist/blob/master/savefig/1000.png)

  - 3000回学習
![3000回学習画像](https://github.com/zashio/DCGAN_mnist/blob/master/savefig/3000.png)

  - 5000回学習
![5000回学習画像](https://github.com/zashio/DCGAN_mnist/blob/master/savefig/5000.png)

  - 15000回学習 : だいたいこの辺りが限界ってところでしょうか。
![15000回学習画像](https://github.com/zashio/DCGAN_mnist/blob/master/savefig/15000.png)

- 以上のような感じで、いい感じに学習できたと思います。
- [前回のGAN](https://github.com/zashio/GAN_mnist)に見られたような砂っぽいノイズがほとんどないですね。成功してます。

### Usage
- [Google Colabratory](https://colab.research.google.com/)で、GITHUB上のNotebookを開けるので、zashioのGAN_mnist.ipynbを指定してください。
- 開いたら、上のセルから順に、 Shift + Enter で実行していけば、学習がスタートします。

### Contribution
- ガンガンにフォークして試していってください。
- どんな魔改造もお待ちしております。

### License
This source is licensed under the Apache License, Version2.0

### Author
zashio
