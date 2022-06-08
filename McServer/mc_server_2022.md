# MC Server

マイクラサーバー構築について書く

## 2022/06/08 23:48

- version up 作業を行った
	- 1.18 -> 1.19
	- ついでに自分のマイクラも1.19をダウンロードしておいた
	- アップデートコマンドは問題なく実行完了
	- ログインしてからしばらく散歩したが特に問題なさそう
		- このへんはユーザーからの報告あり次第対応

version up command:
```shell
curl https://gist.githubusercontent.com/zztkm/87da5f85c78ac80a03182807bed6a6bc/raw/68b894074ad9fe63bf0f01de3def5e886657bfdc/build-spigot-latest.sh | bash
```

- 上のコマンドを流すと、mc-spigot server の最新バージョンがビルドされる
- ただし、サーバーのメモリなどを決め打ちにしているなどがありパフォーマンスを出せない場面もある
	- つまりちょっとビルド遅い
- エラーハンドリングもしていないのでかなり自己責任で使ってもらう必要がある
- source code: https://gist.github.com/zztkm/87da5f85c78ac80a03182807bed6a6bc

