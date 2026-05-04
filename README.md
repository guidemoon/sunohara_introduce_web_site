# 春原 衛 ポートフォリオサイト

新しい方への自己紹介を目的とした、シングルページのポートフォリオサイトです。

公開URL: `https://guidemoon.github.io/portfolio/`(デプロイ後に有効)

---

## ファイル構成

```
portfolio/
├── index.html       # サイト本体(HTML、CSS、JavaScriptをすべて内包)
└── README.md        # このファイル
```

外部依存はGoogle Fonts(Noto Sans JP / JetBrains Mono)のみです。
画像、フレームワーク、ビルドツールは不要で、`index.html` を開けばそのまま動作します。

---

## サイトの構成

縦スクロール1ページの構成です。

| セクション | 内容 |
|---|---|
| HEADER | 名前、ポートフォリオ年 |
| HERO | キャッチコピー、自己紹介の要約、タグ |
| ABOUT | これまでの経歴の物語 |
| CAPABILITIES | 提供できる3つの価値 |
| EXPERIENCE | 職歴の時系列(Artriam、Noe Labo、過去の所属を含む) |
| SKILLS | 技術 / ビジネス / 業界知見 / 資格 |
| HOBBIES | 仕事以外の活動 |
| CONTACT | SNSへのリンク |
| FOOTER | コピーライト |

---

## デザイン方針

- 日本語メインのサンセリフ体(Noto Sans JP)で読みやすさを優先
- 白を基調にした高コントラストなシンプルデザイン
- アクセントカラーは青(#1d4ed8)1色のみ
- 装飾を抑えて、内容に集中できる構成
- スマートフォン・タブレット・PCに対応(レスポンシブ)

---

## ローカルでの確認

ブラウザで`index.html`をダブルクリックするだけで確認できます。

```bash
# macOS
open index.html

# Windows
start index.html
```

ファイルをブラウザにドラッグ&ドロップしても確認可能です。

---

## GitHub Pagesへの公開手順

### 1. GitHubリポジトリを作成

GitHubにログインして、新しいリポジトリを作成します。

- リポジトリ名: `portfolio`(任意)
- 公開設定: Public
- READMEファイルの自動作成: 不要

### 2. ローカルからリポジトリへPush

```bash
cd portfolio
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/guidemoon/portfolio.git
git push -u origin main
```

### 3. GitHub Pagesを有効化

1. リポジトリのページで `Settings` をクリック
2. 左メニューから `Pages` を選択
3. `Source` で `Deploy from a branch` を選択
4. Branch を `main`、フォルダを `/ (root)` に設定
5. `Save` をクリック

数分後、 `https://guidemoon.github.io/portfolio/` のようなURLでサイトが公開されます。

### 4. 公開URLの確認

`Settings → Pages` のページに、公開URLが表示されます。

---

## カスタムドメインを設定する場合

独自ドメインを使いたい場合は以下を行います。

1. リポジトリのトップに `CNAME` ファイルを作成し、ドメイン名のみを記載
2. ドメインのDNS設定でAレコードまたはCNAMEレコードをGitHub Pagesに向ける
3. GitHub Pagesの設定画面でカスタムドメインを入力

詳細はGitHub Pages公式ドキュメントを参照してください。

---

## 内容の更新方法

`index.html` を直接編集して、コミット・プッシュすれば数分で反映されます。

```bash
# 編集後
git add index.html
git commit -m "Update content"
git push
```

### よくある更新

| 更新内容 | 編集箇所(検索キーワード) |
|---|---|
| Heroのキャッチコピー | `<h1>ヘルスケアの現場課題を` |
| 自己紹介文 | `<div class="about-body">` |
| 経歴の追加・更新 | `<div class="experience-list">` |
| スキルの追加・削除 | `<div class="skills-grid">` |
| SNSリンクのURL変更 | `class="social-icon"` |
| Instagram/YouTube有効化 | `class="social-icon disabled"` を `class="social-icon"` に変更し、`<span>` を `<a href="...">` に書き換え |

---

## SEO設定について

このサイトは `<meta name="robots" content="noindex, nofollow">` を設定しているため、検索エンジンのインデックス対象外です。
URLを知っている人だけが閲覧できる状態になっています。

検索エンジンに表示させたい場合は、`<head>` 内のこの行を削除します。

---

## 連絡先

- X: [@sunoharamamoru](https://x.com/sunoharamamoru)
- Facebook: [プロフィール](https://www.facebook.com/profile.php?id=61576617264653)
- LinkedIn: [プロフィール](https://www.linkedin.com/in/%E8%A1%9B-%E6%98%A5%E5%8E%9F-6a7015373/)
- note: [@sunohara_mamoru](https://note.com/sunohara_mamoru)
- GitHub: [@guidemoon](https://github.com/guidemoon)
- Qiita: [@haru4989](https://qiita.com/haru4989)

---

## 関連サイト

- 株式会社Artriam: [artriam.com](https://artriam.com)
- Noe Labo(個人事業): [noe-labo.com](https://noe-labo.com)

---

© 2026 春原 衛 / Mamoru Sunohara
