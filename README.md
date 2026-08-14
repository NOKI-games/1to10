# 1 TO 10 ⚡

**[▶ 今すぐプレイ / Play now](https://noki-games.github.io/1to10/)**

1から指定した数字まで、画面に散らばった数字を順番にタップしていくスピードゲームです。ルールは単純、でもハイスコアを狙うと止まらなくなる中毒性。単一の `index.html` で完結する静的サイトなので、GitHub Pages でそのまま公開・プレイできます。インストール不要、無料。

## 遊び方

- ホーム画面のスライダー／±ボタンで、最後の数字(2〜20)を設定します。
- STARTを押すと3秒のカウントダウン後にゲーム開始。
- 1から設定した数字まで、順番にタップします。
- 間違った順番でタップすると0.35秒のペナルティが加算されます。
- タイムに応じて S / A / B / C / D のランクが表示されます。
- 結果とベストタイムは、設定ごとに自動保存されます(YouTube Playables環境ではプラットフォームのセーブAPI、それ以外はブラウザのlocalStorageを使用)。

対応言語: 日本語 / English / Español / 中文 / 한국어(設定画面から切り替え可能)。
対応環境: PC(マウス)・Android・iPhone(タッチ)すべてに対応したレスポンシブデザイン。

## アプリのようにインストールする(PWA)

ストアを経由せず、ホーム画面にアイコンを追加してアプリのように起動・オフライン再生できます。

- **Android(Chrome)**: サイトを開き、メニュー(⋮)→「アプリをインストール」または「ホーム画面に追加」
- **iPhone(Safari)**: サイトを開き、共有ボタン(□に↑)→「ホーム画面に追加」

一度開いておけば、通信が不安定な場所でもオフラインでプレイできます(Service Worker によるキャッシュ)。

## ファイル構成

```
index.html            ページ本体(HTML/CSS/JSすべて内包)
manifest.json         PWA用マニフェスト(ホーム画面追加・アプリ名・アイコン設定)
sw.js                 Service Worker(オフラインキャッシュ)
audio/                タップ音・カウントダウン音などのサウンドファイル
favicon.ico           ファビコン
icon-180.png          Apple touch icon(ホーム画面アイコン用)
icon-192.png          PWAアイコン(通常)
icon-512.png          PWAアイコン(通常・大)
icon-512-maskable.png PWAアイコン(Android アダプティブアイコン用)
og-image.png          SNSシェア用のプレビュー画像(OGP)
```

## GitHub Pages での公開

1. リポジトリの Settings → Pages を開く
2. Source を「Deploy from a branch」、Branch を `main` / `/(root)` に設定
3. 数分後に `https://noki-games.github.io/1to10/` で公開されます

現在このリポジトリは **Public** で公開中です。上のリンクからすぐにプレイできます。
