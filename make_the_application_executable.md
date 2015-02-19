# Make the application executable

この章で、これまで作成してきたコードをWebアプリケーションとして実行可能にします。

### ここで説明すべきこと(wip)
- Javaで作られたWebアプリケーションは、伝統的にWARファイルという形式にする。
- Springではより簡単なアプローチとして、実行可能なJARファイル(executable JAR file)というアプローチを取ることができる。
    - これはjavaではおなじみの`main()`メソッドから実行可能ということ。
    - 内臓Tomcatがあるので、動作させるために他に環境が必要ない。
- runメソッドにApplication.classを渡す意味。
- @ComponentScanアノテーションと@Componentアノテーション(これは多少文章読めでいいかも？バランス難しそう)
- @EnableAutoConfigrationアノテーションで面倒な設定は省略できる(web.xmlいらない！さよならXML地獄)

## Build an executable JAR

JARファイルの作成を行い、`java -jar`コマンドでWebアプリケーションを実行してみましょう。
