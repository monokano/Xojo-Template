## 変更点

### 2022.12.13
* **Single**
	* **Extras**
        * myListBoxのFinderソートが機能していなかった不具合を修正した。
        
### 2022.12.8
* **Single**
	* **Extras**
        * API2のmyListBoxのヘッダの色を白にする処理を改善。
        
### 2022.12.6
* **Single**
	* **Extras**
        * myListBoxの不具合を修正。API2のmyListBoxのヘッダの色を白にした。
        
### 2022.11.23
* **Single**
	* **Extras**
        * myListBoxの行の色を修正した。

### 2022.9.21
* API2用を追加。
* **Single/Multi**
	* ウインドウメニューにドキュメントウインドウのメニュー項目を自動生成するようにした。

### 2022.6.26
* **Drop to Window**
    * 古いSingleベースだったのを修正した。
    
### 2022.6.14
* **Single/Drop to Window**
    * ShowInFinder メソッドを修正した。

### 2022.6.11
* **Single**
    * myListboxクラスで行に横腺を描画していたのを廃止した。
* **Single/Multi**
	* WindowEX.DisableAutoTabbing を追加した。

### 2022.6.10
* **Single/Multi**
	* Window1.AdjustPosition を削除し、WindowEXモジュールを追加した。
	* WindowEX.AdjustWindow で、ウインドウの位置とサイズの調整をマルチディスプレイ対応にした。
* **Drop to Window**
	* Sample-JP > Drop to Window を追加した。

### 2022.5.20
* **Droplet**
	* 廃止。macOS 10.12以降のセキュリティ強化の影響で使用に難があるため。
* **Single/Multi**
	* IDE Scriptで使用しているコマンド「CurrentBuildAppName」の仕様がXojo 2022r1で変更されたので対策した。

### 2021.9.17
* **Droplet**
	* フォルダーもドロップできるようにした。

### 2021.5.28
* **Single**
	* Window1.AdjustPosition をブラッシュアップした。

### 2020.12.23
* **Single**
    * Window.CloseでQuitするのをやめて、App.AutoQuitにした。

### 2020.12.15
* **Single**
	* **Extras**
        * ArrayEx.IndexOf を追加した。

### 2020.12.10
* **Single**
	* **Preferences**
        * Prefs.GetArrayInteger／Prefs.GetArrayString／Prefs.GetArrayVariant／Prefs.GetDictionary を追加した。

### 2020.12.5
* **Single**
	* 初期設定周りを見直した。

### 2020.12.4
* **Single**
	* General.ShowAlertYesNo を追加した。
	* Window1.AdjustPosition にサイズ調整も加えた。
	* Prefs.SetArrayInteger／Prefs.GetArrayInteger を追加した。
* **Multi**
	* App.FrontmostWindow1 を追加した。
	* App.GetAllWindow1 を追加した。
	* Window1.AdjustPosition を追加した。

### 2020.11.21
* **Single**
	* **Extras**
        * myTextArea.SolvedTextに不具合があったので防止策を施した。
	* **Preferences**
        * Prefs.Hasを追加した。

### 2020.11.22
* **Droplet/Single/Multi**
	* AboutWindowクラスを削除し、macOS標準のorderFrontStandardAboutPanelを使用。
	* ビルド時にScriptでInfo.plistのCFBundleVersionをBuild Versionのみに書き換えるようにした。
	* ビルド時にScriptでInfo.plistにAppleEventsUsageDescriptionを追加するようにした。
* **Single**
	* Info.plistの同梱を廃止。
* **Droplet**
	* Timerを使っているメリットを生かすように処理の流れを変えた。

### 2020.11.21
* **Single**
	* **Extras**
        * GetSystemVersionIntがBig Sur 11.0に対応していなかったので直した。
        * myTextArea.ShowFindBarを削除。
        * myTextArea.FindSettingを追加。Openイベントで実行するようにした。
* **Multi**
    * App.RefreshWindowMenuTitleを追加。
* **Single/Multi**
	* **MenuBar**
        * MenuSelectAllモジュールをCocoaMenuに改名。
        * CocoaMenuItemFindAbstractクラス、CocoaMenuItemFindクラスを追加。
	* メニュバーにメニュー項目EditFindを追加。設定不要で検索バーを表示できるようになった。
	* ウインドウメニューの標準の項目もCocoaMenu仕様に変更した。

### 2020.11.20
* **Single**
	* **Extras**
        * Show...系のメソッドを実行時に最前面になるようにした。
        * SystemVersionをGetSystemVersionIntに改名。
        * SystemVersionToIntを追加
        * StringExモジュールを追加した。

### 2020.11.17
* **Single**
	* **Extras**
        * General.GetFrontmostAppBundleIDを追加した。
        * General.GetFrontmostAppNameを追加した。
	* AboutWindowのサイズを調整した。

