# 東工大文芸部

東工大文芸部の「論理哲学論考」読書会のレジュメや参考資料を管理するためのリポジトリ

# レジュメを管理するための方法

- リポジトリをforkする

右上の fork というボタンを押してください

- forkしたリポジトリを自分のアカウントにあるリポジトリからcloneする

このリポジトリからcloneしても共同開発しているとは言えません。
なので、必ず自分のリポジトリからcloneするように。

- ローカルに落としたリポジトリにファイルを追加する

- `$ git add [filename]`

- `$ git commit -m [commit message]`

- `$ git push`

- pull request を作成

- merge されるのを待つ

# ~~makepdf.shについて~~

makepdf.sh は tex ファイルをコンパイルして pdf を生成するスクリプトです。
使い方は

```
$ sh makepdf.sh [filename]
```

でok! [filename]は拡張子なしでやるとスムーズです。

***コマンド入力でフォントを埋め込むためこのスクリプトを使ってのコンパイルは一旦中止とします。**

# フォントの埋め込み方法

OS Xの場合は
```
$ platex foo.tex
$ dvipdfmx -f hiragino.map foo.dvi
```
でフォントを埋め込むことが可能です。これにより日本語の文字化けを防止できます。
