## 変更点

### 2019.7.27
* **Single Window Desktop App for Mac**
    * **UnicodeNormalization**
        * 不要なエラー表示がされていたのを修正。


### 2019.7.26
* **Single Window Desktop App for Mac**
    * **Extras**
        * CodePointモジュールを追加。
            * コードポイント関連のメソッド集。
        * SortArrayモジュールを追加。
            * 配列のソート関連メソッド集。
        * Iconモジュールを追加。
            * アイコン取得関連のメソッド集。
        * Generalモジュールを追加。
            * 使用頻度が高い一般的なメソッド集。
    * **Window1**
        * AdjustPositionメソッドを追加。
            * ウインドウ位置のはみだしを調整するメソッド。
    * **Preferencesモジュールを追加**
        * 環境設定関連のメソッド集。
        * Window1の位置とサイズの読み書きを仕込んであります。
    * AboutWindowのアイコンのHi-DPI対応。
    * App.CloseにQuit時のクラッシュ防止を仕込んだ。
* **Multi Window Desktop App for Mac**
    * AboutWindowのアイコンのHi-DPI対応。
    * App.CloseにQuit時のクラッシュ防止を仕込んだ。
* **Droplet**
    * App.CloseにQuit時のクラッシュ防止を仕込んだ。


### 2019.7.21
* **Single Window Desktop App for Mac**
    * **Extras**
        * RegExXojoモジュールを追加
            * XojoのRegExクラス関連のメソッド集。
        * UnicodeNormalizationモジュールを追加
            * Unicode正規化関連のメソッド集。
    * App.EnableMenuItems を改善。
* **Multi Window Desktop App for Mac**
    * App.EnableMenuItems を改善。


### 2019.7.7
* **Single Window Desktop App for Mac**
    * **myTextArea**
        * Undo履歴を区切る「BreakUndo」メソッド追加。
        * マージンを設定できる「SetMargin」メソッド追加。
        * フォント内のlineGapを使うかどうかを設定できる「UsesFontLeading」メソッド追加。（NSLayoutManagerではデフォルトがTrue。これをFalseにできる）
        * メソッドとプロパティの名称変更
            * SelectAllSV → SolvedSelectAll
            * SelTextSV → SolvedSelText
            * TextSV → SolvedText
        * [insertText:](https://developer.apple.com/documentation/appkit/nstextview/1449174-inserttext?language=objc) がDeprecatedだったので、[insertText:replacementRange:](https://developer.apple.com/documentation/appkit/nstextinputclient/1438258-inserttext?language=objc)に変更した。