# even-odd-problem
「任意の整数について、奇数か偶数か判定する」コードを自動生成するコードについてまとめたリポジトリです。ネタ元: https://twitter.com/NAGAYASU_Shinya/status/1143868066440216577

## OCaml

From [https://twitter.com/50storms/status/1144233650495475712](https://twitter.com/50storms/status/1144233650495475712)

```ocaml
(* MetaOCaml *)
let rec oddaux param b i =
  if i = max_int then
    .< false >.
  else .< if .~param = i then b else .~(oddaux param (not b) (i+1))>.
in .<fun x -> .~(oddaux .<x>. false 0)>.
```
