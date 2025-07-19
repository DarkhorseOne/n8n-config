# n8n-config

## workflow sources

### 1. The official n8n Template Library
n8n.io/workflows

### 2. Community GitHub repos (open source, free)

| Repo                                     | Stars | What’s inside                                                            | Why it’s good                                                                                                      |
| ---------------------------------------- | ----- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `restyler/awesome-n8n`                   | 1.4 k | Top-100 community nodes ranked by npm downloads                          | Great when you need a **node** (integration) rather than a whole template. Updated July 6 2025. ([GitHub][1])      |
| `enescingoz/awesome-n8n-templates`       | 6.9 k | Thousands of JSON templates grouped by app (Slack, Notion, OpenAI, etc.) | Biggest single archive; every file is import-ready. Quality varies—test on a staging instance first. ([GitHub][2]) |
| Reddit dump (`r/n8n` “1 000+ workflows”) | —     | Script-scraped bundle of every template on the web                       | Good for discovery; expect duplicates and broken creds. ([Reddit][3])                                              |

[1]: https://github.com/restyler/awesome-n8n "GitHub - restyler/awesome-n8n: Useful n8n resources: list of community nodes and tutorials"
[2]: https://github.com/enescingoz/awesome-n8n-templates "GitHub - enescingoz/awesome-n8n-templates: Supercharge your workflow automation with this curated collection of n8n templates! Instantly connect your favorite apps-like Gmail, Telegram, Google Drive, Slack, and more-with ready-to-use, AI-powered automations. Save time, boost productivity, and unlock the true potential of n8n in just a few clicks."
[3]: https://www.reddit.com/r/n8n/comments/1kx9u01/all_of_n8n_workflows_i_could_find_1000_enjoy/?utm_source=chatgpt.com "All of N8N workflows I could find (1000+) enjoy - Reddit"

### 3. Third-party marketplaces (paid or freemium)
| Marketplace       | What you get                                                    | When to bother                                                                          |
| ----------------- | --------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| **n8nMarket.com** | Individually priced “premium” templates from vetted freelancers | If you need production-ready flows and can expense \$10-\$50 each. ([n8nmarket.com][1]) |

[1]: https://n8nmarket.com/?utm_source=chatgpt.com "n8n Marketplace | Premium Automation Templates"

## Quick evaluation checklist (don’t skip this)
1. **Last updated date:** Anything untouched for more than 6 months may fail on the latest n8n version.
2. **Credential storage:** Prefer templates that use environment variables instead of hard-coded secrets.
3. **Error handling:** Check for error handling nodes. If there’s no “Catch” sub-workflow, add one before going live.
4. **License:** Most GitHub repos use MIT; marketplace items may have restrictions—always read the fine print.
5. **Dry-run:** Import into a disabled workflow first, use mock endpoints instead of real APIs, and only enable triggers last.

