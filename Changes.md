## 変更点

### 2019.12.16
* **Single Window Desktop App for Mac**
    * 初期設定に関するコードが分散していたのをPreferencesモジュールにまとめた。
### 2019.12.14
* **Single Window Desktop App for Mac**
* **Droplet**
    * アプリ終了時のクラッシュ予防でApp.terminateを使っていたが、App.Close以外ではQuitでするようにした。QuitにしないとApp.CancelCloseイベントが発動しないからです。
### 2019.12.13
* Xojo 2019r3で「Supports Dark Mode」をONにして保存し直した。
* **Single Window Desktop App for Mac**
    * **myListBox**
        * ダークモードに対応。（ダークモード非対応のXojoバージョンでもエラーにならないので大丈夫）
### 2019.8.10
* **Single Window Desktop App for Mac**
    * **myTextArea**
        * 「SetSystemFont」メソッド追加。
        * 「SetFontWithName」メソッド追加。
        * 「SetFontPanelMenu」メソッド追加。
        * 「LayoutOrientation」プロパティ追加。
### 2019.8.3
* **Single Window Desktop App for Mac**
    * BringFrontmostMeメソッドを改善。
    * SetProxyIconメソッドを改善。
* **Multi Window Desktop App for Mac**
    * ウインドウメニューの記号が不正確になる不具合を修正。
    * SetProxyIconメソッドを改善。

### 2019.8.2
* **Single Window Desktop App for Mac**
    * Generalモジュールにメソッド「BringFrontmost」「BringFrontmostMe」を追加。
    * Window1にSetProxyIconメソッドを追加。
* **Multi Window Desktop App for Mac**
    * Window1にSetProxyIconメソッドを追加。

### 2019.8.1
* **Single Window Desktop App for Mac**
* **Droplet**
    * Quit時のクラッシュをさらに防ぐため、QuitをすべてNSApplicationのterminateを使用するようにした。

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