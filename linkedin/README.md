# LinkedIn drafts

Drafts for LinkedIn, kept here next to the sources. **Nothing in this folder has been posted to LinkedIn yet** (status column). The canonical version of every piece lives on [keshavaai.in](https://keshavaai.in/blog); the drafts here are adapted for LinkedIn's editor.

| Piece | Status | Files | Canonical page | Posted on |
|---|---|---|---|---|
| Autonomy is earned: how much freedom should an AI agent get? | Draft | [article](articles/autonomy-is-earned.html) · [post](posts/autonomy-is-earned.md) | [autonomy-is-earned](https://keshavaai.in/journal/autonomy-is-earned) | |
| AI caching, explained simply: three ways an AI avoids doing the same work twice | Draft | [article](articles/llm-caching-untangled.html) · [post](posts/llm-caching-untangled.md) | [llm-caching-untangled](https://keshavaai.in/journal/llm-caching-untangled) | |
| 50 tests passed. Is it safe? Why "no failures" is not proof | Draft | [article](articles/zero-failures-not-proof.html) · [post](posts/zero-failures-not-proof.md) | [zero-failures-not-proof](https://keshavaai.in/journal/zero-failures-not-proof) | |

## The workflow
1. Publish on the website first (the page, sitemap and feed go live together).
2. Post the short LinkedIn **post** (`posts/*.md`) with the video or image from `media/`. Put the link with the UTM tag in the first comment or at the end.
3. Only if wanted, publish the longer LinkedIn **article** version (`articles/*.html`): copy the content box into LinkedIn's *Write article* editor. It links back to the canonical page.
4. Change the status above to *Published* and fill in the date.

## Notes
- Preview pages: [index.html](index.html). They carry `noindex` and a canonical link to keshavaai.in so search engines treat the website as the original. The pages are still public by URL (GitHub Pages), so keep nothing private here.
- LinkedIn articles cannot hold tables or interactive embeds. Tables become lists; the interactive animation becomes a GIF plus a link.
- Rules for every piece: sourced or "illustrative" numbers, invented examples, no employer, client or course material.
- Regenerate from the website's article data with `node tools/build-linkedin.mjs` in the website project.
- The older caching documents in the repository root predate the corrected version here (the root copy still has the original, unverified provider numbers). Prefer `articles/llm-caching-untangled.html`.
