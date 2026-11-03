# Final Task Pool

Audit date: **2026-11-03**.

Project: [spainricardo765-cell/BenchTasksCollv3](https://github.com/spainricardo765-cell/BenchTasksCollv3).
Branch: **finalpool**, based on main commit `6ac0348555050a99bcf4f08ff8bf920616482289`.

## Result

**0 implemented task directories qualify at the recorded revisions.** All 116 checked directories are marked `implementing` in Notion. This pool therefore contains only the audit documentation and manifest, not fabricated or partially checked task implementations.

### Requirements applied

The rules come from `tasks/examples/example-task/readme.txt` and its example files:

- `task_config.json` must have a non-empty `needed_mcp_servers` field and a non-empty `needed_local_tools` field containing `claim_done`.
- `docs/agent_system_prompt.md` and `docs/task.md` must be non-empty and entirely English (no Chinese).
- A non-empty optional `docs/user_system_prompt.md` must also be entirely English.
- `evaluation/main.py`, `preprocess/main.py`, `initial_workspace`, and `groundtruth_workspace` are explicitly optional.
- Beyond those explicit content requirements, no behavioral, execution, code-quality, or unlisted-file requirements were added.

Every checked task directory lacks `task_config.json`. No implementations were modified to satisfy this requirement artificially.

### Tracker updates

- Reviewed all 14 developer branches and their latest task-changing commits.
- Corrected 54 existing `implemented` rows to `implementing`.
- Added the 28 absent tasks represented in those latest commits.
- Also added `lueyang-dev/client-portal`, which is changed by the latest Lueyang commit but was missing from the tracker.
- Final tracker: 116 rows; 0 `implemented`, 116 `implementing`.
- Lueyang's deletion of the optional `territory-manager/preprocess/main.py` was not, by itself, a reason to reject the task.

## Commits and results

`Latest tasks` below contains the task directories touched by the latest task-changing commit. That commit can also update an existing task; it is not necessarily a directory addition. The total-checked column also includes previously existing task directories on the same branch.

| Developer branch | Latest task-changing commit | Latest tasks | Checked | Implemented |
| --- | --- | --- | ---: | ---: |
| fan-dev | [8b90f34](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/8b90f34538e4e106eba103265efaa9a456be498c) | `discount-calculator`, `loyalty-program` | 8 | 0 |
| gyy | [9612fff](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/9612ffff37072726292c77df0f4c6db2f8df1bbb) | `robots-handler`, `sitemap-generator`, `tag-manager` | 9 | 0 |
| haoze | [e0072cf](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/e0072cf979548c56984072cd76f529c7beea59b2) | `media-organizer`, `streaming-service` | 7 | 0 |
| jl_dev | [4e2b63f](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/4e2b63f5dafce88b60886ed6e6af7bd9a8966296) | `customer-feedback-processor`, `inventory-management` | 7 | 0 |
| junteng_dev | [4ab0c54](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/4ab0c5415824d799c3457a26482f9b794c7e9e93) | `customer-portal`, `help-desk` | 10 | 0 |
| junxian_dev | [96bbc11](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/96bbc11b6fc701d07d961aaf070c434fccd1794f) | `currency-converter`, `social-connector` | 8 | 0 |
| lueyang-dev | [bf8b9a1](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/bf8b9a1d25edd81b158db0bb7f49d8624348e74d) | `territory-manager` | 10 | 0 |
| lv | [0be3288](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/0be3288e0fd4ae1f241d3ce9cc1c864ae2606d37) | `analytics-dashboard`, `insights-engine`, `survey-builder` | 9 | 0 |
| ruige | [a6f3fba](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/a6f3fba387f68acaf6517803e88b40a4a3c52658) | `log-analyzer`, `web-crawler` | 8 | 0 |
| wenshuo-dev | [d11080e](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/d11080ed8d65fb72eb32d9353cb20844b593f9e8) | `cache-optimizer`, `scheduler` | 7 | 0 |
| xiaochen_dev | [20bfc73](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/20bfc73490dcf4029b92123b6055e076b7eb5dfa) | `health-monitor`, `status-checker` | 10 | 0 |
| yuxuan-dev | [e82c829](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/e82c8295f9506ced6862ab7f39048a731b48beb4) | `sync-service` | 7 | 0 |
| yuzhen-dev | [c68265d](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/c68265dafe0a0eccc6e183ff96d1a3e5591a3d8b) | `audit-logger`, `resource-monitor` | 9 | 0 |
| zhaochen | [b5f9cc4](https://github.com/spainricardo765-cell/BenchTasksCollv3/commit/b5f9cc4f79bb9218e40c0293ab9ec4e90352a626) | `certificate-manager`, `storage-manager` | 7 | 0 |

## Verification and provenance

- [Task Tracker](https://app.notion.com/p/Task-Tracker-40d046bca0c8811797cafff63d83ffa2) contains the current statuses and implementors.
- [Full audit notes](https://app.notion.com/p/Task-Audit-2026-11-03-40d046bca0c881bfb72acc34fd5dae58) records the review method, branch revisions, and additional language findings.
- [manifest.json](manifest.json) records every inspected task name, validation failures, and the currently empty selection.

This is a point-in-time audit. Once a source task passes the acceptance rules and its Notion status becomes `implemented`, its complete existing task directory can be added under `tasks/finalpool/<task-name>` using its recorded source branch mapping.
