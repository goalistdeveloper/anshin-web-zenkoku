# anshin-web-zenkoku
全国版 安診WebHP

## ファイル構成

```
index.html            LP本体（マークアップのみ）
assets/css/           スタイルシート（index.html で読み込み順に注意）
  ├ variables.css     デザイントークン（色・角丸）。配色変更はここだけ
  ├ base.css          リセット・基本タイポグラフィ・ユーティリティ
  ├ layout.css        コンテナ・ヘッダー・フッター・スマホ固定CTAバー
  ├ components.css    ボタン・ラベル・テーブル・フォームなど共通部品
  └ sections.css      S1〜S11 の各セクション固有スタイル
assets/img/           画像・動画
docs/                 企画資料・配布資料
```

CSSは上記の順に読み込んでいます。後ろのファイルほど優先されるため、
`<link>` の並び順を入れ替えると表示が崩れる場合があります。
