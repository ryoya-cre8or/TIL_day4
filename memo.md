### やったこと

* DartPadのnull safety
* 1行関数での記述

**DartPadのnull safety**

*　コンストラクターを使ったベストな解決策はコンストラクターの引数にrequiredをつける

**変更前1**

* 名前付き引数であるn1とn2がnullである可能性がある

※ただし通常の引数では問題ない

<img src="https://github.com/ryoya-cre8or/TIL_day4/blob/main/%E5%A4%89%E6%9B%B4%E5%89%8D1%E7%94%BB%E5%83%8F.png" width="300px"/>


**変更前2**

* n1とn2がnullだった時戻り値がint型にならない

<img src="https://github.com/ryoya-cre8or/TIL_day4/blob/main/%E5%A4%89%E6%9B%B4%E5%89%8D2%E7%94%BB%E5%83%8F.png" width="300px"/>


**変更後**

* null防止をする

<img src="https://github.com/ryoya-cre8or/TIL_day4/blob/main/%E5%A4%89%E6%9B%B4%E5%BE%8C%E7%94%BB%E5%83%8F.png" width="300px"/>

if文を省略することも可能

```
a ??= 1 //aがnullの時は１を代入
```

<img src="https://github.com/ryoya-cre8or/TIL_day4/blob/main/%E5%A4%89%E6%9B%B4%E5%BE%8C%E7%94%BB%E5%83%8F(%E7%9C%81%E7%95%A5ver.).png" width="300px"/>

**1行関数での記述**

```
int add() {
  return 5 + 2;
}
```

上のコードは下と同義
```
int add() => 5 + 2;
```

つまりこう書ける
```
void main() {
  print(add()); 
}

int add() => 5 + 2;
```