### 2020.11.15
* **Single**
	* **Extras**
        * UnicodeNormalizationで対象文字列が英数字1文字のときなどでエラーになっていたのを修正した。

### 2020.11.14
* **Single**
	* **Extras**
        * ArrayExで配列要素数が1つ以下なら処理しないようにした。

### 2020.11.11
* **Single**
	* **Extras**
        * myTextArea.SetFixedPitchFont を追加した。

### 2020.11.8
* **Single**
    * **Extras**
        * モジュール「SortArray」を「ArrayEx」に改名した。
        * ArrayExにRemoveDuplicate を追加した。
        
### 2020.11.4
* **Single**
    * **Extras**
        * FolderItemExモジュールを追加した。
            * FileType取得などビルトインにはないメソッド集

### 2020.11.2
* Xojo2018r2（OS X Mavericks 10.9対応の最終バージョン）に統一した
* **Single**
    * **General.ShowInFinder**
        * 動作しなくなっていたので修正した。
    * **General.SystemVersion**
        * 追加した。
    * **Preferences.Raed/Preferences.SetDefault**
        * デフォルトウインドウサイズをパラメーターに加えた。
* **Droplet**
    * 「2019r1まで」「2019r2以降」のどちらでも動作する1つにまとめた。
    
### 2020.9.30
* **Single**
    * **myListBox**
        * 罫線の描画を追加した。

### 2019.12.17
* **Droplet**
    * Xojo 2019r2からドロップレットの設定方法が変更になっていたので「2019r1まで」「2019r2以降」の2つに分けた。

### 2019.12.16
* **Single**
    * 初期設定に関するコードが分散していたのをPreferencesモジュールにまとめた。

### 2019.12.14
* **Single**
* **Droplet**
    * アプリ終了時のクラッシュ予防でApp.terminateを使っていたが、App.Close以外ではQuitでするようにした。QuitにしないとApp.CancelCloseイベントが発動しないからです。

### 2019.12.13
* Xojo 2019r3で「Supports Dark Mode」をONにして保存し直した。
* **Single**
    * **myListBox**
        * ダークモードに対応。（ダークモード非対応のXojoバージョンでもエラーにならないので大丈夫）

### 2019.8.10
* **Single**
    * **myTextArea**
        * 「SetSystemFont」メソッド追加。
        * 「SetFontWithName」メソッド追加。
        * 「SetFontPanelMenu」メソッド追加。
        * 「LayoutOrientation」プロパティ追加。

### 2019.8.3
* **Single**
    * BringFrontmostMeメソッドを改善。
    * SetProxyIconメソッドを改善。
* **Multi**
    * ウインドウメニューの記号が不正確になる不具合を修正。
    * SetProxyIconメソッドを改善。

### 2019.8.2
* **Single**
    * Generalモジュールにメソッド「BringFrontmost」「BringFrontmostMe」を追加。
    * Window1にSetProxyIconメソッドを追加。
* **Multi**
    * Window1にSetProxyIconメソッドを追加。

### 2019.8.1
* **Single**
* **Droplet**
    * Quit時のクラッシュをさらに防ぐため、QuitをすべてNSApplicationのterminateを使用するようにした。

### 2019.7.27
* **Single**
    * **UnicodeNormalization**
        * 不要なエラー表示がされていたのを修正。

### 2019.7.26
* **Single**
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
* **Multi**
    * AboutWindowのアイコンのHi-DPI対応。
    * App.CloseにQuit時のクラッシュ防止を仕込んだ。
* **Droplet**
    * App.CloseにQuit時のクラッシュ防止を仕込んだ。

### 2019.7.21
* **Single**
    * **Extras**
        * RegExXojoモジュールを追加
            * XojoのRegExクラス関連のメソッド集。
        * UnicodeNormalizationモジュールを追加
            * Unicode正規化関連のメソッド集。
    * App.EnableMenuItems を改善。
* **Multi**
    * App.EnableMenuItems を改善。

### 2019.7.7
* **Single**
    * **myTextArea**
        * Undo履歴を区切る「BreakUndo」メソッド追加。
        * マージンを設定できる「SetMargin」メソッド追加。
        * フォント内のlineGapを使うかどうかを設定できる「UsesFontLeading」メソッド追加。（NSLayoutManagerではデフォルトがTrue。これをFalseにできる）
        * メソッドとプロパティの名称変更
            * SelectAllSV → SolvedSelectAll
            * SelTextSV → SolvedSelText
            * TextSV → SolvedText
        * [insertText:](https://developer.apple.com/documentation/appkit/nstextview/1449174-inserttext?language=objc) がDeprecatedだったので、[insertText:replacementRange:](https://developer.apple.com/documentation/appkit/nstextinputclient/1438258-inserttext?language=objc)に変更した。
