---
title: "Obsidianとquartzで日記兼ノートまとめページをGithub Pagesに作った話"
created: 2023-04-11 21:52
tags:
- post
- notes
- howto
---

## 要はこのサイトの作り方

といっても[jackyzha0/quartz: 🌱 host your own second brain and digital garden for free](https://github.com/jackyzha0/quartz) をUse Templateしたら大体完成する。

なぜQuartzにしたのかというと他のやつだとWiki感が出過ぎてしまうから、ちょっと日記寄りにしたかった。あと後述のattachmentsとかの設定でうまくいかなかった

`config.toml`やら`data/config.yaml`をいじくり回す。まだまだ知らない機能しかない

ObsidianでVaultとして開くときはリポジトリのルートフォルダにする。
![[../attachments/スクリーンショット 2023-04-11 22.03.51.png]]
つまりこう、そうしないとなんかうまくいかなかった気がする

### Obsidianの設定

Link fomatの設定は「Relative to file」にするとうまくいく

Default location for new notesも「In the folder specified below」で`content/notes`にしている

Attachmentも同様、「Default location for new attachments」は「In the folder specified below」で`content/attachments

入れたプラグインはObsidian GitとTemplater、テンプレートは[quartz/content/templates at hugo · nakano57/quartz](https://github.com/nakano57/quartz/tree/hugo/content/templates) こんな感じ。

Daily noteも場所が`content/daily`だったりするだけで大体同じ

あと[iOSショートカットを使ってWebページのURLをMarkdownでコピーする｜Kenta Nakai / UROURO｜note](https://note.com/urouro_net/n/n5ddba05aff45) とかMacでも似たようなものを入れるととても捗る。

[Markdown形式でWebサイトのタイトルやURLをコピーできるSafari機能拡張「URL Linker (旧Markdown Linker)」がコピー形式のカスタマイズに対応。](https://applech2.com/archives/20210907-url-linker-for-safari-now-available.html) これはMacのSafariで使っている。TwitterにShareするときのスタイルでCopyとかもできて便利。
