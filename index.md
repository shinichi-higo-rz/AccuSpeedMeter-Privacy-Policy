---
title: "AccuSpeedMeter (ASM) Privacy Policy"
description: "AccuSpeedMeter privacy policy in Japanese and English"
lang: en
---

# AccuSpeedMeter (ASM) Privacy Policy

**公開前の最終確認中 / Final review before publication**  
**Effective date / 発効日:** To be confirmed before publication  
**Last updated / 最終更新日:** 2026-10-31

## English

### 1. Scope
This policy describes how AccuSpeedMeter (ASM) handles information. Separate terms and privacy policies may also apply to third-party services such as Google Maps, Android, data providers, and destinations selected by the user for sharing.

### 2. Information handled
Depending on the features used and permissions granted, ASM handles the following information on the device:

- **Location and measurement data:** latitude, longitude, time, speed, distance, elevation, and accuracy.
- **GNSS data:** satellite identifiers, signal strength, positioning, satellite and measurement logs, and navigation messages.
- **Session and settings data:** measurement start/end times and locations, session identifiers, recording state, and app settings.
- **Voice memos:** audio recorded at the user's request, recording time, session association, and recording location.
- **Diagnostic information:** logs used to troubleshoot app behavior. Depending on settings and export options, logs may contain technical information and location- or session-related information.
- **External-service settings:** an OpenWeather API key if configured by the user. The key is encrypted for on-device storage using an Android Keystore-managed key. The key is excluded from ASM's settings backup/export and, in the current Android backup rules, its encrypted SharedPreferences file is excluded from cloud backup and device transfer.

### 3. Purposes and on-device storage
Information is used to display speed, distance, elevation and satellite information; save and review measurement history; record and play voice memos; retrieve and cache elevation data; export or share information at the user's request; and troubleshoot the app.

Measurement history and GNSS logs are stored in the app database or similar storage. Voice memos are stored in app-specific internal storage. Elevation data may be cached. Information may remain on the device until the user deletes it in the app.

### 4. External services
Depending on the feature, settings and region, ASM sends requests to:

- **Geospatial Information Authority of Japan (GSI):** elevation tiles for Japan. Requests use tile identifiers derived from the target location, which can reveal the approximate area being queried.
- **Copernicus DEM distribution services:** elevation tiles outside Japan. Requests use tile identifiers derived from the target location, which can reveal the approximate area being queried.
- **Japan Meteorological Agency (JMA):** sea-level pressure and AMeDAS-related data. The app downloads the station table, latest observation time, and observation map; it selects a nearby station locally using the device location, and the current request URLs do not include the user's coordinates.
- **OpenWeather:** if enabled and configured with an API key, requests containing latitude, longitude and the API key are sent to retrieve pressure data.
- **Google Maps, Street View and related services:** the Google Maps SDK/services communicate to display maps and panoramas. Depending on the SDK version and use, Google may automatically collect request metadata (such as device/OS and SDK version information), IP address, a pseudonymous SDK identifier, crash metrics and stack traces, and certain interaction data. The SDK may also process the coordinates supplied for the requested map or panorama.
- **Place-name lookup (Android Geocoder):** when resolving names for recorded locations, coordinates may be processed by Android or its provider depending on the device's Geocoder implementation and service configuration.
- **Android and user-selected sharing destinations:** when OS backup/device transfer, file selection or sharing features are used, the operating system or selected destination may process the relevant information.

Each provider's own terms and privacy policy govern its handling of information. This policy will be updated if provider behavior or ASM implementation changes.

### 5. Transfers to the developer and third parties
At the time this policy was prepared, no feature was identified that automatically sends measurement history or voice memos to a server operated by the ASM developer. Requests to external data providers and map services occur as needed to provide the features described above.

When the user exports or shares a file, it is passed to the storage location or app selected by the user. Subsequent handling is governed by the destination's policies and settings.

