# ねこ見守り v1.7 — インストールブロックの確認資料

**この文書は Google Play プロテクトへの説明用です。Google による安全認定を意味しません。**

## アプリの情報
- アプリ名: ねこ見守り テスト
- Android パッケージ名: `jp.nekowatch.monitor`
- バージョン: `1.7-screen-share-test` / `versionCode 3`
- APK: [v1.7 試験版 APK](https://raw.githubusercontent.com/sui-0825/neko-watch-apk/main/neko-watch-v1.7-test.apk)
- ファイル SHA-256: `001037ee672801eb0da095e79de0629fcd98780fc5529f35e9db4b4ea1318eef`

## 機能と権限
この APK は開発段階のローカル画面色判定テストです。Android の MediaProjection により、毎回ユーザーが画面共有を許可した後に画面フレームを読み、指定範囲に黄色があるかを端末上で判定し、その状態を小窓に表示します。

Android 標準の画面共有と小窓表示に必要な以下の権限を使います。
- `FOREGROUND_SERVICE`
- `FOREGROUND_SERVICE_MEDIA_PROJECTION`
- `SYSTEM_ALERT_WINDOW`
- `POST_NOTIFICATIONS`

**使用しない権限:** `INTERNET`, `BIND_ACCESSIBILITY_SERVICE` / ユーザー補助サービス, SMS, 連絡先。

**未実装の機能:** 自動タップ・自動スクロール・黄色の回転速度の検出・猫の縮小検出。画面画像をファイルに保存したり、サーバーへ送信したりする処理はありません。

## 現在の状況
Google Play ストアには公開せず、所有者の Android テスト端末に APK をサイドロードする方式を検証中です。端末で Google Play プロテクトから「デバイスを保護するため、アプリをブロックしました」「このデベロッパーのアプリは Play プロテクトにスキャンされたことがありません」と表示され、インストールが停止しました。

現在は実機テストを停止しています。Play プロテクトの無効化や警告回避は推奨しません。正式な確認・再審査を希望します。

## 注意点
この APK は **Android Debug 署名**による技術検証版であり、製品版ではありません。署名はAPKの形式的な完全性を示すだけで、悪意ある挙動がないことや Google からの承認を意味しません。
