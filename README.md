## k.bal.gdn

- [Kidspod;](http://kidspod.club/)
- [イチゴジャム レシピ](https://15jamrecipe.jimdofree.com/)

Kidspod; で公開しているプログラム等から「プログラムをみる」をクリックした時、\
安全のためにリンク先の URL が表示されているのですが、\
イチゴジャム レシピ で採用している [Jimdo](https://www.jimdo.com/jp/) では\
URL に日本語を使用するため、長く分かりにくい URL になってしまいます。\
そこで専用の短縮 URL を作成し、改善する事にしました。

___

## 転送 URL の確認

転送先を確認できるように GitHub でソースを公開しています。

- [▲ Vercel](https://vercel.com/)
- [Vercel | ふうせん🎈 FU-SEN](https://balloon.asia/vercel/)

2021年12月6日より ▲ Vercel  を採用しています。\
`vercel.json` で転送処理ができます。このファイルで 転送元・先 を確認可能です。

```
{
  "redirects": [
    { "source": "転送元", "destination": "転送先" },
    { "source": "転送元", "destination": "転送先" },

           :

    { "source": "転送元", "destination": "転送先" },
    { "source": "転送元", "destination": "転送先" }
])
```

記載のない参照は特別処理をしない場合はファイルを参照・表示しますが、\
該当ファイルがなければ `404.html` を表示します。（Not Found）

___

Powered by [▲ Vercel](https://vercel.com/)
