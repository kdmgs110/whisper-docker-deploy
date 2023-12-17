# 使い方

このレポジトリはwhisperをフォークして、dockerでbuildすればすぐ使えるようにしたものです。

https://github.com/openai/whisper

## セットアップ 
- Docker Desktopをインストールしてください
- 以下のコマンドを実行してください

```
docker build -t whisper .
docker run -it -d -v $(pwd):/workspace/ --name whisper whisper
docker exec -it whisper bash
```

※こちらを参考にして作成しました
https://zenn.dev/kento1109/articles/d7d8f512802935

## 利用方法

`whisper sample.mp3 --language ja`