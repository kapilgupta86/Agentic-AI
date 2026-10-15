# LinkedIn post for the evaluation article (draft for the author to edit and post)

Plain language on purpose (WRITING STANDARD in CLAUDE.md): a smart 10-year-old should follow it.
The article is live at https://keshavaai.in/journal/zero-failures-not-proof after the next deploy. Post after that.
Picture to attach: `public/img/blog/zero-failures-not-proof.png`. Put the link at the end or in the first comment, with the UTM below.

---

**Option A**

Imagine a bag of red and blue marbles. You pull out 10, and all 10 are blue. Are there no red ones? You cannot say.

Testing an AI is the same. "All 50 tests passed" sounds like proof. It is not.

There is a simple rule of thumb, the rule of three. If n tests in a row all passed, the real failure rate is probably below about 3 divided by n.

🔹 10 tests passed: it could still fail about 26 times in 100
🔹 50 tests passed: about 6 times in 100
🔹 500 tests passed: about 6 times in 1,000

So I try to say "no failures in 50 tests", not "it is safe".

Three habits keep a release gate honest:
1. Choose the pass mark before you test, so you cannot move the line to fit the result.
2. Mark some tests as critical. One failure there stops the release, however good the average is.
3. Check what really happened (is there a payment record?), not only what the AI said.

Plain-words guide, with a glossary and the exact maths underneath: https://keshavaai.in/journal/zero-failures-not-proof?utm_source=linkedin&utm_medium=post

What is one test you would never let an AI skip?

---

**Option B (short)**

"All tests passed" is not the same as "safe".

50 perfect tests only tell you the real failure rate is probably below about 6 in 100. For a friendly reply, fine. For a payment, no.

Set the pass mark first, mark the critical tests, and let one critical failure stop the release. Guide: https://keshavaai.in/journal/zero-failures-not-proof?utm_source=linkedin&utm_medium=post

---

Notes
- At most three hashtags (#AIEngineering #LLMOps #AIEvaluation).
- Reply to every comment in the first hour. Save good questions as topics for the next article.
- Check the numbers before posting: 1 - 0.05^(1/n) gives 25.9%, 5.8%, 3.0% and 0.6% for n = 10, 50, 100 and 500.
- The claim holds for independent tests that look like real use. The article says so under "The limits of this advice". Keep that if you edit.
