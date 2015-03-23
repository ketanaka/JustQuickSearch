# Just Quick Search

### [目次]

  - カスタム検索について
  - Open URL 機能について

# カスタム検索について
設定画面の「Custom Search」では、検索対象を自由に設定できます。
設定できる項目は、Title と URL です。

Title は検索対象選択画面に表示される、検索対象の名前です。
URL は検索実行時に開く URL です。

URL 内の「キーワード」を与えたい部分は**`_._`**で表現します。

**例）Yahoo! 検索**

Title : Yahoo!

URL : http://search.yahoo.co.jp/search?ei=UTF-8&p=_._

上記の設定を行うと、キーワードを「iPhone」として検索を実行した場合、http://search.yahoo.co.jp/search?ei=UTF-8&p=iPhone が開きます。

### URL 例一覧

以下の URL を使用したい場合は、URL をコピーし、本アプリ設定画面の「Custom Search」-> 「URL」に貼り付けてください。

**Yahoo! 検索**

http://search.yahoo.co.jp/search?ei=UTF-8&p=_._

**マップ**

http://maps.google.com/maps?q=_._

**Google 翻訳  英語 -> 日本語**

http://translate.google.com/m/translate?q=_._&sl=en&tl=ja

**Google 翻訳  日本語 -> 英語**

http://translate.google.com/m/translate?q=_._&sl=ja&tl=en

**goo 辞書 すべての辞書検索**

http://dictionary.goo.ne.jp/smp/srch/all/_._/m0u/

**goo 辞書 国語辞書検索**

http://dictionary.goo.ne.jp/smp/srch/jn2/_._/m0u/

**goo 辞書 英和検索**

http://dictionary.goo.ne.jp/smp/srch/ej3/_._/m0u/

**goo 辞書 和英検索**

http://dictionary.goo.ne.jp/smp/srch/je2/_._/m0u/

**コトバンク 用語検索**

http://m.kotobank.jp/word/_._

**コトバンク 英和検索**

http://m.kotobank.jp/ejword/_._

**コトバンク 和英検索**

http://m.kotobank.jp/jeword/_._

**YouTube**

http://m.youtube.com/results?search_query=_._

**ニコニコ動画**

http://sp.nicovideo.jp/search/_._

#### NOTE

`http://`で始まるURLは、検索実行時に Safari が起動します。Sleipnir がインストールされている状態で、`http://`を`sleipnir://`に置き換えると Sleipnir が起動します。Sleipnir では広告を非表示に設定することもできます。

### アプリ連携

※これ以降は別途アプリのインストールが必要です。

**Google Maps**

comgooglemaps://?q=\_._

**Twitter**

twitter://search?query=\_._

**kotobank for iPhone**

kotobank://search?query=\_._

**ウィズダム英和・和英辞典**

mkwisdom://jp.monokakido.WISDOM/search?text=\_._

**大辞林**

mkdaijirin://jp.monokakido.DAIJIRIN/search?text=\_._

**角川類語新辞典**

mkruigo://jp.monokakido.RUIGO/search?text=\_._

みなさんもお気に入りの URL を探してみてください。

# Open URL 機能について

`http://`または`https://`から始まる URL が入力された状態で検索を実行すると、本アプリはその URL を直接開きます。URL を開くアプリは「with Scheme」で設定可能です。

#### スキーム一覧（私が動作確認したものです）

  - http -> Safari で開く
  - sleipnir -> Sleipnir で開く
  - googlechrome -> Chrome で開く

デフォルトは Safari で開きます。Use Sleipnir がオンなら Sleipnir で開きます。

「with Scheme」でスキームを設定するときは、そのスキームが有効かをチェックしています。スキームが正しいのにエラーメッセージが表示されるときは、そのアプリがインストールされていない可能性があります。ご注意ください。

通知センターからの起動時には、URL は自動で開かれます。（Auto Search のオン/オフにかかわらず）

内部の処理としては、`http://`または`https://`から始まる URL が入力され検索が実行されたとき、「with Scheme」でスキームが設定されている場合は、`http`の部分をそのスキームに置き換えます。

##### 例）

  - with Scheme : `googlechrome`
  - 入力された URL : `http://www.google.com`
  - 検索時に開かれる URL : `googlechrome://www.google.com`

私は Sleipnir と Chrome しか確認していませんが、他にも`http`の部分を`カスタム URL スキーム`で置き換えて、URL を開くことができるアプリがあるかもしれません。

興味がある方は探してみてください。
