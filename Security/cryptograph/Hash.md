# Hash関数とは

任意の

## 特徴

### 1. 一方向性


### 2. 第二現象計算困難性

ある入力値と同じハッシュ値となるような別の入力を求めることが困難

### 3. 衝突困難性

同じ出力値を生成する2つの入力値を発見することが困難

## Hash関数の意義

Hash valueはfinger printと一緒。

## Hash関数の具体化

MD4,MD5,SHA,SHA-1,SHA-2,SHA-3 ...

## Hash関数の利用

### 1. パスワード認証

普通はサーバにはハッシュ値しかない。

But あなたのパスワードは〜ですよとしてメールが帰ってくるとしたら、生のパスワードが入っていること。

### 2. File改ざん検知

1. Fileに対し、Hash値を計算し、結果を安全に保存(*)
2. 再度ハッシュ値を計算し(*)と比較
3. 両者が同じであれば改ざんなしとみなせる

### 3. Message改ざん検知

MAC(Message Authentication Code)
メッセージにMACを追加し送信
マCをhash(K,m)などで生成(Kは共有鍵)
