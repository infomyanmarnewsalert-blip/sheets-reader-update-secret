# sheets-reader

- バッチング：スプレッドシートで最初の編集を検知してから 5 分後に 1 回だけ起動（5 分内の複数編集をまとめる）
- 差分の算出：GAS 側で added_emails / removed_emails / total_count を計算して payload に同梱
- Secret 更新：Actions 側で最新のシート内容を再読込し、カンマ区切り文字列を Secret に反映
