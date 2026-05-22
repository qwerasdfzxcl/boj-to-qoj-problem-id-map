# BOJ to QOJ Problem ID Map

Public BOJ problem ID to QOJ problem ID mapping.

## Files

- `boj_to_qoj_problem_id_map.json`: compact object mapping BOJ problem IDs to QOJ problem IDs.
- `boj_to_qoj_problem_id_map.detailed.json`: public detail export with the same mapping plus QOJ URL, QOJ title when available, and a coarse `match_type`.

## Schema

Compact file:

```json
{
  "1014": 5769
}
```

Detailed file:

```json
{
  "metadata": {
    "schema_version": "public-v1",
    "mapping_count": 7868
  },
  "boj_to_qoj": {
    "1014": 5769
  },
  "mapping_details": {
    "1014": {
      "boj_problem_id": 1014,
      "qoj_problem_id": 5769,
      "qoj_url": "https://qoj.ac/problem/5769",
      "match_type": "contest_export",
      "qoj_title": "Example"
    }
  }
}
```

`match_type` is intentionally coarse and should be treated as provenance context, not as independent proof that two problems are equivalent.

The public export omits internal review logs, source category paths, previous mapping records, and account-specific data.