### 6. Export, diagnostics and backup
GNSS session exports may include location, time, satellite information and measurement logs from the selected session. Diagnostic logs may contain device environment, settings, operational events and, in some cases, location- or session-related information. Review the file and destination before sharing or saving it.

Android backup and device-transfer behavior depends on the OS version, device and user settings. ASM's current rules exclude the elevation-cache database and the encrypted OpenWeather API-key preferences file from cloud backup and device transfer; this does not mean all other app data is excluded.

### 7. Permissions
Location is used for measurement and location display; the microphone is used for voice memos initiated by the user; and the camera is used by camera-related features. Notifications and internet access are used where needed. Permissions can be changed in device settings, but denying or revoking a permission may make related features unavailable.

### 8. Retention, deletion and security
Delete measurement history and voice memos through the app where deletion controls are provided. Exported files and copies stored by sharing destinations are not removed when data is deleted in ASM. Clearing app data or uninstalling the app may cause loss of data that has not been backed up.

The developer takes information protection into consideration but cannot guarantee complete security across all environments, including devices, OS backups, sharing destinations and external services. Use care when sharing location history or audio.

### 9. Children's use
Minors should consult a parent or guardian and take care when storing or sharing location information, movement history and recordings.

### 10. Changes
This policy may be updated as features, external services or laws change. After publication, the latest version will be available at the public URL listed below.

### 11. Contact
Privacy inquiries: **accuspeedmetersupport@gmail.com**

---

---

## Japanese

### 1. 適用範囲
本ポリシーは、AccuSpeedMeter（ASM）アプリが情報をどのように取り扱うかを説明します。Google Maps、Android、データ提供元、利用者が選択する共有先などの第三者サービスには、それぞれの規約・プライバシーポリシーも適用されます。

### 2. 取り扱う情報
利用する機能と許可設定に応じて、ASMは次の情報を端末上で扱います。

- **位置・計測情報：** 緯度・経度、時刻、速度、距離、標高、精度など。
- **GNSS情報：** 衛星識別情報、受信信号強度、測位・衛星・測定ログ、ナビゲーションメッセージなど。
- **セッション・設定情報：** 計測の開始・終了時刻、開始・終了地点、セッション識別子、記録状態、アプリ設定など。
- **音声メモ：** 利用者が録音を開始した場合の音声ファイル、録音時刻、セッションとの関連付け、録音地点情報。
- **診断情報：** アプリの動作や障害の調査に使うログ。ログには技術情報や、設定・ログ出力オプションによって位置・セッションに関する情報が含まれる場合があります。
- **外部サービス用の設定：** 利用者が設定した場合のOpenWeather APIキー。キーはAndroid Keystoreで管理される鍵を用いて暗号化し、端末内に保存します。ASM独自の設定バックアップ／エクスポートには含めず、現在のAndroidバックアップ設定でも暗号化された設定ファイルをクラウドバックアップおよび端末移行の対象から除外しています。

### 3. 利用目的と端末内保存
情報は、速度・距離・標高・衛星情報の表示、計測履歴の保存と振り返り、音声メモの録音・再生、標高データの取得・キャッシュ、利用者が開始するエクスポート／共有、動作確認・障害調査のために利用します。

計測履歴やGNSSログはアプリのデータベース等に保存します。音声メモはアプリ専用の内部保存領域に保存します。標高データ等はキャッシュされる場合があります。これらの情報は、利用者がアプリ内で削除するまで端末に残ることがあります。

### 4. 外部サービスへの通信
機能・設定・利用地域に応じて、ASMは以下のサービスにリクエストを送信します。

