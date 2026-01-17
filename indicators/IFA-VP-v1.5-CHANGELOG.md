# IFA-VP Context v1.5 変更点サマリー

## v1.4 → v1.5 主な変更

### 1. ロジック整合

| 項目 | v1.4 | v1.5 | 理由 |
|------|------|------|------|
| 変数宣言 | `var string`で毎バー上書き | `string`のみ（varなし） | 冗長性排除 |
| Score計算 | `var int`+`:= 0`リセット | `int`で毎バー新規 | 明確性向上 |
| VP計算 | インライン | `calcVolumeProfile()`関数化 | 可読性・再利用性 |

### 2. input整理

| 項目 | v1.4 | v1.5 |
|------|------|------|
| 命名規則 | `ui_*`, `vp_*`混在 | `i_*`で統一 |
| グループ定数 | 文字列直書き | `GROUP_*`定数 |
| tooltip | 一部のみ | 全項目に追加 |

### 3. 命名統一

| カテゴリ | v1.4 | v1.5 |
|----------|------|------|
| 描画オブジェクト | `ui_poc_line` | `linePoc` |
| 計算結果 | `core_poc_price` | `pocPrice` |
| ステータス | `core_context_bias` | `contextBias` |

### 4. コメント
- 全コメントを英語に統一（TradingView公開用）
- セクション区切りを明確化（`//===`）
- 各セクションの役割を明記

### 5. リペイント対策（確認済み）

| 計算 | タイミング | リペイント |
|------|------------|-----------|
| SMA | 毎バー | なし（過去値固定） |
| SMA Cross | `ta.crossover` | なし（確定後） |
| VP計算 | `barstate.isconfirmed` | なし |
| Context Score | 毎バー（VP値参照） | なし（VP確定後） |
| POC Enter | 毎バー判定 | なし（状態機械） |

---

## 明日の案件作業用 差分メモ

### Abraham案件（ICT/SMT/Box）との切り替え点

IFA-VP v1.5のコードを案件用に改造する場合の差分ポイント：

#### 1. 共通で使える部分
```
- Core計算の枠組み（ATR、SMA計算）
- 描画オブジェクトの事前確保パターン
- barstate.isconfirmed/islastの分離
- テーブル表示の構造
```

#### 2. 案件で変更が必要な部分
```
- VP計算 → ICT構造検出（BOS/CHoCH/Sweep）に置換
- Context Score → SMTスコア計算に置換
- POC/VA → FVG/OB/Liquidity Zoneに置換
- Badge → シグナル表示（ただしBUY/SELL注意）
```

#### 3. 案件Milestone1の範囲（仕様確定後）
```
- signals: Entry/Exitの条件表示
- alerts: アラート条件（TradingView設定用）
- testing: バーリプレイでの動作確認
- 自動執行は含めない
```

#### 4. 切り替え手順（案件開始時）
```
1. IFA-VP-v1.5.pineをコピー
2. ファイル名を案件用に変更
3. VP計算部分をICT計算に置換
4. 描画部分を案件要件に合わせて変更
5. アラート条件を案件仕様に合わせる
```

---

## ファイル一覧

| ファイル | 内容 |
|----------|------|
| `IFA-VP-Context-v1.5.pine` | 本体コード（完成版） |
| `IFA-VP-v1.5-CHECKLIST.md` | 動作確認チェックリスト |
| `IFA-VP-v1.5-CHANGELOG.md` | このファイル |

---

## TradingView公開準備

### 公開時のDescription（別途作成済み）
- 英語版: 案件引き継ぎドキュメントに記載

### 公開前の最終確認
- [ ] コンパイルエラーなし
- [ ] 警告最小限
- [ ] チェックリスト完了
- [ ] スクリーンショット準備
