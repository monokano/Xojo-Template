## 変更点

#### Single Window Desktop App for Mac
* myTextArea　2019.7.7
    * Undo履歴を区切る「BreakUndo」メソッド追加。
    * マージンを設定できる「SetMargin」メソッド追加。
    * フォント内のlineGapを使うかどうかを設定できる「UsesFontLeading」メソッド追加。（NSLayoutManagerではデフォルトがTrue。これをFalseにできる）
    * メソッドとプロパティの名称変更
        * SelectAllSV → SolvedSelectAll
        * SelTextSV → SolvedSelText
        * TextSV → SolvedText
    * [insertText:](https://developer.apple.com/documentation/appkit/nstextview/1449174-inserttext?language=objc) がDeprecatedだったので、[insertText:replacementRange:](https://developer.apple.com/documentation/appkit/nstextinputclient/1438258-inserttext?language=objc)に変更した。