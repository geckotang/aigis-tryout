# aigis v1.1.1 のサンプルです

## ディレクトリ構成

```yaml
- aigis_config.yml # 設定ファイル
- build/           # 生成物
  - styleguide/
- src/             # スタイルガイドの元になるCSSなど
  - css/
    - style.css
    - util.css
- styleguide_assets/ # スタイルガイド自身のテンプレートファイルやCSS
  - aigis_assets/
  - template_hbs/
    - index.hbs
    - components.hbs
    - sidemenu.hbs
```

スタイルガイドに読み込ませるCSSやJSなどがあれば、`styleguide_assets/template_hbs/index.hbs`のhead部分を修正する

## コマンド

### 関連ファイルのインストール

```bash
npm i
```

### スタイルガイド生成

```bash
npm run guide
```

`./aigis_config.yml` に記述してある内容を元にスタイルガイドを生成します。

### バージョン確認

```bash
npm run aigis -- --version
```
