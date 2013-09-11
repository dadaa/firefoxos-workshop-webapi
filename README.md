# firefoxos-worksho-webapi
## firefoxos,workshop,webapi
This document is made by [gitfab](http://gitfab.org)
---
# WebAPI を使ったアプリ
Firefox OS では、html、css、JavaScript といったウェブ技術によって記述・構成されていきますが、既存のウェブアプリケーションとの相違点の一つは、デバイスとの連携ができる点であり、より魅力的なウェブアプリケーションを作る可能性を秘めていると考えます。ここでは、WebAPI を使った簡単なアプリのテンプレートや WebAPI の種類、許可などについて記述しています。
---
# スケルトンのダウンロード


[webapitests.zip](https://raw.github.com/dadaa/firefoxos-worksho-webapi/master/gitfab/resources/webapitests.zip)
---
# マニフェストファイルの編集
manifest.webapp をテキストエディタで開き、編集してください。
---
# ひとまず動くか確認する
notification が出れば成功。

![notification.png](https://raw.github.com/dadaa/firefoxos-worksho-webapi/master/gitfab/resources/notification.png)
---
# WebAPI を使ってみる
以下のページを参考に、index.html, main.js, main.css を編集して、WebAPI を取り込んでみる。

[https://developer.mozilla.org/ja/docs/WebAPI](https://developer.mozilla.org/ja/docs/WebAPI)
---
# WebAPI の許可
利用する WebAPI によっては、利用者の許可が必要なものがあります。その場合、manifest.webapp に記述が必要になります。例えば以下は Geolocation を利用する場合の記述例になります。

{ 
  "version": "0.1",
  "name":"sample",
...
  "permissions": {
    "geolocation":{}
  }
}


許可が必要な WebAPI については以下をご参考ください。
[https://developer.mozilla.org/ja/docs/Web/Apps/App_permissions](https://developer.mozilla.org/ja/docs/Web/Apps/App_permissions)
---
# 実装例
以下は Ambient Light 、Geolocation、Proximity を用いた実装例です。

[webapitests-all.zip](https://raw.github.com/dadaa/firefoxos-worksho-webapi/master/gitfab/resources/webapitests-all.zip)

![webapitests.JPG](https://raw.github.com/dadaa/firefoxos-worksho-webapi/master/gitfab/resources/webapitests.JPG)
---
# WebAPI を使ったサンプルアプリを作ってみる

---
