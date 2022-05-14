# Fast-API Tutorial
TODOアプリをFast-APIで構築


```
# コンテナ起動
% docker-compose up
```
- docker-compose.yaml
	docker-composeの定義ファイル。この中で、Dockerfileを呼び出して、Dockerコンテナのビルド

- Dockerfile
  Dockerの定義ファイル。
  利用する公開イメージを取得し、 poetryによって、パッケージ定義ファイルである pyproject.toml を元に各pythonパッケージをインストール。


## Library
- Pydantic
  FastAPIに依存するライブラリ　型ヒント（Type Hint）のバリデーションを行ってくれる（単なるIDEの型チェックだけのためではなく、実行時の評価を行う）

- Pytest
  ユニットテストフレームワーク

- pytest-asyncio
  Pytestを非同期用に拡張

### Type hint
- Union
  X型 もしくは Y型  e.g. Union[X, Y] = X or Y

- Optional
  None もしくはX型  e.g. Optional[X] = Union[X, None]

### Pytest
- フィクスチャ（fixture）
    テスト関数の前処理や後処理を定義することができる関数。xUnit系のユニットテストツールで言うところの、 setup() や teardown() に相当、Pythonには yield 文があるため、これらをまとめて１つの関数として定義可能。（ジェネレータとして定義）

