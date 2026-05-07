# ai-scan-main-pip

Probe 1/2 for **SCA-5368** — default branch with AI deps. AI scan IS expected
to run on this branch (positive case).

## Layout

```
.whitesource
requirements.txt           ← anthropic, openai, requests
autotest_config.json       ← branch: null (default-branch flow)
```

## How the test runs

1. Fork `mend-detection-qa/ai-scan-main-pip`.
2. `branch: null` ⇒ today's default-branch flow runs unchanged.
3. Trigger commit + security check on the default branch.
4. Assert: deps `anthropic`, `openai`, `requests` detected; AI-scan-executed log
   line present (TODO placeholder).