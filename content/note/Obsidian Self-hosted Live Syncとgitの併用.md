---
title: "Obsidian Self-hosted Live Syncとgitの併用"
created: "2023-06-13 01:04"
slug: 2023-06-13-01-04
tags:
- post
- note
---

GitHub Pagesで公開しているのでこれをLive Syncをうまく組み合わせたい
なので設定した方法をメモする

## Live Syncの設定

hidden fileは同期しない
設定はCustomization Syncでやる
他はデフォルト

## Gitの設定

当然.gitディレクトリは同期されないのでこれは別に取ってくる
なぜしないのかというとこれもLive SyncされるとGitがうまく動かなかったため、除外

obsidian gitでremoteを設定してpullでもいいが、大きいrepositoryだとpullする時にエラーが出た
なので、[Working Copy](https://apps.apple.com/app/id896694807)なんかを使ってCloneしてから、ファイルアプリにて.gitディレクトリを移動させる

これで完了