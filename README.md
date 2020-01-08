# AI トレーニング

AI トレーニングのお題

# 自由に触れるLinux環境を手に入れよう

なにはともあれ、AIのフレームワークを触るには、自由に触れるLinux環境が必要。  
ということで、以下 いずれかの方法で、自由に触れるLinux環境を作成しましょう。

* 初心者向け VirtualBox
  - 自身のWindowsPCにVirtualBoxをインストールし、Linuxを立ち上げる
  - 自身のWindowsPCのSpecに依存するので、あまり早くはない・・・
  - 参考サイト
    - [【2018最新】VirtualBoxでUbuntu18.04の導入から設定まで詳しく解説](https://www.sejuku.net/blog/82291)

* 中級者向け AWS EC2インスタンス
  - 1年間はどんなに使っても無料。1年過ぎても小さいサイズならずっと無料
  - 無料期間なら高スペックなLinuxが手に入る
  - Proxyに悩まされずに済む
  - クレジットカード情報が必要
  - 無料期間終了が近くなったら、作ったEC2インスタンスを消しておいたほうが無難
  - 参考サイト
    - [AWSにEC2インスタンスを立ち上げよう](https://hacknote.jp/archives/41967/)
        - AWS初心者の方に向け、AWSアカウントの取得とWebサーバーとなるEC2インスタンスの立ち上げまでを紹介します
    - [AWSのサーバーにログインしてみよう](https://hacknote.jp/archives/42191/)
    - [AWSの無料アカウントを作成する(Amazon Web Services)](https://www.ritolab.com/entry/9)

* ？級者向け WSL
  - VMよりは断然軽い。ただし、完全Linuxではないので 動かないアプリケーションもあるかもしれない
  - Linuxさえ入ってしまえば、TensorFlowやPytorchのinstall方法は、以下と同じ
  - 参考サイト
    - [【WSL入門】第1回　Windows 10標準Linux環境WSLを始めよう](https://www.atmarkit.co.jp/ait/articles/1903/18/news031.html)
    - [Windows 10でLinuxを使う](https://qiita.com/whim0321/items/093fd3bb2dd287a72fba)


# AI フレームワークの Hellow world

TensorFlowやPytorchをインストールし、Hellow world/MNISTをやってみよう

* Tensorflow
  - 参考サイト
    - [TensorFlow (CPU Only) インストール](https://www.server-world.info/query?os=Ubuntu_18.04&p=tensorflow&f=1)
    - [Proxy下でTensorFlowのMNIST](https://qiita.com/Knoth/items/822dab08681e7fe1c47e)
    - [pythonでbasic認証付きのhttpプロキシを経由する時のハマりポイント](https://qiita.com/arc279/items/f44ab151c59d152056dc)

* Pytorch
  - 参考サイト
    - [Ubuntu 18.04にPyTorch 1.0をインストールし、MNISTの手書き分類を実行する](https://symfoware.blog.fc2.com/blog-entry-2344.html)
    - 上記 GPUは使わないので、cudaは入れない
    - Proxyの話も解決する必要あり
    - [この辺参照](https://github.com/pytorch/vision/issues/1033)

* Proxyの話
  - pipやapt-getのproxyは、以下の方法1で、だいたい解決できる
  - (pytorchやtensorflowのmnistデータdownloadは、環境変数だけでは解決できないので、上に上げプログラム対処が必要)
  - [環境変数を設定する](https://qiita.com/firstVersion/items/2fa8f86a5b77d688dc1a#%E6%96%B9%E6%B3%951%E7%92%B0%E5%A2%83%E5%A4%89%E6%95%B0%E3%82%92%E8%A8%AD%E5%AE%9A%E3%81%99%E3%82%8B)


# おまけ 読み物

[学習済みの様々なディープラーニング・モデルをメチャ簡単に利用できる！ Model Asset Exchange(MAX)をご紹介します](https://qiita.com/ishida330/items/6e66323dfd56205fbe80)  
上記記事を読んでおいてください.  
AIフレームワークの登場で、機械学習が使いやすくなり、さらに学習済みのモデルの再利用までできるようになりましたが、  
やっぱり、まだまだ敷居が高いです．そのため、上記記事にあるようなものが出てきています。  
  
この記事を読むと、AIや機械学習でどんなことができるか？というのが掴めると思います。


