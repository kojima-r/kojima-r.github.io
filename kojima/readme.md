# はじめに

このフォルダは個人用サイトのテンプレートです．
サンプルを自分の情報に書き換えて、ページの内容を更新しましょう．
以下は、変更するべき場所を指示したガイダンスです．

# テンプレートの構成

このテンプレートは以下のようなファイル構成になっています．

```
├── assets
│   ├── css
│   │   ├── bootstrap.css
│   │   ├── font-awesome.min.css
│   │   └── main.css
│   ├── fonts
│   ├── img
│   │   ├── header_back.png
│   │   ├── link_icon.png
│   │   └── user.png
│   └── js
├── index.en.html
└── index.html
```

この中で書き換えるべきファイルはindex.html, index.en.htmlの2つです．

# 置き換えるべきファイル群

このテンプレートで置き換えるべきファイル群は以下の2つのファイルです．

* assets/img/user.jpg: ユーザの顔写真データです．自分のものに置き換えましょう．
写真をそのまま置くと大きすぎるので何らかのソフトでトリミング，縮小して適切なサイズに調整しましょう．
* assets/img/header_back.png: トップで使われている写真データです．自分で好きなものを作って、置き換えましょう．
写真をそのまま置くと大きすぎるので何らかのソフトでトリミング，縮小して適切なサイズに調整しましょう．

# index.htmlの書き換え

テキストエディタ（またはhtmlエディタ）で、index.htmlを開くと、編集すべき箇所に日本語でコメントしています．
それをみながら、編集していけば基本的に編集は終了します．念のため、ここでも編集するべき箇所を紹介していきます．

## サイトのタイトル

12行目付近にサイトのタイトルを指定する部分があります．好きなフレーズに書き換えましょう．

```html
	<!-- ここを自分の名前に置き換えよう -->
	<title>Ryosuke Kojima's Page</title>
	<!-- ここまで -->
```

## サイトトップの画像と文句

サイトトップにかっこいい写真を配置し、自分の好みの格言でも配置しましょう．

サイトトップの写真は前述のようにassets/img/header_back.pngを置き換えることで、格言は94行目付近を編集することでそれぞれ変更できます．

```html
	<!-- 適当に好きなフレーズに書き換えましょう。 -->
	<h2> Something is wrong with the world </h2>
	<!-- ここまで -->
```

## プロフィール

次にプロフィールの修正をしましょう．具体的には自分のプロフィールの文言と写真を修正します．

ユーザ写真の入れ替えは、前述のようにassets/img/user.jpgを入れ替えましょう．
プロフィールについては86行目付近を修正すれば大丈夫です．

```html
	<!-- 自分のプロフィールに書き換えよう -->
	<h4>小島　諒介</h4>
	<p>
		東京工業大学大学院情報理工学研究科情報環境学専攻<br/>
		中臺研究室 D2<br/>
		Email: kojima[at]cyb.mei.titech.ac.jp<br/>
	</p>
	</div>
	<div class="col-lg-4">
		<!-- assets/img/user.pngを自分の写真に置き換えよう -->
		<img class="img-circle" src="assets/img/user.jpg" height="200" width="200">
	</div>
	
```

## サイト紹介文

プロフィールの修正が終わったら、その下のサイト紹介文を修正します．これまでと同じように、99行目付近を修正します．

```html
	<!-- 自分用のメッセージに書き換えよう -->
		<h4>ようこそ</h4>
		<p>こんにちは。小島　諒介です。このページは、私のやってきたことを簡単にまとめています。
		私は東京工業大学で修士時代に人工知能・機械学習・データマイニングの研究を行っていました．
		現在は，音を中心とした環境の理解（音環境理解）に関する研究をしています．</p>
```	

## 実績

実績は、自分の論文のbibtexをbibtex_selectedというidのついているtextareaとbibtex_workというidのついているtextareaとに書くことで作ります．

```html
	<textarea id="bibtex_work" style="display:none;">
	  @misc{ wiki:ast,
	    author = "Wikipedia",
	    title = "Abstract syntax tree --- Wikipedia{,} The Free Encyclopedia",
	    year = "2010",
	    url = "\url{http://en.wikipedia.org/w/index.php?title=Abstract_syntax_tree&oldid=351440895}",
	    note = "[Online; accessed 30-March-2010]"
	  }

	  @misc{lrpdf,
	    author = "Andreas Kunert",
	    title = "LR Parser für Pragmatiker",
	    year = "2008",
	    url = "\url{http://www2.informatik.hu-berlin.de/~kunert/papers/lr-analyse/}"
	  }
	</textarea>
```

## 自分のSNSアカウントの編集

これは好みで、やってもやらなくても良いですが、自分のtwitterやfacebookアカウントにビューワを誘導したい場合は、以下のリンクを修正してください．

```html
	<!-- 自分のTwitterページのリンクに書き換えよう。（したくない場合はhrefの値を#にしましょう） -->
	<a href="https://twitter.com/onuxy">
		<i class="fa fa-twitter"></i>
	</a>
	<!-- 自分のFacebookページのリンクに書き換えよう。（したくない場合はhrefの値を#にしましょう） -->
	<a href="https://www.facebook.com/ryosuke.kojima.509">
		<i class="fa fa-facebook"></i>
	</a>

```

以上、基本的にはindex.en.htmlも同様の手順で修正していきます．index.en.htmlは英語ページですので、英語でいろいろと記述しましょう．










