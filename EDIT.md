# 作業の進め方

## はじめに
- Gitの基本的な知識を有している人が想定読者です。
- どんなGitクライアントを利用しても構いませんが、コマンドラインクライアントの操作例を記述します。

## 流れ

### Clone
[リポジトリ](https://github.com/MakiNish/GitBook_for_Spring)をローカルにクローンします。
```
$ git clone https://github.com/MakiNish/GitBook_for_Spring.git
```

### Branch
クローンしたリポジトリ上に作業ブランチを作成します。
```
$ git checkout -b {branch_name}
```
> __Note:__ 上のコマンドは元のブランチ(cloneしたときはマスターブランチにいるはず)から、新しいブランチを作成しつつ切り替えています。`{branch_name}`には適当な名前を入れてください。

### ファイル編集
[What you'll buildの例](https://github.com/MakiNish/GitBook_for_Spring/blob/master/what_youll_build.md)を参考にファイルを作成します。


### Commit & Push
普通にCommit・Pushします。

```
$ git add {filename}
$ git commit -m {commit message}
$ git push
```

### Pull Request(作成)
[プルリクエストページ](https://github.com/MakiNish/GitBook_for_Spring/pulls)からプルリクエストが作成できます。

ブランチの選択の画面で、
- base: master
- compare: {your branch}

にして、"Create Pull Request"です。

### Pull Request(マージ)
プルリクエストが作成されたら本田がレビューします。その後本田がマージを行い、Gitbookにも自動的に反映されます。

もちろん、他のメンバーのプルリクエストを見て気付いたことなどなにかありましたら言っていただけるといいと思います。
