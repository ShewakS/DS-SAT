FlowRack Logistics Pvt. Ltd. — Synthetic Raw Dataset Pack

This is a synthetic practice dataset for the Warehouse Efficiency Insight assessment.
All records are fictional and generated for learning/practice. It is deliberately unprocessed and includes data-quality issues.

Files:
- orders.csv: order_id, item_count, priority, order_timestamp
- picks.csv: pick_id, order_id, picker_id, zone_id, item_id, start_time, finish_time, quantity
- items.csv: item_id, category, size, storage_class
- workers.csv: picker_id, shift, experience_band
- zones.csv: zone_id, zone_type, distance_band

Intentionally included issues (not an exhaustive row-by-row map):
- Missing values in timestamps and attributes
- Exact duplicate records and repeated IDs requiring investigation
- Inconsistent capitalization/spacing in categorical labels
- Invalid timestamp strings
- Negative durations caused by finish times before start times
- Negative/missing quantities and implausible item counts
- Missing or unknown foreign keys
- Conflicting duplicate reference records

Important:
- These files are intentionally RAW. Do not assume repeated IDs are always safe to delete; inspect and document decisions.
- Queue time cannot be confidently calculated from order_timestamp and start_time unless you verify their meaning and account for timestamps that can precede/overlap other activities. Treat any derived queue-time proxy as an assumption.
- Synthetic data is for practice and must not be represented as real company operational data.
