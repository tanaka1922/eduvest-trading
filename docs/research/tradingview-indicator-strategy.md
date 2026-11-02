# TradingViewインジケーター公開・販売戦略 Deep Research

**調査日**: 2025年11月25日

---

## 目次

1. [スクリプト公開の種類とルール](#1-スクリプト公開の種類とルール)
2. [招待制スクリプト（有料販売）の設定方法](#2-招待制スクリプト有料販売の設定方法)
3. [成功しているインジケーター開発者の事例分析](#3-成功しているインジケーター開発者の事例分析)
4. [収益化パターン](#4-収益化パターン)
5. [Pine Script投稿の審査基準](#5-pine-script投稿の審査基準)
6. [QQE系インジケーターの競合状況](#6-qqe系インジケーターの競合状況)
7. [戦略提案](#7-戦略提案)

---

## 1. スクリプト公開の種類とルール

### 公開範囲（Visibility）

| 種類 | 説明 |
|------|------|
| **Public（公開）** | 全ユーザーに表示。モデレーション対象 |
| **Private（非公開）** | 自分のみ表示。友人との共有用 |

### アクセスタイプ（Access Types）

| タイプ | コード公開 | 利用制限 | 必要アカウント | 販売可否 |
|--------|-----------|----------|---------------|---------|
| **Open-Source** | 公開 | なし | 無料 | 不可（無料のみ） |
| **Protected** | 非公開 | なし | Pro/Pro+/Premium | 不可（無料のみ） |
| **Invite-only** | 非公開 | 招待者のみ | **Premium必須** | **可能** |

### 重要ルール

- **Open-SourceとProtectedは定義上「無料」** - 課金は禁止
- **Invite-onlyのみ有料販売が可能**
- Publicの場合、公開後15分以内のみ編集・削除可能
- タイトルは**英語必須**
- **Pine Script v6**の使用を推奨

**参考**: [Script publishing rules](https://www.tradingview.com/support/solutions/43000590599-script-publishing-rules/)

---

## 2. 招待制スクリプト（有料販売）の設定方法

### 必要条件

1. **Premiumアカウント**が必須
2. **Vendor Requirements**への準拠
3. **Public invite-only**での公開が必須（Privateでの販売は**永久BANリスク**）

### レピュテーション要件

TradingViewは、ベンダーに対して**有用なコンテンツ提供による信頼構築**を求めています：

- アイデア、動画、スクリプト、コメント等で**即時的な価値を提供**
- ティーザー的コンテンツ、宣伝目的のコンテンツは禁止
- 期間限定オファーは禁止
- **勧誘行為は重大な違反**（コメント・いいね・フォローの依頼禁止）

### 価格設定方法

- TradingViewは取引に**一切関与しない**（売上手数料なし）
- 価格は**ベンダーと購入者間で直接決定**
- 説明欄での**非現実的な主張は禁止**
- 過去の成績から将来の成績を推測させる表現は禁止

### ユーザー招待の仕組み

1. チャートにインジケーターを追加
2. 「Publish indicator」をクリック
3. プライバシーと可視性設定でInvite-onlyを選択
4. 公開後、スクリプトページに**アクセス管理ボタン**が表示
5. ユーザーのTradingView IDを入力して招待

**参考**:
- [Vendor Requirements](https://www.tradingview.com/support/solutions/43000549951-vendor-requirements/)
- [Publishing invite-only scripts](https://www.tradingview.com/support/solutions/43000614617-publishing-invite-only-scripts/)

---

## 3. 成功しているインジケーター開発者の事例分析

### トップ開発者

| 開発者 | フォロワー | 特徴 |
|--------|-----------|------|
| **LuxAlgo** | 800,000+ | 最大手。包括的なインジケータースイート |
| **Zeiierman** | 多数 | 機関投資家向けツールキット（トレンド、構造、流動性分析） |
| **BigBeluga** | 多数 | モメンタム、ダイバージェンス、出来高ベースツール |
| **Flux Charts** | 多数 | マルチタイムフレームシステム（需給、プライスアクション） |
| **Loxx** | 多数 | 高度な技術的バリエーション（Adaptive、Juirk-Filtered等） |

### 成功パターン分析

#### 無料と有料の使い分け戦略

1. **無料スクリプトで信頼構築** → フォロワー獲得
2. **高品質な有料スクリプト**で収益化
3. **定期的なアップデート**で継続的な価値提供

#### フォロワー獲得方法

- **人気銘柄に焦点**: BTCUSD、Gold、EURUSD、SPX500、Oil、GBPUSD
- **人気時間軸**: 1時間足〜日足
- **質重視**: 1日5つ以上のアイデア投稿は品質低下と見なされる
- **透明性**: 事後的な勝ちトレード公開、勝ちのみの更新は避ける
- **アイデアの更新**: トレード管理の状況を継続的に共有

**参考**: [How to build a following on TradingView](https://www.tradingview.com/support/solutions/43000570846-how-to-build-a-following-on-tradingview/)

---

## 4. 収益化パターン

### TradingView内での収益化

| 方法 | 詳細 |
|------|------|
| **Invite-only販売** | Premium必須。直接販売（TradingView手数料なし） |
| **Editor's Picks報酬** | 選出されると**$100/回**（2023年4月〜） |
| **Creator Program** | 招待制。信頼されたPine Script開発者向け |
| **アフィリエイト** | Pro紹介で手数料獲得 |

### 外部プラットフォーム連携

#### Gumroad

多くの開発者がGumroadでインジケーターを販売：

- **Oracle Trading Indicator** - シグナル提供
- **OrderVibe** - エントリー、SL、TP表示
- **Ultimate TradingView Suite** - 複合ツールセット
- **Market Map PRO** - 月額/年額サブスクリプション

**販売フロー**:
1. Gumroadで商品ページ作成
2. TradingViewユーザー名を購入時に入力させる
3. 支払い確認後、Invite-onlyスクリプトにアクセス権を付与

#### その他のプラットフォーム

| プラットフォーム | 用途 |
|----------------|------|
| **NOTE（日本）** | 日本語圏向け教育コンテンツ販売 |
| **Teachable/Udemy** | トレーディング教育コース |
| **Fiverr/Upwork** | カスタムインジケーター開発受託 |
| **Patreon** | サブスクリプション型アクセス |

**参考**: [Gumroad Trading Category](https://gumroad.com/business-and-money/investing?tags=trading)

---

## 5. Pine Script投稿の審査基準

### オリジナリティ要件

- **ビルトイン機能の焼き直し禁止**
- **自動生成コード、学習教材コードの再投稿禁止**
- **クローズドソースは独自性の説明必須**（説明がなければモデレート対象）

### コード再利用ルール

| 条件 | ルール |
|------|--------|
| **オープンソース再利用** | 原作者クレジット必須 + **大幅な改善**が必要 |
| **ライブラリ使用** | オープンソース公開なら許可不要 |
| **Protected/Invite-onlyでのライブラリ使用** | **原作者の明示的許可必須** |

### 「大幅な改善」とは

以下は**改善と見なされない**：
- スタイル変更
- 入力パラメータの変更
- 変数名の変更
- コードの並べ替え
- Pine Scriptバージョン変換

### モデレーションプロセス

1. 公開後、モデレーターが審査
2. 違反があれば非表示化
3. **PineCoders**アカウントから違反内容の通知
4. 修正して再公開可能

### 説明欄の要件

- **マッシュアップの場合**: 各コンポーネントの連携理由を説明
- **英語が主要言語**（タイトルは英語必須）
- 勧誘的表現の禁止

**参考**:
- [Tips for script authors](https://www.tradingview.com/support/solutions/43000549935-tips-for-script-authors/)
- [Writing / Publishing scripts](https://www.tradingview.com/pine-script-docs/writing/publishing/)

---

## 6. QQE系インジケーターの競合状況

### QQEとは

**Qualitative Quantitative Estimation（QQE）** は、RSIを平滑化し、ATRベースのトレーリングストップラインを追加したインジケーター。

| 特徴 | 詳細 |
|------|------|
| **ベース** | RSI |
| **追加要素** | Fast/Slow ATRトレーリングストップ |
| **用途** | トレンド方向・強度の判定 |
| **利点** | RSIより滑らかで信頼性が高い |
| **欠点** | RSIベースのためダイバージェンス時に偽シグナル |

### TradingView上の人気QQEインジケーター

| インジケーター | 作者 | 特徴 |
|---------------|------|------|
| **QQE MOD** | Mihkel00 | 2つのQQEを統合、ボリンジャーバンド付き |
| **Quantitative Qualitative Estimation QQE** | KivancOzbilgic | 基本版 |
| **Adaptive QQE** | Loxx | Ehlers自己相関ドミナントサイクル搭載 |
| **Juirk-Filtered QQE Histogram** | Loxx | Juirkフィルター適用ヒストグラム版 |
| **On-Chart QQE of RSI** | Loxx | チャート上表示版 |
| **QQE of Parabolic-Weighted Velocity** | Loxx | パラボリック加重速度版 |
| **QQE signals** | colinmck | シグナル特化版 |

### 競合分析と差別化ポイント

#### 既存インジケーターの傾向

- **基本版**: シンプルなQQE実装
- **MOD版**: 複数QQEの統合、視覚的強化
- **Adaptive版**: 市場状況への適応機能
- **フィルター版**: ノイズ除去の強化

#### 差別化の機会

1. **マルチタイムフレーム対応** - 複数時間軸のQQEを一画面で
2. **アラート機能強化** - 条件カスタマイズ可能なアラート
3. **他インジケーターとの組み合わせ** - VWAP、出来高等との統合
4. **バックテスト機能** - ストラテジーとしての実装
5. **ダイバージェンス検出** - QQEの弱点を補完
6. **日本市場特化** - 日本時間セッション、日本株対応

**参考**:
- [QQE MOD](https://www.tradingview.com/script/TpUW4muw-QQE-MOD/)
- [Adaptive QQE](https://www.tradingview.com/script/GdU0SSSf-Adaptive-Qualitative-Quantitative-Estimation-QQE-Loxx/)

---

## 7. 戦略提案

### フェーズ1: 基盤構築（0-3ヶ月）

1. **無料オープンソースインジケーター公開**
   - QQEの改良版または組み合わせ版
   - 日本語解説付きで日本市場にも対応
   - 人気銘柄（BTC、Gold、EURUSD）でアイデア投稿

2. **レピュテーション構築**
   - 週2-3回のアイデア投稿
   - コミュニティへの貢献（質問回答等）
   - 既存スクリプトの更新・改善

### フェーズ2: 収益化準備（3-6ヶ月）

1. **Premiumアカウント取得**
2. **有料版の開発**
   - 無料版の高機能版
   - 独自機能追加（アラート、MTF等）
3. **外部プラットフォーム準備**
   - Gumroadアカウント設定
   - 販売ページ作成

### フェーズ3: 本格収益化（6ヶ月〜）

1. **Invite-onlyスクリプト公開**
2. **価格設定**
   - 月額: $10-30
   - 年額: $80-200
   - 永久: $200-500
3. **マーケティング**
   - TradingViewアイデアでの露出
   - X（Twitter）での発信
   - YouTube教育コンテンツ

### 推奨する差別化ポイント

| 項目 | 内容 |
|------|------|
| **技術的差別化** | QQE + VWAP + 出来高の統合 |
| **地域特化** | 日本市場向け機能（日本時間、日本株対応） |
| **UX差別化** | 初心者向けの分かりやすいUI |
| **サポート差別化** | 日本語サポート提供 |

---

## 参考リンク集

### TradingView公式

- [Script publishing rules](https://www.tradingview.com/support/solutions/43000590599-script-publishing-rules/)
- [Vendor Requirements](https://www.tradingview.com/support/solutions/43000549951-vendor-requirements/)
- [Publishing invite-only scripts](https://www.tradingview.com/support/solutions/43000614617-publishing-invite-only-scripts/)
- [Tips for script authors](https://www.tradingview.com/support/solutions/43000549935-tips-for-script-authors/)
- [How to build a following](https://www.tradingview.com/support/solutions/43000570846-how-to-build-a-following-on-tradingview/)
- [Writing / Publishing scripts](https://www.tradingview.com/pine-script-docs/writing/publishing/)

### 外部プラットフォーム

- [Gumroad Trading](https://gumroad.com/business-and-money/investing?tags=trading)

### QQE関連

- [QQE MOD by Mihkel00](https://www.tradingview.com/script/TpUW4muw-QQE-MOD/)
- [Adaptive QQE by Loxx](https://www.tradingview.com/script/GdU0SSSf-Adaptive-Qualitative-Quantitative-Estimation-QQE-Loxx/)
- [QQE by KivancOzbilgic](https://www.tradingview.com/script/0vn4HZ7O-Quantitative-Qualitative-Estimation-QQE/)

---

*本調査は2025年11月25日時点の情報に基づいています。TradingViewのポリシーは変更される可能性があるため、最新情報は公式ドキュメントを参照してください。*
