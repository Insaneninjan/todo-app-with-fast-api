# Fast-API Tutorial

```
% docker-compose up
```


- docker-compose.yaml
	docker-composeの定義ファイル。この中で、Dockerfileを呼び出して、Dockerコンテナのビルドを行います。
- Dockerfile
  Dockerの定義ファイル。
  利用する公開イメージ（今回はPython 3.9がインストールされたOSイメージ）を取得し、 poetry （後述）によって、パッケージ定義ファイルである pyproject.toml を元に各pythonパッケージをインストールします。
