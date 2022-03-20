# my_dockerfiles
Collection of template dockerfiles for my own use.
These dockerfiles are mainly used with Remote Containers, the extension of VisualSourceCode

## How to use
ディレクトリごとコピーし、使用目的に合わせて編集してからdockerを起動します
テンプレートとしての位置づけなので、直接dockerを起動することを想定していません。

## reference sites
- [VScodeでdockerの開発環境(python)を使う。](https://qiita.com/katakaku/items/b8dcac4aa14d585e4038)
    Remote Containersを使った操作の概要

- [【venv不要】Remote Containersで作る最強のPython開発環境【VSCode/Docker】](https://qiita.com/0MeO/items/1fc3995e568d2c95569e)
    Python + Docker + VSCodeの基本

## 各Dockerfileの説明
### Python 3.10
Remote Containersを使って生成したDockerfileをベースにしました。
次の機能が組み込まれており、すぐにPythonを使うことができます。
- VSCodeコードのlinterとformattingの設定
- autopep8, flake8

今のところ(Mar., 2022)Python3.10は"Fluent Python 2nd"の勉強の目的でつかうため、追加でインストールしたライブラリはNumpyだけです。必要に応じてrequirements.txtに追加してください。

### ds_all_in_one
データサイエンス用の機能がほぼ全部入りです。
DockerHubのjupyter/datascience-notebookが元イメージで、Python、R、Juliaとそれらのデータサイエンス用のライブラリが入っています。
Pythonのlinterにflake8を、formatterにblackを追加しました。
イメージのビルドに時間はかかりますが、その後は快適に使えると思います。
