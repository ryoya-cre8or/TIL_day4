### やったこと

* DartPadのnull safety

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
