# 画像変換コマンド

## 実装仕様
- ディレクトリを指定する
- 指定したディレクトリ以下のJPGファイルをPNGに変換（デフォルト）
- ディレクトリ以下は再帰的に処理する
- 変換前と変換後の画像形式を指定できる（オプション）
- 自作パッケージと標準パッケージと準標準パッケージのみ使う
    - 準標準パッケージ：golang.org/x以下のパッケージ
- ユーザ定義型を作ってみる
- Go Modulesを使ってみる

> @tenntennさんが作成したGopher道場の課題です。 Gopher道場については以下のURLから参照してください。
> - https://gopherdojo.org/

## 使用方法
- ビルド
```zsh
go build main.go
```

- 実行例
```zsh
./main -b png -a jpeg (ディレクトリのパス名)
```

- オプション <br>
  <br>
-b : 変換前の拡張子 <br>
-a : 変換後の拡張子  