- **国土地理院（GSI）：** 日本国内の標高タイル取得。リクエストには対象地点から算出したタイル識別子が含まれるため、照会対象のおおよその地域が分かる場合があります。
- **Copernicus DEM配信サービス：** 海外の標高タイル取得。リクエストには対象地点から算出したタイル識別子が含まれるため、照会対象のおおよその地域が分かる場合があります。
- **気象庁（JMA）：** 海面気圧やアメダス関連データの取得。観測所一覧、最新の観測時刻、観測データを取得し、端末の位置を使った観測所の選択はアプリ内で行います。現在の実装では、JMAへのリクエストURLに利用者の座標は含まれません。
- **OpenWeather：** 利用者が有効化しAPIキーを設定した場合、気圧データ取得のため緯度・経度とAPIキーを含むリクエストを送信します。
- **Google Maps／Street View等：** 地図・パノラマ表示のためGoogle Maps SDK／サービスが通信します。SDKのバージョンや利用方法に応じて、端末・OS・SDKのリクエスト情報、IPアドレス、仮名化されたSDK識別子、クラッシュ指標・スタックトレース、一部の操作情報などがGoogleに自動収集される場合があります。また、表示対象として渡した座標が処理される場合があります。
- **地点名検索（Android Geocoder）：** 記録地点の名称を取得する機能では、端末のGeocoder実装・サービス構成に応じて、座標等がAndroidやその提供元で処理される場合があります。
- **Androidの機能や選択した共有先：** OSのバックアップ・端末移行、ファイル選択、共有などを利用した場合、それぞれのOS機能や選択先のサービスが情報を処理する場合があります。

各提供者による情報の取扱いは、各社の規約・プライバシーポリシーに従います。提供者の仕様やASMの実装が変更された場合、本ポリシーも更新します。

### 5. 開発者への送信・第三者提供
本ポリシー作成時点で、ASMの開発者が運営するサーバーへ計測履歴や音声メモを自動送信する機能は確認していません。外部データ提供元や地図サービスへのリクエストは、前項のとおり機能の提供に必要な範囲で発生します。

利用者がエクスポートや共有を実行した場合、作成したファイルは利用者が選択した保存先・アプリに渡ります。その後の取扱いは共有先のポリシー等に従います。

### 6. エクスポート、診断ログ、バックアップ
GNSSセッションのエクスポートには、選択したセッションの位置、時刻、衛星情報、測定ログ等が含まれる場合があります。診断ログにも端末環境、設定、動作イベント、場合によっては位置・セッション関連情報が含まれます。共有・保存する前に、ファイルの内容と保存先を確認してください。

Androidのバックアップ／端末移行は、OSのバージョン、端末、ユーザー設定に応じて動作します。ASMの現在の設定では、標高キャッシュ用データベースとOpenWeather APIキーを含む暗号化設定ファイルをクラウドバックアップおよび端末移行の対象から除外していますが、それ以外のすべてのアプリデータが対象外になることを意味しません。

### 7. 権限
位置情報は計測・位置表示などに、マイクは利用者が開始する音声メモ録音に、カメラはカメラを利用する機能に使用します。機能に応じて通知やインターネット通信も使用します。端末の設定で権限を変更できますが、権限を拒否・取り消すと関連機能が利用できない場合があります。

### 8. 保持、削除、セキュリティ
計測履歴や音声メモは、アプリ内に削除機能がある場合はそこから削除してください。エクスポート済みファイルや共有先に作られたコピーは、アプリ内で削除しても消えません。アプリデータの消去やアンインストールにより、バックアップされていないデータが失われる場合があります。

開発者は情報保護に配慮しますが、端末、OSバックアップ、共有先、外部サービスを含むすべての環境で完全な安全性を保証することはできません。位置・移動履歴や音声データの共有には注意してください。

### 9. 子どもの利用
未成年者が利用する場合は、保護者と相談のうえ、位置情報・移動履歴・録音データの保存や共有に注意してください。

### 10. ポリシーの変更
機能、外部サービス、法令等の変更に応じて本ポリシーを改定する場合があります。公開後は、下記の公開URLで最新版を提供します。

### 11. お問い合わせ
プライバシーに関する問い合わせ先：**accuspeedmetersupport@gmail.com**

---
