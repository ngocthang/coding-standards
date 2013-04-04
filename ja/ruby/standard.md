##Ruby コーデング規約（標準スタイル編）

####レイアウト

#####エンコーディング
* UTF-8以外は使用しない。

* 基本的にスクリプトエンコーディングのマジックコメントが必要なソースコードにしない。

**理由**

* UTF-8がcomputer/webの世界で事実上の標準エンコードであるため。

* 2バイト文字は基本的にユーザーのために記述するものであり、それはソースコードに埋め込まれずにlocaleファイル等に記述されるべきものであるため。


#####基本
* インデントはホワイトスペース2個
* ハードタブは使用しない
* 1行の文字数は80文字以下にする
* 行の最後に無駄なホワイトスペースは付けない
* 演算子の前後、コロンの前後、カンマの後ろとセミコロンの後ろににホワイトスペースを1個置く
* カンマ、セミコロンの前にはホワイトスペースは置かない

```ruby
sum = 1
a, b = 1, 2
1 > 2 ? true : false; puts 'Hi'
```

* [] () {} 全ての前後にホワイトスペースは置かない

```ruby
a = [1, 2, 3] #"[" の左のスペースは = の後ろのもの
[1, 2, 3].each{|num| puts num * 2}
def method(a, b, c)
```

