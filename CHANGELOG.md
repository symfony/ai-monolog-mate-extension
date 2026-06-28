CHANGELOG
=========

0.13
----

 * Mark the entries returned by `monolog-search`, `monolog-context-search` and `monolog-tail` as untrusted data, since log messages and their context are frequently controlled by end users
 * Allow `ai_mate_monolog.log_dir` to be a map of context name to log directory. Log entries and files then carry a `kernel_context` field, and `monolog-search`, `monolog-context-search`, `monolog-tail`, `monolog-list-files` and `monolog-list-channels` accept an optional `kernelContext` filter parameter

0.7
---

 * Merge `monolog-search-regex` into `monolog-search` via a `regex` parameter
 * Remove `monolog-by-level` tool (use `monolog-search` with `level` filter instead)
 * Add `@param` docblocks to all tool methods for AI-readable parameter descriptions
 * Add optional TOON format encoding for `LogSearchTool` methods to reduce token consumption

0.3
---

 * Add `INSTRUCTIONS.md` with AI agent guidance for log analysis tools

0.1
---

 * Add bridge
