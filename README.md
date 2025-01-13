# Just Quick Search

### [目次]

- `カスタム検索` について
- `URL を直接開く` 機能について

# カスタム検索について

設定画面の「カスタム検索」では検索対象を自由に設定できます。
設定できる項目はタイトルと URL です。

タイトルは検索対象選択画面に表示される検索対象の名前です。
URL は検索実行時に開く URL です。

URL 内の「キーワード」を与えたい部分は `_._` で表現します。

### 例）Yahoo! 検索

タイトル : Yahoo!

URL : `http://search.yahoo.co.jp/search?ei=UTF-8&p=_._`

上記の設定を行うと、キーワードを「iPhone」として検索を実行した場合 http://search.yahoo.co.jp/search?ei=UTF-8&p=iPhone が開きます。

### URL 例一覧

以下の URL を使用したい場合は URL をコピーし、本アプリ設定画面の「カスタム検索」-> 「URL」に貼り付けてください。

- Yahoo! 検索
  - `http://search.yahoo.co.jp/search?ei=UTF-8&p=_._`
- マップ
  - `http://maps.google.com/maps?q=_._`
- Google 翻訳  英語 -> 日本語
  - `https://translate.google.com/?q=_._&sl=en&tl=ja&text=_._&op=translate`
- Google 翻訳  日本語 -> 英語
  - `https://translate.google.com/?q=_._&sl=ja&tl=en&text=_._&op=translate`
- YouTube
  - `http://www.youtube.com/results?search_query=_._`
- X
  - `https://x.com/search?q=_._`

# URL を直接開く機能について

`http://` または `https://` から始まる URL が入力された状態で検索を実行すると、本アプリはその URL を直接開きます。URL を開くアプリは `スキーム` で設定可能です。

### スキーム一覧（私が動作確認したものです）

  - `http` -> Safari で開く
  - `jqs` -> アプリ内ブラウザで開く
  - `googlechrome` -> Chrome で開く
  - `sleipnir` -> Sleipnir で開く

デフォルトは Safari で開きます。  
アプリ内ブラウザが ON の場合はアプリ内ブラウザで開きます。

内部の処理としては `http://` または `https://` から始まる URL が入力され検索が実行されたとき、スキームが設定されている場合は `http` の部分をそのスキームに置き換えます。

#### 例）

  - スキーム : `googlechrome`
  - 入力された URL : `https://www.google.com`
  - 検索時に開かれる URL : `googlechromes://www.google.com`

私は Chrome と Sleipnir しか確認していませんが、他にも `http` の部分を `カスタム URL スキーム` で置き換えて URL を開くことができるアプリがあるかもしれません。

興味がある方は探してみてください。
