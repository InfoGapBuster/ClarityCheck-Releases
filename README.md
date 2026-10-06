# ClarityCheck

会議や発表の音声・字幕から「情報の伝わりやすさ」をローカル解析するmacOSアプリです。人事評価・採用・人物の能力判定には使用しません。

## ダウンロード

**[最新版をダウンロード](https://github.com/InfoGapBuster/ClarityCheck-Releases/releases/latest)** · [修正履歴](CHANGELOG.md)

Apple Silicon搭載Mac、macOS 14以降が対象です。macOS 27.0.1で動作確認しています。

1. 最新リリースの `ClarityCheck-vX.Y.Z-macOS-arm64.zip` をダウンロードして展開します。
2. ClarityCheck.appを「アプリケーション」フォルダへコピーします。
3. 更新するときは旧版を終了してからアプリを差し替えます。

Developer ID署名・Appleによる公証は未実施です。macOSが初回起動をブロックする場合があります。

## 更新確認

アプリの「ClarityCheck」メニュー →「アップデートを確認…」で最新版の有無を確認できます。起動時にも新しい版がある場合に通知します。「修正履歴を見る」で変更内容を確認できます。更新は配布ページからの手動ダウンロードです。

更新確認は公開GitHub APIへバージョンを問い合わせます。音声・字幕・分析結果を送信しません。オフラインでもローカル解析は利用できます。

## データと検証

データ保存先: `~/Library/Application Support/claritycheck-desktop/data`。アプリの差し替えでは削除されません。元データは解析後、結果は通常24時間以内の保存期限に従って削除します。

リリースには `SHA256SUMS.txt` を添付しています。ZIPと同じフォルダで `shasum -a 256 -c SHA256SUMS.txt` を実行して確認できます。

## このリポジトリについて

公開するのは配布アプリ、利用案内、修正履歴です。アプリのソースは非公開の別リポジトリで管理しています。リリースに自動表示される「Source code」は、この配布用リポジトリの案内ファイルのみです。
