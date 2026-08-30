# GOSAMARU ESTATE / Astro

護佐丸エステートの静的サイトをAstro構成へ移行するための土台です。

## 構成

- `src/layouts/BaseLayout.astro` : `<html>`, `<head>`, Header, Footer の共通レイアウト
- `src/components/Header.astro` : 共通ヘッダー
- `src/components/Footer.astro` : 共通フッター
- `src/components/SectionTitle.astro` : 共通セクション見出し
- `src/components/PageVisual.astro` : 下層ページのメインビジュアル
- `src/pages/` : 各ページ
- `src/styles/global.css` : 共通CSS
- `public/images/` : 画像・アイコン

## 起動

```bash
npm install
npm run dev
```

## 本番ビルド

```bash
npm run build
```

`dist/` に静的ファイルが生成されます。

## 注意

お問い合わせフォームの `action` は `/contact-confirm.php` にしています。
PHP側の確認画面・送信処理は別途作成してください。

現在のHTML原稿に存在しない画像や各下層ページの本文は、仮のパス・プレースホルダーになっています。
