# Local branch: what it carries relative to upstream

`local` = upstream release `v0.8.1` (base) + the `topic/*` branches below. Tags are
`v<base>-local<NN>`. Rules: eejd/macports-ports-local `docs/development-model.md`,
"Forks, upstreams and port tiers".

| Change | Branch | Origin | Upstream status |
|---|---|---|---|
| fix(scheduler): drain final update after shutdown_event is set (the last request's completion could be dropped from the report) | `topic/scheduler-drain-final-update` | own work (eejd/py-guidellm#1) | Not submitted by us. Same defect: vllm-project/guidellm#1221 (open); open upstream fix: vllm-project/guidellm#1223 (not merged as of 2026-10-16). Drop this topic when a release contains a fix for #1221. |
