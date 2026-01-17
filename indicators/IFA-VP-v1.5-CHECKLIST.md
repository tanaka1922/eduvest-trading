# IFA-VP Context v1.5 動作確認チェックリスト

## コンパイル確認
- [ ] TradingViewで貼り付けてコンパイルエラーなし
- [ ] 警告が最小限（意図的なもの以外なし）

## 表示確認（各モード）

### Minimal Mode
- [ ] SMA 20/50/200 ラインが表示される
- [ ] POC/VAH/VAL ラインが表示される
- [ ] 価格ラベルが表示される
- [ ] VA帯塗り・Context Badge は非表示
- [ ] テーブルが表示される

### Impact Mode
- [ ] 上記に加えて VA帯塗り（紫）
- [ ] POC Zone（オレンジ帯）
- [ ] Trend Ribbon（SMA20-50間の塗り）
- [ ] Context Badge（🟢/🔴/⚪/⚠️）
- [ ] Context Heat（Score>=70で背景グロー）
- [ ] POC Reaction Badge（ENTER/IN/EXIT）
- [ ] Cross Pulse（クロス後の小さい丸）

### Pro Mode
- [ ] Impact + VP Full横棒ヒストグラム
- [ ] HVN/LVN の色分け

## リペイント確認（バーリプレイ）
- [ ] SMA Cross: 確定バーでのみ表示、過去に遡って変化しない
- [ ] POC/VAH/VAL: 確定バーでのみ更新
- [ ] Context Badge: 確定バーでのみ状態変化
- [ ] POC Reaction: 確定バーでのみENTER判定

## アラート確認
- [ ] POC Enter: POCゾーンに入った時に発火
- [ ] Uptrend Start (GC 20×50): クロス時に発火
- [ ] Downtrend Start (DC 20×50): クロス時に発火
- [ ] MAJOR Uptrend (GC 50×200): クロス時に発火
- [ ] MAJOR Downtrend (DC 50×200): クロス時に発火
- [ ] Context Change: LONG/SHORT FAVORABLEに変化時に発火
- [ ] Long Favorable: 条件成立時に発火
- [ ] Short Favorable: 条件成立時に発火

## テーブル確認
- [ ] STATUS行: 正しいステータスとアイコン
- [ ] Score行: 0-100の範囲、Strong/Moderate/Weak表示
- [ ] Zone行: Above VAH/Below VAL/At POC/In VA
- [ ] Trend行: BULL/BEAR/FLAT + SMA順序
- [ ] POC行: ENTER/IN/EXIT/OUT
- [ ] Hint行: 状況に応じたガイダンス
- [ ] Version行: v1.5 + モード名

## 設定変更確認
- [ ] SMA色変更 → 即時反映
- [ ] POC/VA色変更 → 即時反映
- [ ] VP Lookback変更 → 次のバー確定で反映
- [ ] VP Rows変更 → 横棒数が変わる（Pro mode）
- [ ] Badge Size変更 → 即時反映

## パフォーマンス確認
- [ ] チャート読み込みが遅くない
- [ ] スクロールがスムーズ
- [ ] タイムフレーム切替が遅くない
