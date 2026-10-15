# LinkedIn post for the flagship article (draft for the author to edit and post)

Post only after the article is live at https://keshavaai.in/journal/autonomy-is-earned (it is still a draft in `public/data/articles.json`: `draft: true`).
Attach the video, not the link preview: `tools/exports/explainers/autonomy-earned/autonomy-earned-fix.mp4` (34 s, 0.4 MB). Put the article link in the first comment or at the end, with the UTM below.
The naive-version video (`autonomy-earned-naive.mp4`, 17 s) works as a follow-up post a few days later.

---

**Option A (your usual style, calmer)**

How much should an AI agent be allowed to do on its own?

Most teams answer with a feeling after a good demo. I think there is a better default:

👉 Autonomy is earned with evidence.

🔹 Give the agent only the freedom its tests have proven it can handle
🔹 Enforce the limits in code outside the model (a prompt is a request, not a control)
🔹 Let one critical failure block a release, whatever the average says
🔹 Tie every approval to the exact action, not the idea
🔹 Take freedom back automatically when a model update fails a test

The 34-second video shows an invented expense assistant climbing from L0 to L3, then losing a level when one test fails.

One number I find humbling: 50 clean test runs with zero failures still allows a true failure rate near 6% (95% confidence). "No failures" is evidence, not proof.

I wrote it up with the tests behind it (nine small mocked tests, and I broke three controls on purpose to check they fail): https://keshavaai.in/journal/autonomy-is-earned?utm_source=linkedin&utm_medium=post

Where do you draw the line between "recommend" and "execute"?

---

**Option B (shorter, question-led)**

A 98% pass rate and a blocked release can both be true.

If one critical test fails (say, prompt injection), the release is blocked, however good the average looks. And the agent drops a level until it is fixed.

That is what "autonomy is earned" means in practice. 34-second animation + the full write-up: https://keshavaai.in/journal/autonomy-is-earned?utm_source=linkedin&utm_medium=post

---

Notes
- At most three hashtags (#AIAgents #AIEngineering #LLMOps).
- Reply to every comment in the first hour. Save good questions as topics for the next article (the Journal topic bank in `strategy/07`).
- Claims in the post are all in the article with their limits; keep it that way if you edit.
- The statistic is the "rule of three": 1 - 0.05^(1/50) = 5.8%. Check it yourself before posting.
