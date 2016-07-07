# HTML5


## 事前にインストール
- SublimeTextとGoogleChromeのインストールを事前に必ずお願いいたします。

[SublimeText](http://www.sublimetext.com/3)
[GoogleChrome](https://support.google.com/chrome/answer/95346?hl=ja)


#学習を始める前に
世の中には数えきれないほどのWebページがあります。
Webページは「Google Chrome」「Firefox」「Safari」といったブラウザから閲覧することができます。
そして、そういったWebページは、ほぼ全て、「HTML」「CSS」で作成されています。
必要に応じて「JavaScript」や「PHP」などといったプログラミング言語も使用しますが、
「HTML」「CSS」は、Webページを作成する際に「必ず」使用する共通技術となります。


#HTMLとは
Hyper Text Markup Language(ハイパーテキスト・マークアップ・ランゲージ)の略



* 文章に意味づけをして、文書構造を作る、Webサイト用の文書を書くための言語。
* HTMLで作るものはあくまで「文書」で、 見出し`<h1>`や、段落`<p>`などでできている。
* 現在、皆さんが目にするインターネット上で公開されてるウェブページのほとんどは、HTMLで作成されています。
* HTMLはそれほど難しい言語ではありません。簡単なウェブページなら、数種類のタグで作成することが可能。

* HTMLの記述は小文字をおすすめします。

<!--
 (1つ前のバージョンのXHTMLでは、要素名と属性名はすべて小文字で記述しなければならないので、HTMLの要素・属性はすべて小文字で記述しておくほうが良いでしょう。)
-->


<!--


Sublime textを使ってこの様に記述すると
![スクリーンショット 2015-07-01 13.27.31.png](https://qiita-image-store.s3.amazonaws.com/0/67977/d77aa138-275b-d60d-d864-f7bc6e4522ed.png "スクリーンショット 2015-07-01 13.27.31.png")

<br>
下記の様にデバイスに表示される
![スクリーンショット 2015-07-01 13.26.21.png](https://qiita-image-store.s3.amazonaws.com/0/67977/afda38d4-b77d-3155-c317-725d3e5f13b6.png "スクリーンショット 2015-07-01 13.26.21.png")

-->











<br>
<br>



#HTMLの記述の仕方

```html:HTML
<!DOCTYPE html> <!--DOCTYPE宣言,HTMLのバージョンを宣言するためのもの-->

<html lang="ja"><!--言語の指定-->

<head><!--ページに表示されない情報(Webページの設定に関する情報)-->

    <meta charset="utf-8"><!--HTML5での文字コードはUTF-8が推奨(文字化け対策)-->
    <title></title><!--ブラウザのタブ上のページのタイトルを指定-->

</head>

<body><!--ページに実際に表示される内容-->

    <h1>HTMLを学習しよう！</h1>
    <p>HTMLはタグで囲むのが基本です</p>

</body>

</html>
```




***HTMLはタグで囲むのが基本です***
ウェブページ内の各部分をどのような要素に割り当てるかによって、タグの種類を使い分けます。


![html_入れ子構造.jpg](https://qiita-image-store.s3.amazonaws.com/0/67977/5bdc8848-8109-dddc-c30f-44f6bbc9b566.jpeg "html_入れ子構造.jpg")

<開始タグ>～</終了タグ>が基本の書き方です。
タグは入れ子の構造になることにご注目ください。複雑な文書になっても、基本の構造は変わりません。

<br>


<!--
- 形ですが、 HTML5(１番新しいバージョン)から`<p>`タグや`<li>`タグなど、HTMLタグの一部には終了タグを省略しても良いとされているものもあります。
- HTML5の前のXHTMLは現在も色んな場面で使われています。XHTMLでは終了タグが必要なものもあるので、基本は全てに終了タグをつけるようにしましょう！
-->


> <開始タグA>
> 　　<開始タグB>ここに内容</終了タグB>
> 　　<開始タグC><開始タグD>ここに内容</終了タグD></終了タグC>
> </終了タグA>


```html:例
<p>pタグは<strong>段落</strong>です</p>
```


![Untitled 16.55.24.png](https://qiita-image-store.s3.amazonaws.com/0/67977/777236fd-e688-8e00-ef5a-2e885c53a65d.png "Untitled 16.55.24.png")　　　　　　　　　![Untitled 16.58.44.png](https://qiita-image-store.s3.amazonaws.com/0/67977/2c11c4c6-67ff-e4ce-5397-1693f1b51347.png "Untitled 16.58.44.png")




<br>
<br>



#HTMLファイルの作成

１, SublimeTextを開く
２, 右下のPlain TextをクリックしHTMLを選択
　 (この時、Plain Text右のTab Sizeを4にしておくと良い)
３, ナビゲーションバーのFileから「Save」又は「command + s」(WinはCtrl + s)
４,ファイルの拡張子は「.html」(デスクトップ(保存場所はどこでもOK)に、新しいフォルダを作成しそちらに保存)




<br>
<br>
<br>



##要素内容を持たない空要素

* HTMLの中には、`<br>`(改行)や`<img>`(imageタグ)のように、要素内容を持たない空要素があります。 <br>このような空要素には終了タグはありません。



<br>
<br>




##属性を指定する

* HTMLでは、それぞれタグの種類ごとに指定できる属性の名称とその値が定義されています。

 （例)　　 `<a href="(url)">〜</a>`
　　　　　　a = anchor（アンカー）の略
　　　　　　href属性は、ハイパーリンク先のURLを指定する際に使用
　　　　　　
 （ダメな例）`<a href="(◯◯.jpg)"></a>`



<br>
<br>

##コメントアウト

<!-- -->で囲まれた部分はブラウザには表示されません

![スクリーンショット 2016-02-23 12.35.27.png](https://qiita-image-store.s3.amazonaws.com/0/67977/daa81532-084e-8356-abf3-ca8419706c71.png "スクリーンショット 2016-02-23 12.35.27.png")　　　　　　　


<br>




##デフォルトHTML

- ファイルの拡張子は「.html」


```html:HTML
<!DOCTYPE html><!--DOCTYPE宣言,HTMLのバージョンを宣言するためのもの。ここではHTML5-->
<html lang="ja"><!--言語の指定-->

<head><!--ページに表示されない内容(hp作成に関する情報)-->

    <meta charset="utf-8"><!--HTML5での文字コードはUTF-8が推奨(文字化け対策)-->

    <title>NOWALL</title><!--タブに表示されるタイトル-->

    <link rel="stylesheet" href="style.css"><!--cssの読み込み-->

</head>


<body><!--ページに実際に表示される内容-->



</body>

</html>

```




<br>
<hr>
<br>

実際にHTMLをかいてみよう！

```html:index.html
<!DOCTYPE html><!--DOCTYPE宣言,HTMLのバージョンを宣言するためのもの。ここではHTML5-->
<html lang="ja"><!--言語の指定-->

<head><!--ページに表示されない内容(hp作成に関する情報)-->

    <meta charset="utf-8"><!--HTML5での文字コードはUTF-8が推奨(文字化け対策)-->

    <title>NOWALL</title><!--タブに表示されるタイトル-->

</head>


<body><!--ページに実際に表示される内容-->

    <h1>HTML/CSSを学習しよう</h1>
    <h5>ELITES CAMP GW編</h5>
    <p>HTML/CSSを使用すると、１からホームページの作成ができます。</p>

</body>

</html>
```