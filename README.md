# url_conv
URL Converter ~ Encoded only "Zenkaku"(2Byte-Shift_JIS) String! ~

## 概要
　例えば「https://ja.wikipedia.org/wiki/文字コード 」といったURLがあるとします。  
　その際、Twitterにそのまま貼り付けると、1バイト文字列以外……つまり「文字コード」の部分に自動でリンクが貼られません。  
　そこで、「https://ja.wikipedia.org/wiki/%E6%96%87%E5%AD%97%E3%82%B3%E3%83%BC%E3%83%89 」と、全角部分だけをURLエンコードしておく必要があります。  
　手動でそれを行わないとならないのは控え目に言ってクソですので、自動化するアプリを作りました。

## 使い方
　テキストボックスにURLを入力してボタンを押します。おしまい。

## 注意点
　細かい話ですが、「全角部分」の長さが1024バイト以上になると正常に変換されません。  
　このバグはHSPの仕様も絡んで修正が難しいので放置しています。  
(どうせそんなURLが入力されることはまずないはずですし)  
　また、[Punycode](https://ja.wikipedia.org/wiki/Punycode)には対応していません……。

## 作者
YSR

## 使用言語
HSP3

## ライセンス
MIT License
