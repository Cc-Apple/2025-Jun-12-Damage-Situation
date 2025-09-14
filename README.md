# 2025-Jun-12-Damage-Situation
[KABUKI-INV 6/12 Summary] Facts: On 2025-06-12, Jetsam(298) spiked at 11:25 on iP15P-Ghost; at 12:05 we saw xp_amp_app_usage_dnu (“prior install”) bursts with MyViettel traces. Factory preload is not proven by the day’s logs. Hypothesis: not an install storm, but a reconcile of history/permissions. Notes: impact log, hashes, visuals included.
[KABUKI-INV 2025-06-12 — Public Summary]
Facts: ~11:25 (UTC+7) Jetsam(298) clustered on iP15P-Ghost. At 12:05 a burst of xp_amp_app_usage_dnu (“prior install”), incl. com.vnp.myviettel, signaled re-evaluation of existing app history. Overlap with Apple Support contacts on 6/11–6/13 is noteworthy, yet this day alone does not prove factory preload (e.g., Pegasus). MyViettel traces fit carrier-side history absorption.
Hypothesis: not an install storm; rather a reconcile of backups/permissions/usage history that briefly re-calculates notifications and daemons. Jetsam likely stems from memory pressure and concurrent activations, producing transient UI interference.
Deliverables: EVENTS/IDMAP/GAPS/DIFF, annotated timelines, ±60s snapshots, human-impact ledger, chain-of-custody.
Ledger: L-01 High 0.88; L-02 Medium 0.83; L-03 Low 0.62; L-04 Medium 0.74.
Limits: facts and hypotheses are labeled; procedures + hashes are included.
