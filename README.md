# my_dockerfiles
Collection of template dockerfiles for my own use.
These dockerfiles are mainly used with Remote Containers, the extension of VisualSourceCode

## How to use
ディレクトリごとコピーし、使用目的に合わせて編集してからdockerを起動します
テンプレートとしての位置づけなので、直接dockerを起動することを想定していません。

## reference sites
- [VScodeでdockerの開発環境(python)を使う。](https://qiita.com/katakaku/items/b8dcac4aa14d585e4038)
    Remote Containersを使った操作の概要を説明しています。

## 各Dockerfileの説明
### Python 3.10
Remote Containersを使って生成したDockerfileをベースにしました。
次の機能が組み込まれており、すぐにPythonを使うことができます。
- VSCodeコードのlinterとformattingの設定
- autopep8, flake8

今のところ(Mar., 2022)Python3.10は"Fluent Python 2nd"の勉強の目的でつかうため、追加でインストールしたライブラリはNumpyだけです。必要に応じてrequirements.txtに追加してください。

