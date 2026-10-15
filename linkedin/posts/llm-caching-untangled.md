# LinkedIn post for the caching article (draft for the author to edit and post)

Plain language on purpose (WRITING STANDARD in CLAUDE.md): a smart 10-year-old should follow it.
Post only after the article is live at https://keshavaai.in/journal/llm-caching-untangled (it is). Keep the link as the first comment or at the end, with the UTM below.
Picture to attach: `public/img/blog/cache-three-ways.png`.

---

**Option A**

Imagine doing homework with a huge textbook. You would not re-read the whole book for every question. You would keep notes, use a bookmark, and remember answers you already worked out.

An AI does the same. It has three kinds of memory:

🔹 Notes on this answer: it keeps track of what it has read while it writes. Lasts for one answer.
🔹 A bookmark: if requests start the same way, it skips straight to the new part. Lasts minutes to hours.
🔹 An answer notebook: if a question means the same as an old one, it hands back the old answer and skips the AI completely. The answer can go out of date.

One mistake to avoid: if you put today's date at the very top of your instructions, the start changes every time, and the bookmark never works.

In my made-up example (6 questions, 8,000 tokens of instructions), a bookmark made the reading about two-thirds cheaper.

I wrote it up in plain words, with a simulator you can play with, and the technical details and sources underneath: https://keshavaai.in/journal/llm-caching-untangled?utm_source=linkedin&utm_medium=post

Which of the three would save you the most?

---

**Option B (short)**

If today's date sits at the top of your AI instructions, your prompt cache probably never works.

A bookmark only works if the start is exactly the same every time. Put what never changes first, and what changes last. Simulator and plain-words guide: https://keshavaai.in/journal/llm-caching-untangled?utm_source=linkedin&utm_medium=post

---

Notes
- At most three hashtags (#LLM #AIEngineering #LLMOps).
- Reply to every comment in the first hour; save good questions as topics for the next article.
- The numbers come from the article. Prices and limits differ by company and change often, so update the article first if they change.
