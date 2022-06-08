# LINE BOT 2022

## 2022/06/09  2:24

- 作成し始めた。
- AWS Lambda + Python 構成
- 気になるので [AWS Chalice](https://aws.github.io/chalice/index.html#)を使ってみる

依存管理には poetry を使っている

以下のようにして Chalice をインストールする

```
poetry add chalice
```

chaliceプロジェクトの初期化(helloworldは適宜自分の好きなプロジェクト名にする)
```
poetry run chalice new-project helloworld
```

おれが使っているPythonのバージョンが3.10だったので警告が出た。まだAWS Lambda で Python3.10 がサポートされていないっぽい
```
$ poetry run chalice new-project helloworld
C:\Users\takum\dev\github.com\veltiosoft\line-bot\.venv\lib\site-packages\chalice\cli\__init__.py:424: UserWarning: You are currently running python3.10, but the closest supported version on AWS Lambda is python3.9
Please use python3.9, otherwise you may run into deployment issues.
  validate_python_version(Config.create())
Your project has been generated in ./helloworld
```