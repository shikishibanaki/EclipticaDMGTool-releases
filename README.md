# Ecliptica DMG Tool（配布用）

VRChat ワールド「Ecliptica」のログを **自分の PC 上だけで** 解析する、身内向け Windows ツールの **完成品置き場**です。

- **ソースコードはこのリポジトリにありません。** Release の添付 zip だけが配布物です。
- 解析対象の VRChat ログは外部へ送信しません。

## ダウンロード

1. [Latest Release](../../releases/latest) を開く
2. **`EclipticaDMGTool.zip`** を使う
3. GitHub が自動で付ける **Source code (zip)** は使わない（README だけです）

同じ Release の `SHA256SUMS.txt` でハッシュを照合してください。

```powershell
Get-FileHash -Algorithm SHA256 .\EclipticaDMGTool.zip
```

## 使い方（概要）

1. zip を、デスクトップやドキュメントなど自分が書き込めるフォルダに展開する（Program Files は不可）
2. `EclipticaDMGTool\EclipticaDMGTool.exe` を起動する
3. フォルダごと使ってください（exe 単体では動きません）

## 自動アップデート

起動時にこのリポジトリの `latest.json` だけを確認し、新しい版があればアプリの画面に知らせが出ます。
［更新する］を押したときだけ、SHA-256 を確認してから入れ替えます。ログは送信しません。

## 注意

- コード署名が無いため、Windows SmartScreen やウイルス対策が警告することがあります。ハッシュが一致していることを確認してから使ってください。
- 管理者権限は不要です。要求する改変版は使わないでください。
- 第三者から「同じ名前の exe」を受け取った場合は、この Releases のハッシュと照合してください。
