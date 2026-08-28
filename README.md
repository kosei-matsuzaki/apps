# apps

個人開発しているスマホアプリの**公開ページ置き場**。
GitHub Pages で配信しています。

<https://kosei-matsuzaki.github.io/apps/>

App Store / Google Play には**公開されたURL**を出す必要があるため、
アプリのリポジトリ（private）とは別に、ここだけを公開しています。

## 中身

```
index.html              アプリの一覧
tsumiage/privacy.html   ツミアゲ プライバシーポリシー
tabishiori/privacy.html タビシオリ プライバシーポリシー
.nojekyll               Jekyll を通さない（そのまま配信する）
```

## 直し方

**ここのHTMLを直接書き換えないでください。**
原本は各アプリのリポジトリにあり、そこから作り直します。

| アプリ | 原本 | 作り直すコマンド |
|---|---|---|
| タビシオリ | `tabishiori/docs/privacy_policy.md` | `python3 tools/build_privacy_page.py` |
| ツミアゲ | `tsumiage/docs/` 配下 | （そのリポジトリの手順に従う） |

作り直した HTML をここへコピーして push すると、1〜2分で反映されます。

## 注意

- **ツミアゲ v1.0.0（公開中）のアプリ内リンクは
  `https://kosei-matsuzaki.github.io/tsumiage-bgm/privacy.html` を指しています。**
  そちらのページはそのまま残してあります。
  次のアップデート（v1.1.0）で `support.dart` の URL をここへ向け、
  移行が済んだら旧ページを畳みます
- BGM の配信は引き続き `tsumiage-bgm` リポジトリの Releases から行っています
  （こちらは移していません）
