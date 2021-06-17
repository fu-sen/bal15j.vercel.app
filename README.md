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

転送先を確認できるように GitHub でソースを公開しています。\

- [Deno Deploy](https://deno.com/deploy)
- [Deno Deploy | ふうせん🎈 FU-SEN](https://balloon.asia/deno-deploy/)

2021年6月18日より Deno Deploy  を採用しています。\
わざわざソースを記載する必要がありますが、世界各地のエッジサーバで処理され、\
日本でも東京・大阪にエッジサーバが存在します。

`index.js` のソースにリストを入れています。ここで 転送元・先 を確認可能です。

```
const redir = new Map([
  ["転送元", "転送先"],
  ["転送元", "転送先"],

           :

  ["転送元", "転送先"],
  ["転送元", "転送先"]
])
```

記載のない参照は Not Found です。

- [Cloudflare Workers](https://workers.cloudflare.com/)
- [Cloudflare Workers | ふうせん🎈 FU-SEN](https://balloon.asia/cloudflare-workers/)

Deno Deploy を採用する前は Cloudflare Workers を使用しています。\
この 2 サービスは JavaScript ソースで互換性があります。\
Deno Deploy が公開ソースをシンプルにできるのと、\
Cloudflare Workers は Workers Site も使用していたため、\
Deno Deploy で動作可能な環境は移してサーバを分散する事にしました。

幸い Deno Deploy でそのまま動作可能なソースの状態で維持できていました。

- [独自ドメインで独自の短縮 URL を作る方法。| ふうせん🎈 FU-SEN](https://balloon.asia/2020/02/%E7%8B%AC%E8%87%AA%E3%83%89%E3%83%A1%E3%82%A4%E3%83%B3%E3%81%A7%E7%8B%AC%E8%87%AA%E3%81%AE%E7%9F%AD%E7%B8%AE-url-%E3%82%92%E4%BD%9C%E3%82%8B%E6%96%B9%E6%B3%95/)

いくつか転送ができる Web サービスを把握しているため、\
後に使用する Web サービスを変更する可能性があります。\
（実際数ヶ月おきに変更しています）

___

Powered by [Deno Deploy](https://deno.com/deploy)
