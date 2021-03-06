Mobage ShellApp SDK Sample Application
================================================================================


サンプルアプリケーションについて
--------------------------------------------------------------------------------
Mobage ShellApp SDKを利用したゲームアプリケーションの雛形として利用できるサンプルコードです。


注意事項
--------------------------------------------------------------------------------
本サンプルの動作を確認するには、別途PHPサーバーをご用意頂き
SDKに同梱のサーバー側サンプルコードを動作させて頂く必要があります。


セットアップ
--------------------------------------------------------------------------------
### 共通
パートナーデベロッパーサイトにおいて

- sandboxのアプリケーション
- アプリケーションにログインするためのテストユーザー

の登録を行ってください。

アプリケーションを登録する際、「利用するSDK」は「ShellApp SDK」を選択するようにしてください。
一度登録すると変更できませんので、ご注意ください。

### Android
`android/README.md`を参照してください。

### iOS
`ios/README.md`を参照してください。


サンプルコードのその他機能
--------------------------------------------------------------------------------
本サンプルコードでは、Mobage ShellApp SDKの機能とは別に
ゲーム開発に役立つと思われる機能および、セキュリティ向上のための機能を搭載しています。

### サウンド機能
Native機能を利用した簡易的なBGM・SE再生機能があります。
カスタムブリッジメソッドを提供しているため、JavaScriptからBGM・SEの再生指示ができます。
提供しているJavaScript APIは以下のものです。詳細はプログラミングガイドを参照ください。
```
sdksample.Music.play()
sdksample.Music.pause()
sdksample.Music.resume();
sdksample.Music.stop();
sdksample.SoundEffect.play();
```

### ドメインホワイトリスト機能
WebViewで任意のサイトを開くことができてしまう状態はセキュリティ上問題があるため、
ホワイトリストに含まれるドメインのみを開くようにする機能が組み込まれています。

参考
--------------------------------------------------------------------------------
- [プログラミングガイド](https://docs.mobage.com/display/JPJSSDK/NBPF+Home)
