# Gen command

## 概要
HTMLやCSSを学習したいので、プレーンなHTMLプロジェクトをローカルで作成したい！ 
そんなときのためのコマンドです。

## 導入

1. 以下の例のような形でリポジトリをクローンします

ex.

```
- HOME
   - クローンするためのディレクトリ  <-- ここにリポジトリをクローンする !
```

2. パスを通します (**dirname** はクローンされた場所のフルパス).

```
echo 'export PATH=$PATH:dirname' >> ~/.bash_profile
```

上の例だと、以下のようになります↓
ex.

```
echo 'export PATH=$PATH:/Users/ユーザー名/クローンするためのディレクトリ/Gen-command' >> ~/.bash_profile
```

3. シェルの設定を反映

```
source ~/.bash_profile
```

Enjoy!😄

## 使い方

このコマンドは、指定されたディレクトリ（dirName）にhtmlとcssのファイルを生成します。

```
gen dirName
```

このオプションは、デフォルトのcssファイルの名前をオプション引数の名前に書き換えて生成されます。

```
gen dirName -c origin.css
```

これにより、javascriptファイルも生成されます。

```
gen dirName -j
```

Bootstrap テンプレート付きでも生成できます。

```
gen dirName -b
```

## 仕様

* macOSX Catalina 10.15.6
