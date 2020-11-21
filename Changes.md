## 変更点

### 2020.11.21
* **Single Window Desktop App for Mac**
	* **Extras**
        * GetSystemVersionIntがBig Sur 11.0に対応していなかったので直した。
        * myTextArea.ShowFindBarを削除。
        * myTextArea.FindSettingを追加。Openイベントで実行するようにした。
* **Multi Window Desktop App for Mac**
    * App.RefreshWindowMenuTitleを追加。
* **Single/Multi Window Desktop App for Mac**
	* **MenuBar**
        * MenuSelectAllモジュールをCocoaMenuに改名。
        * CocoaMenuItemFindAbstractクラス、CocoaMenuItemFindクラスを追加。
	* メニュバーにメニュー項目EditFindを追加。設定不要で検索バーを表示できるようになった。
	* ウインドウメニューの標準の項目もCocoaMenu仕様に変更した。

### 2020.11.20
* **Single Window Desktop App for Mac**
	* **Extras**
        * Show...系のメソッドを実行時に最前面になるようにした。
        * SystemVersionをGetSystemVersionIntに改名。
        * SystemVersionToIntを追加
        * StringExモジュールを追加した。

### 2020.11.17
* **Single Window Desktop App for Mac**
	* **Extras**
        * General.GetFrontmostAppBundleIDを追加した。
        * General.GetFrontmostAppNameを追加した。
	* AboutWindowのサイズを調整した。

### 2020.11.15
* **Single Window Desktop App for Mac**
	* **Extras**
        * UnicodeNormalizationで対象文字列が英数字1文字のときなどでエラーになっていたのを修正した。

### 2020.11.14
* **Single Window Desktop App for Mac**
	* **Extras**
        * ArrayExで配列要素数が1つ以下なら処理しないようにした。

### 2020.11.11
* **Single Window Desktop App for Mac**
	* **Extras**
        * myTextArea.SetFixedPitchFont を追加した。

### 2020.11.8
* **Single Window Desktop App for Mac**
    * **Extras**
        * モジュール「SortArray」を「ArrayEx」に改名した。
        * ArrayExにRemoveDuplicate を追加した。
        
### 2020.11.4
* **Single Window Desktop App for Mac**
    * **Extras**
        * FolderItemExモジュールを追加した。
            * FileType取得などビルトインにはないメソッド集
### 2020.11.2
* Xojo2018r2（OS X Mavericks 10.9対応の最終バージョン）に統一した
* **Single Window Desktop App for Mac**
    * **General.ShowInFinder**
        * 動作しなくなっていたので修正した。
    * **General.SystemVersion**
        * 追加した。
    * **Preferences.Raed/Preferences.SetDefault**
        * デフォルトウインドウサイズをパラメーターに加えた。
* **Droplet**
    * 「2019r1まで」「2019r2以降」のどちらでも動作する1つにまとめた。
    
### 2020.9.30
* **Single Window Desktop App for Mac**
    * **myListBox**
        * 罫線の描画を追加した。
### 2019.12.17
* **Droplet**
    * Xojo 2019r2からドロップレットの設定方法が変更になっていたので「2019r1まで」「2019r2以降」の2つに分けた。
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