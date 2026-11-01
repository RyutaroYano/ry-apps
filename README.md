# ry-apps

個人用のウェブアプリ置き場。ビルドステップなしの静的サイト（素のHTML/CSS/JavaScript）で、GitHub Pagesで公開している。

公開URL: https://apps.ryutaroyano.jp/

## アプリ

- [`gamification.html`](gamification.html): ゲーミフィケーション自己報酬アプリ。やったことで点数をためて、サイコロで報酬を引く。データはGoogle Apps Scriptの先のGoogleドライブ／スプレッドシートに保存し、合言葉で守っている。

## 設計上の約束

- **罰則なし設計**: やらなかったことによる減点機能は追加しない。
- **オフラインファースト**: `localStorage` を正とし、GASへは未送信分を溜めて送り直す方式で同期する。
- **合言葉などの秘密情報はこのリポジトリに置かない**（このリポジトリは公開）。
