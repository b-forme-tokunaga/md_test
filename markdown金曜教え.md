金曜日に実演できれば

GitHub Flavored Markdown
`GitHub Flavored Markdown`

目標
ビジュアルとコードの一致だけでいい。
知らない人に周知。

何で、こんなことをするのか、READMEを書いてもらうために。
- zoomでライブ感を出す。自分のvscodeの画面を共有して。
- 自分のvscodeで、`.md`ファイルをプレビューする。
  - タブを右クリックで、「プレビューを開く」をクリック。
  - 編集パネルを二画面にしてプレビューを見ながら書くのもいいです。



# 金曜にギットハブの readme に使える程度のマークダウンの書き方を教える

金曜にギットハブの readme に使える程度のマークダウンの書き方を教えるの 30 分の説明ぐらい。

</br>

厳密に教えるのは `GitHub Flavored Markdown` という Markdown が掛かれている。

- チートシート [Markdown 記法 サンプル集](https://qiita.com/tbpgr/items/989c6badefff69377da7)
- 参考ページその２ [メモ書きやドキュメント作成に便利な「Markdown 記法」を使ってみよう](https://www.asobou.co.jp/blog/bussiness/markdown#:~:text=Markdown%EF%BC%88%E3%83%9E%E3%83%BC%E3%82%AF%E3%83%80%E3%82%A6%E3%83%B3%EF%BC%89%E3%81%A8%E3%81%AF,%E4%BB%A5%E4%B8%8B%E3%81%AE%E7%89%B9%E5%BE%B4%E3%81%8C%E3%81%82%E3%82%8A%E3%81%BE%E3%81%99%E3%80%82)

## 教える内容

- 見出し系
  - [見出し](https://qiita.com/tbpgr/items/989c6badefff69377da7#%E8%A6%8B%E5%87%BA%E3%81%97)
- リスト系
  - [箇条書きリスト](https://qiita.com/tbpgr/items/989c6badefff69377da7#%E7%AE%87%E6%9D%A1%E6%9B%B8%E3%81%8D%E3%83%AA%E3%82%B9%E3%83%88)
- `> 引用`
  - [引用](https://qiita.com/tbpgr/items/989c6badefff69377da7#%E5%BC%95%E7%94%A8)
- コードプレビュ
    - [pre記法](https://qiita.com/tbpgr/items/989c6badefff69377da7#pre%E8%A8%98%E6%B3%95%E3%82%B9%E3%83%9A%E3%83%BC%E3%82%B94-or-%E3%82%BF%E3%83%96)
    - [GFM:pre記法](https://qiita.com/tbpgr/items/989c6badefff69377da7#gfmpre%E8%A8%98%E6%B3%95%E3%83%81%E3%83%AB%E3%83%803)
- 強調系
    - [code記法](https://qiita.com/tbpgr/items/989c6badefff69377da7#code%E8%A8%98%E6%B3%95)から太文字と斜め文字の混合まで
    - [GFM:取り消し線](https://qiita.com/tbpgr/items/989c6badefff69377da7#gfm%E5%8F%96%E3%82%8A%E6%B6%88%E3%81%97%E7%B7%9A)
- リンク([外へのリンク](https://qiita.com/tbpgr/items/989c6badefff69377da7))
    - [リンク](https://qiita.com/tbpgr/items/989c6badefff69377da7#%E3%83%AA%E3%83%B3%E3%82%AF)
- 文章の改行
    - 空行を入れるか`</br>`で改行。
- html タグをそのまま書ける。
    - ***知っているhtmlタグを言ってください。*** **おそらく有効です**

## html タグをそのまま書ける実演

<script>alert('JavaScriptのalert関数の実行');</script>
<script>console.log('コンソールログも動く？');</script>

```js
<script>alert('javaScriptのalert関数の実行');</script>
```

で js は実行できるかも？実行できるとセキュリティー上の問題が発生するが......

```php
<?php
5+5
```

<details>
    <summary>折り畳み</summary>

```html

<details>
    <summary>折り畳み</summary>
    <b>折り</b>た<i>た</i>まれる本文
</details>

 ```

   </br>
    <b>折り</b>た<i>た</i>まれる本文
</details>

記法法のそれぞれの拡張。上記 5 つの他の場所での使用例。

</br>
改行のタグ後のに改行して、code記法にならない場合もある->`こことか`

改行

改行１

改行 2

> 引用
>
> > 引用２
> >
> > > 引用 3

###### シャープ 6 語

####### シャープ 7 語

############################## シャープ 31 語

1. 1-1
1. 1-2
1. 1-3
1. 1-4

上下一行開け、タブか半角空白でブロックコードになるらしい、知らなかった。

    class Hoge
      def hoge
        print 'hoge'
      end
    end


バッククォート×3でやった方が安全？シンタックスハイライト使えるし？`~`チルダ方式もあったようだ。
```ruby
    class Hoge
      def hoge
        print 'hoge'
      end
    end
```
