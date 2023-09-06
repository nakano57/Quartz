
## ストレージ

今あるDell Optiplex 3050をつかおう。
BcacheとかそのままNASにすると

[nfsサーバを構築しKubernetesからストレージとして利用してみた - DENET 技術ブログ](https://blog.denet.co.jp/building-an-nfs-server-and-using-it-as-storage-from-kubernetes/)

[k3dで永続ボリューム(PersistentVolume)を使う - Qiita](https://qiita.com/yuta_vamdemic/items/766fd5da53e0850e4bc7)

## クラスター

k3sが軽そう

色々あっておもしろい

[k3os 高可用性（HA)インストール - Qiita](https://qiita.com/taga090/items/b43e7e0edc68db370144)

[ラズパイでK3sクラスター構築 - Sogo.dev](https://sogo.dev/posts/2023/06/k3s-setup)

慣れているUbuntu Serverで下のやり方が良さそう
とりあえずserverとagent1台づつで始めてみようかな

## Network 

NASと繋がるため、宅内LANを少なくとも5Gbpsにしたいな…高えが…
![[../attachments/IMG_3811.jpeg]]

高え

## 学び

brewやaptのようなノリでhelmがあるらしい

