# 被害記録（人間被害マッピング）
- Case-ID: KABUKI-INV  /  Updated: 2025-09-14 11:50 UTC+0700

## L-20250612-01 — 2025-06-12 11:25  time_score=3
- device: iP15P-Ghost
- event_type: 入力妨害 / フリーズ（Jetsam 由来）
- impact: 画面操作・アプリ切替の一時不能。常駐群が同秒活性。
- log_ref: JetsamEvent-2025-06-12-112511.docx; OUT_ZIP_INTEGRATION/EVENTS.csv(bug_type=298)
- ref_diff: OUT_ZIP_INTEGRATION/tamper_join_sec.csv; OUT_ZIP_INTEGRATION/PIVOT.csv; OUT_ZIP_INTEGRATION/DIFF_events.csv
- severity: High (3)
- confidence: 0.88
- custody_capture/analysis: /mnt/data/KABUKI_INV_2025-06-12_OUT_ZIP_INTEGRATION/sha256_chain_generated.csv
- notes: CoreRepairCoreXPCService/AppleDeviceQueryService/remoted/locationpushd/Shortcuts 同秒帯活性。
- flame_flag: Apple=Yes; Microsoft=No; Meta=No; VN-Telco=?; CN-Vendor=No

## L-20250612-02 — 2025-06-12 12:05  time_score=2
- device: iP15P-Ghost
- event_type: データ再同期 / 権限・履歴の再適用（reconcile 兆候）
- impact: アプリが“既存扱い”で一括復活。通知/権限状態が短時間に変化の可能性。
- log_ref: bug_type225-2025-06-12 120519 .docx; OUT_ZIP_INTEGRATION/EVENTS.csv(bug_type=225); OUT/IDMAP.csv
- ref_diff: OUT_ZIP_INTEGRATION/PIVOT.csv; OUT_ZIP_INTEGRATION/DIFF_keywords.csv
- severity: Medium (2)
- confidence: 0.83
- custody_capture/analysis: /mnt/data/KABUKI_INV_2025-06-12_OUT_ZIP_INTEGRATION/sha256_chain_generated.csv
- notes: xp_amp_app_usage_dnu（prior install）束。com.vnp.myviettel 等を含むが“インストール爆撃”ではなく履歴合流の説明が妥当。
- flame_flag: Apple=Yes; Microsoft=No; Meta=No; VN-Telco=Yes; CN-Vendor=No

## L-20250612-03 — 2025-06-12 05:07  time_score=1
- device: iPhone 12 Ghost（推定）
- event_type: システム前処理 / バックグラウンド起動
- impact: 体感影響は不明（短時間の入力遅延・通知遅延の可能性）。
- log_ref: bug_type_202-2025-06-12-050716; OUT_ZIP_INTEGRATION/EVENTS.csv(bug_type=202)
- ref_diff: OUT_ZIP_INTEGRATION/PIVOT.csv
- severity: Low (1)
- confidence: 0.62
- custody_capture/analysis: /mnt/data/KABUKI_INV_2025-06-12_OUT_ZIP_INTEGRATION/sha256_chain_generated.csv
- notes: 6/13のサポート接触付近にも202系が継続（橋渡し）。
- flame_flag: Apple=Yes; Microsoft=No; Meta=No; VN-Telco=No; CN-Vendor=No

## L-20250612-04 — 2025-06-12 12:05  time_score=2
- device: iP15P-Ghost
- event_type: キャリアアプリ履歴の合流（補助記録）
- impact: 通知・権限状態が“既存扱い”で再評価される可能性。
- log_ref: OUT/EVENTS.csv(excerpt: xp_amp_app_usage_dnu; bundleId=com.vnp.myviettel); OUT/IDMAP.csv
- ref_diff: OUT_ZIP_INTEGRATION/DIFF_keywords.csv(APPS_SNS_FIN 増分)
- severity: Medium (2)
- confidence: 0.74
- custody_capture/analysis: /mnt/data/KABUKI_INV_2025-06-12_OUT_ZIP_INTEGRATION/sha256_chain_generated.csv
- notes: ベクタ確定の根拠ではないが、同分帯の一括整合の一部として整合。
- flame_flag: Apple=Yes; Microsoft=No; Meta=No; VN-Telco=Yes; CN-Vendor=No
