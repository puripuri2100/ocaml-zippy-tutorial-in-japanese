モジュール
==============================

長い module type を `*.ml` と `*.mli` で繰り返すのが面倒なら `*_intf.ml` を書く
===========================================================================================

モジュール型とそれに関連するコードを書いていて、モジュール型が長くなると
`*.ml` ファイルにも `*.mli` ファイルにもそのモジュール型を書かなければならなくなり、
とても面倒になる。そういった場合はモジュール型の定義だけを外に出してしまうとよい。

例えば、 `*_intf.ml` というファイルに。 `*` というモジュールに関するインターフェースを
定義する、というくらいの意味の名前。ここにはモジュール型の定義のみを書くことにすれば
隠蔽の必要もないので `*_intf.mli` を書く必要もない。
