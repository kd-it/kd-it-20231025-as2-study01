# 練習2

練習1と同様に「読み込むたびに1〜6の値を返す」Webアプリケーションを作って下さい。
仕様としては、以下のものとします。

* 実装できるなら言語は問いません、不安な方はPHPでいいでしょう
* 呼び出されたらJSON形式のデータとして、キー"roll"の値として返してください
    * httpにおけるContent-TypeもJSONのものとなるようにしてください(`application/json`)
* イメージでは80をEXPOSEしておいてください(暗黙でも可)
* 上記イメージを使ったポッドマニフェストを作成してください、ただし仕様として以下を含めてください
    * マニフェストファイルは`pod-diceweb.yml`とする
    * ポッド名はdiceとする
    * リソース制限でCPU利用を50m(50ミリ秒/秒)とする
    * コンテナの外部露出ポートとして80/tcpを使用する宣言を含める

戻りのJSON例としては、以下のようなものとなります。

```json
{"roll": 5}
```
