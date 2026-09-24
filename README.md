# aliba コーポレートサイト

静的HTMLをGitHubのmainブランチからVercelへ公開します。

## 2026-09-24の変更

- ホームの制作事業カードを同じ高さにし、アプリ制作の紹介画像を追加。
- services/apps/ に公開中2アプリの実際のアイコン・プレイ画像と公式App Storeバッジを掲載。
- images/business-apps-20260924-v3.png は事業紹介用の生成イメージ。公開中アプリの実画面とは別。
- 実画像はAppleの公開iTunes Lookup APIで確認した各アプリのアセット。ID: 6809498156、6811368161。
- App StoreバッジはApple公式配布SVGを変更せず利用。
- privacy、personal-info、apps、contact の説明を実装済み／予定の区別と実際のフォーム構成に合わせて更新。

## 確認

ローカルプレビュー: python -m http.server 8767
PC 1280px・スマホ390pxで画像表示、カード高さ、メニュー、アプリ紹介への遷移、App Storeリンクを確認。
実機の広告SDK・同意動作とApp Storeのプライバシー申告は別途確認が必要。
app-ads.txtは既存行を維持し、承認された7行を追加済み。

## 参照

- https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg
- https://developer.apple.com/app-store/marketing/guidelines/
- https://developer.apple.com/app-store/user-privacy-and-data-use/
- https://unity.com/legal/game-player-and-app-user-privacy-policy
