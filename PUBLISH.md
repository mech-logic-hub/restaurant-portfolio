# 公開リポジトリへの切り出し手順

このフォルダを **公開リポジトリ `restaurant-portfolio`** として独立させます。
本リポジトリ（非公開）には制作サンプルを残しません。

## 1. GitHub で空リポジトリを作成

1. https://github.com/new を開く
2. 設定:
   - **Repository name**: `restaurant-portfolio`
   - **Public**
   - README / .gitignore / license は **追加しない**（空のまま）
3. **Create repository**

## 2. このフォルダを push

```bash
cd restaurant-portfolio
git init -b main
git add -A
git commit -m "feat: 飲食店 LP サンプル初版"
git remote add origin https://github.com/mech-logic-hub/restaurant-portfolio.git
git push -u origin main
```

## 3. GitHub Pages を有効化

1. 新リポジトリの **Settings → Pages**
2. **Source**: GitHub Actions
3. Actions タブで `Deploy GitHub Pages` が成功するのを待つ

公開 URL:

```
https://mech-logic-hub.github.io/restaurant-portfolio/
```

## 4. 本リポジトリからこのフォルダを削除

公開確認後、life-log 側で `restaurant-portfolio/` を削除して commit してください。

## 現在の内容

| サンプル | パス |
|----------|------|
| 温かみ | `/warm/` |
| 和モダン | `/wa-modern/` |
| 町食堂 | `/machi-shokudo/` |

サンプル店名は **まちの灯食堂**（架空）。副業・検証用の固有名詞は含みません。
