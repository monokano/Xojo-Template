[変更点](./Changes.md)

# Xojoテンプレート

[Xojo](https://www.xojo.com/)は統合開発環境のひとつで、同一のソースでクロスプラットフォーム開発ができることを売りにしています。そのため新規作成で用意されているのは、各プラットフォームで共通している項目に限られています。そんな中でmacOS専用のデスクトップアプリを作ろうとすると、ちょっと歯がゆい思いをしてしまいます。

ここにあるテンプレートは、macOSのデスクトップアプリならここから始めるのが早いだろうと考えたものです。macOSアプリとして最低限の仕込みをしてあります。

Xojoの「Project Templates」フォルダに入れておくとよいでしょう。


## テンプレートの説明

### Template-JP

#### Single Window Desktop App for Mac
* ウインドウがひとつだけのデスクトップアプリです。
* デフォルトの言語は英語。メニュー項目を日本語ローカライズしています。
* メニューバーにMacアプリとして最小限の仕込みをしています。
    * TeztArea等の文字編集でUndo/Redoができます。
    * Xojo製Macアプリには、TextArea等でサロゲートペア文字が混在していると「編集 > すべて選択 ⌘A」ですべて選択されない厄介な不具合があります。これを回避する仕込みがされているので安心です。
* ちょっとした仕込みをしてあるTextAreaとListBoxのカスタムクラスのおまけ付き。


#### Multi Window Desktop App for Mac
* 複数の新規ウインドウを作れるデスクトップアプリです。
* 複数ウインドウ対応以外はSingleと同じです。
* こちらにカスタムクラスのおまけは付いていません。

#### Droplet
* アプリアイコンにドロップして実行するドロップレットです。
* ドロップされると、AppクラスのOpenDocumentイベントで処理をして、完了したら終了します。
* 複数のアイテムがドロップされても、ひとつずつ処理をして、一通り処理が完了したら終了します。
* macOSだけでなく、クロスプラットフォームで使えると思います。たぶん。


## ライセンス

 [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).
