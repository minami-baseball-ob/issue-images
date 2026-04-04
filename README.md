# issue-images

フィードバック・バグ報告用の画像ストレージ。

## 仕組み

[OB会サイト](https://minami-baseball-ob.vercel.app/)のフッター・aboutページにあるGoogleフォームから送信された画像が、Google Apps Script経由でこのリポジトリに自動保存されます。

```
OBメンバー → Googleフォーム（カテゴリ・内容・画像）
         ↓
Google Apps Script → GitHub Contents API
         ↓
このリポジトリに画像コミット → GitHub Issue本文にMarkdown埋め込み
```

## 関連リポジトリ

- [minami-baseball-ob](https://github.com/yasumorishima/minami-baseball-ob)（private） — OB会サイト本体
- [minami-baseball-ob-docs](https://github.com/yasumorishima/minami-baseball-ob-docs) — 技術解説
- [masters-docs](https://github.com/yasumorishima/masters-docs) — マスターズ甲子園大会資料
