# Contents

- About Custom Search
- About OpenURL

# About Custom Search

"Custom Search" in "Settings", You can customize the search targets.  
Item is "Title" and "URL".  
"Title" is name of search target.  
"URL" is a URL that opens when you execute a search.  
Represented by the `_._`, you want to give a "keyword" in the URL.

## Ex) Yahoo! Search

**Title** : Yahoo!

**URL** : `http://search.yahoo.com/search?ei=UTF-8&p=_._`

Do the above, if you execute a search as keyword is "iPhone",  
It's opened this URL.

http://search.yahoo.com/search?ei=UTF-8&p=iPhone

## List of URL Examples

If you want to use the following URL, please copy and paste to "Settings" -> "Custom Search" -> "URL".

- Apple Maps
    - `https://maps.apple.com/?q=_._`
- Google Maps
    - `comgooglemaps://?q=_._`
- Yahoo! Search
    - `http://search.yahoo.com/search?ei=UTF-8&p=_._`
- Google Translate  English -> Japanese
    - `https://translate.google.com/?q=_._&sl=en&tl=ja&text=_._&op=translate`
- Google Translate  Japanese -> English
    - `https://translate.google.com/?q=_._&sl=ja&tl=en&text=_._&op=translate`
- YouTube
    - `http://www.youtube.com/results?search_query=_._`
- X
    - `https://x.com/search?q=_._`

# About OpenURL

When you execute a search with the URL beginning with "https://" or "http://", this app will directly open that URL.  
Can be set in `Scheme` app to open the URL.

## Ex) Open with Google Chrome

Scheme : `googlechrome`

Install "Chrome" : https://apps.apple.com/us/app/google-chrome/id535886823

## Ex) Open with Sleipnir

Scheme : `sleipnir`

Install "Sleipnir" : https://apps.apple.com/us/app/sleipnir-mobile/id404732112
