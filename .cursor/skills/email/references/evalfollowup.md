# Example: customer follow up with recommendations

Pattern: thank them for the meeting, acknowledge what was learned, frame the diagnosis gently, give numbered recommendations with short labels, end with a concrete next pass and offer to review together.

---

Hi team,

Thanks for sharing your internal eval workflow with me today. Learned a lot! The cost gap may look larger than it should be, and I think a few changes will give you a much cleaner read.

1. Tighten the eval methodology
Re-run each tool from a brand-new workspace via the Cursor CLI. Pinning the same model, same reasoning effort, repo state, and prompt. Also worth noting: on the Claude Code side, ccusage doesn't always reflect true billed cost, please cross-check against invoices. 

2. Audit Cursor workspace
A lot of the input + cache-write inflation is likely from accumulated skills, rules, and MCP servers being auto-injected into context. The 13K-token "Hi" thread is a good illustration, link. Disable anything not required for the POC and re-run from a clean profile. 

3. Cross-check against independent benchmarks
Our internal data and third-party evals (Artificial Analysis' coding-agents benchmark, link) put the Cursor harness at parity or slightly ahead on cost. A gap this large usually points to methodology rather than the harness.

4. Run implementation on Composer 2.5
Cursor is model-neutral, so the full implementation flow can run on Composer 2.5. It is dramatically cheaper than the frontier models competitors are locked into, link. For a cost-first evaluation, this should be the headline config.

Suggested next pass: clean workspace → Cursor CLI → audited existing workspace → Composer 2.5, then share the per-step numbers. Happy to jump on a call to review results together.

Thanks,
Joseph
