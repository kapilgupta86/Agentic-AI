# LinkedIn teaser for the caching article (draft for the author to edit and post)

Post only after the article is live (it is: https://keshavaai.in/journal/llm-caching-untangled). Keep the link as the first comment or at the end; use the UTM so visits show in analytics.

---

**Option A (your usual style, calmer)**

Three different things all get called "caching" in LLM land. They run at different moments, live for different lengths of time, and fix different problems.

🔹 KV cache: lives for one answer. Always on. Makes token-by-token decoding possible.
🔹 Prompt (prefix) cache: lives minutes to hours. Reuses the prefill work when the start of your prompt is identical. One timestamp near the top of the prompt breaks it.
🔹 Semantic cache: lives until you say so. Skips the model entirely when a question is similar enough to an old one. The trade is a risk of stale answers.

I wrote it up with a diagram, a table of what Anthropic, OpenAI and Google document today (checked 14 Oct 2026, with sources), and a small simulator where you can change the prefix size, the gap between requests and the cache lifetime and see what happens to the cost.

One thing the simulator makes obvious: with a 1.25x write price and a 0.1x read price, a cached prefix already pays for itself on the first reuse.

Full article and simulator: https://keshavaai.in/journal/llm-caching-untangled?utm_source=linkedin&utm_medium=post

What is the cache mistake you have seen most often?

---

**Option B (shorter)**

If a timestamp sits at the top of your prompt, your prompt cache probably never hits.

Prompt caching needs an exact prefix match. Static content first, dynamic content last. I built a small simulator so you can see it: https://keshavaai.in/journal/llm-caching-untangled?utm_source=linkedin&utm_medium=post

---

Notes
- Hashtags: at most three (#LLM #AIEngineering #LLMOps).
- Reply to every comment in the first hour; save good questions as topics for the next article.
- Numbers in the post come from the article; if provider pricing changes, update the article first.
