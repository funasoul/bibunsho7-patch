Bibunsho7-patch/Patch.app: ［改訂第7版］LaTeX2e美文書作成入門 ヒラギノフォントパッチ
====================

「新しいmacOSへアップグレードしてから、 `(u)platex+dvipdfmx` でヒラギノフォントを埋め込めなくなって困っています :cry: 」という方向けのアプリです！

## 重要

TeX Live 2020以降、標準で `(u)platex+dvipdfmx` でタイプセットしたときに埋め込まれる日本語フォントが[原ノ味フォント](https://github.com/trueroad/HaranoAjiFonts)になりました。
TeX Live 2020以降を標準でインストールした直後から、多ウェイトで原ノ味明朝、ゴシックが利用可能になっています。


## 概要

 * [［改訂第7版］LaTeX2e美文書作成入門](http://gihyo.jp/book/2017/978-4-7741-8705-1)の付録DVD-ROM内のMac OS X用インストーラーから、
   TeX Live 2016（第1刷）またはTeX Live 2017（第2刷）をデフォルト（`/Applications/TeXLive/Library/texlive/{2016,2017}/`）でインストールした方
 * （［こ㊙こ㊙だ㊙けのナイショ話、］[M㊙cTeX](http://www.tug.org/mactex/)とそのお仲間である[B㊙sicTeX](http://www.tug.org/mactex/morepackages.html)から、
   TeX Live YYYYをデフォルト（`/usr/local/texlive/YYYY{,basic}/`）でインストールした方）

のうち、

 * 手元のMac OSバージョンをOS X 10.11 (El Capitan), macOS 10.12 (Sierra), macOS 10.13 (High Sierra), macOS 10.14 (Mojave), macOS 10.15 (Catalina), macOS 11 (Big Sur), macOS 12 (Monterey), macOS 13 (Ventura), macOS 14 (Sonoma)にアップグレードした方。
 * 上記のMac OSバージョンをアップグレード後、`(u)platex+dvipdfmx` でMac OSに同梱されているヒラギノフォントを埋め込めずに、どうすればよいか分からない方。
 * TeX Liveのディレクトリ構成に関して、全く分からない方。
 * ターミナル.appなどのコマンドライン操作が苦手な方。

上記に該当する方で、同書籍の付録DVD-ROMからインストールされるTeX Live環境を引き続き利用しつつ、
`(u)platex+dvipdfmx` でヒラギノフォントを埋め込めるようにしたい方は、本パッチをご利用になりますと、簡単に実現できます。

## 利用方法

 1. 最新版 `bibunsho7-patch-X.X-YYYYMMDD.dmg` を [Releases - munepi/bibunsho7-patch](https://github.com/munepi/bibunsho7-patch/releases) からダウンロードします。
 1. ダウンロードした `bibunsho7-patch-X.X-YYYYMMDD.dmg` をダブルクリック、もしくは、右クリックより開くをして、dmgを展開します。
 1. 展開したdmgのフォルダ内にある `Patch.app` をダブルクリック、もしくは、右クリックより開くをして実行します。

Happy TeXing!

## 同書籍のサポートページ

 * [奥村晴彦先生](http://okumuralab.org/bibun7/)
 * [技術評論社](http://gihyo.jp/book/2017/978-4-7741-8705-1/support)

## 本アプリの解説ページ

[TeX ＆ LaTeX Advent Caleandar 2017](https://adventar.org/calendars/2229)の8日目の記事として、本アプリの解説を簡単に載せました。

 * [［改訂第7版］LaTeX2e美文書作成入門 ヒラギノフォントパッチ](https://qiita.com/munepi/items/c4274da0646b3e785c7f) via [Qiita](https://qiita.com/)

なお、本ページをWebブラウザで開きますと、一見の文章量に対してWebブラウザ内のスクロールバーがやたらめったら余裕がありますので、どうかお察しください☃

## コマンドラインに慣れている方

``` shell
$ git clone --recursive https://github.com/munepi/bibunsho7-patch.git
$ cd bibunsho7-patch/

（必要に応じて、該当バージョンをcheckout： git checkout vX.Y）

$ sudo ./Patch.sh
```

なお、`Patch.app`は、本アプリの仕様上、OS X 10.10 (Yosemite)以降でしか動作しません。
一方、直接、コマンドラインから、`Patch.sh` を実行すると、OS X 10.10 (Yosemite)未満でも動作するはずです。


## キーワード

Mac OS X, macOS, TeX Live, x86_64-darwin, MacTeX, BasicTeX, LaTeX, pLaTeX, upLaTeX, dvipdfmx, ヒラギノフォント, ヒラギノ明朝, HiraMin, HiraginoSerif, ヒラギノ角ゴ, HiraKaku, HiraginoSans, ヒラギノ丸ゴ, HiraMaru, HiraginoSansR

## License

This program is licensed under the terms of the MIT License.


--------------------

Munehiro Yamamoto
https://github.com/munepi
