# 1 TO 10

1から指定した数字まで、画面に散らばった数字を順番にタップしていくスピードゲームです。単一の `index.html` で完結する静的サイトなので、GitHub Pages でそのまま公開できます。

## 遊び方

- ホーム画面のスライダー／±ボタンで、最後の数字(2〜20)を設定します。
- STARTを押すと3秒のカウントダウン後にゲーム開始。
- 1から設定した数字まで、順番にタップします。
- 間違った順番でタップすると0.35秒のペナルティが加算されます。
- タイムに応じて S / A / B / C / D のランクが表示されます。
- 結果とベストタイムは、設定ごとに自動保存されます(YouTube Playables環境ではプラットフォームのセーブAPI、それ以外はブラウザのlocalStorageを使用)。

対応言語: 日本語 / English / Español / 中文 / 한국어(設定画面から切り替え可能)。

## ファイル構成

```
index.html   ページ本体(HTML/CSS/JSすべて内包)
audio/       タップ音・カウントダウン音などのサウンドファイル置き場(未追加)
```

## 音声ファイルについて(TODO)

`index.html` は以下の音声ファイルを `audio/` フォルダから読み込む想定で作られていますが、現時点ではまだ配置されていません。

- `audio/click.wav`
- `audio/bass.wav`
- `audio/pop.wav`
- `audio/tone.wav`
- `audio/wrong.wav`
- `audio/countdown.wav`

音声ファイルが無くても、再生に失敗するだけでゲーム自体は問題なく動作します(無音になるだけ)。あとから同名のファイルを `audio/` フォルダに追加すれば、そのまま音が鳴るようになります。

## GitHub Pages での公開

1. リポジトリの Settings → Pages を開く
2. Source を「Deploy from a branch」、Branch を `main` / `/(root)` に設定
3. 数分後に `https://<ユーザー名>.github.io/1to10/` で公開されます

現在このリポジトリは Private のまま準備を進めています。公開の合図があり次第、Public化 と Pages の有効化を行います。
