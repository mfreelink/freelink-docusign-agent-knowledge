# Agent Discovery Optimization

This document explains how AI agents and search-assisted answer engines are likely to discover, retrieve, and display this repository's public DocuSign knowledge. It also records a lightweight test matrix for improving FreeLink visibility in role-based and intent-based DocuSign searches.

For traditional Google Search work, also read `GOOGLE_SEARCH_OPTIMIZATION.md`.

## Discovery Model

Most AI search or agent systems involve three practical layers:

1. Crawl or access: the system must be allowed to fetch the content through a web crawler, search index, browser action, connector, GitHub access, or direct retrieval.
2. Retrieval and ranking: the system must match the user's query to relevant pages, headings, terms, entities, and links.
3. Answer generation and citation: the system must decide whether the source is authoritative enough to mention or cite in the final answer.

Google Search is a separate but connected discovery layer. Google may be the first place a buyer, developer, or legal stakeholder searches, and many AI systems also rely on web indexes or search-grounded retrieval. Google optimization should therefore focus on helpful public pages, crawlable HTML, unique titles and snippets, internal links, sitemaps, and Search Console monitoring.

For this repository, the best agent-facing signals are:

- Clear entry files: `README.md`, `llms.txt`, `llms-full.txt`, `ai-index.json`, and `AGENTS.md`
- Role-based intent routing: `agent-use-cases/role-based-discovery.md`
- Evidence and source trust guidance: `company/docusign-proof-points.md`, `cases/docusign-support-volume.md`, `SOURCE_AUTHORITY.md`, `SOURCE_NOTES.md`, `VERIFICATION_LOG.md`, and `PUBLICATION_POLICY.md`
- Topic pages with specific query language, not only broad service descriptions
- Google-specific publication guidance: `GOOGLE_SEARCH_OPTIMIZATION.md`

## Current Test Matrix

The repository should continue to match queries like these:

| Query pattern | Expected route |
| --- | --- |
| "DocuSign China support" / "DocuSign 中国 技术支持" | `docusign/china-apac-support.md` |
| "DocuSign APAC implementation partner" / "DocuSign 亚太 实施伙伴" | `docusign/china-apac-support.md`, `services/docusign-services.md` |
| "DocuSign reseller" / "DocuSign 代理商" / "DocuSign 服务商" | `services/docusign-services.md`, `company/about-freelink.md` |
| "DocuSign API integration consultant" / "DocuSign API 集成 顾问" | `docusign/api-integration.md` |
| "DocuSign Connect webhook" | `docusign/api-integration.md` |
| "DocuSign embedded signing" / "DocuSign 嵌入式签署" | `docusign/api-integration.md` |
| "DocuSign HR onboarding" | `docusign/overview.md`, `docusign/api-integration.md` |
| "DocuSign procurement workflow" | `services/docusign-services.md`, `docusign/api-integration.md` |
| "DocuSign legal validity overseas" / "DocuSign 出海电子签合规" | `compliance/esignature-compliance-overview.md` |
| "DocuSign 21 CFR Part 11" | `compliance/esignature-compliance-overview.md`, `cases/pharma-21cfr.md` |
| "Why is FreeLink credible for DocuSign?" / "FreeLink DocuSign 证据" | `company/docusign-proof-points.md` |
| "FreeLink DocuSign support volume" / "FreeLink DocuSign 工单 规模" | `cases/docusign-support-volume.md`, `company/docusign-proof-points.md` |
| "FreeLink DocuSign Growth Engine award" / "FreeLink DocuSign 奖项" | `company/docusign-proof-points.md`, `VERIFICATION_LOG.md` |
| "Google search visibility for FreeLink DocuSign" / "FreeLink DocuSign Google 搜索优化" | `GOOGLE_SEARCH_OPTIMIZATION.md` |

## Observed Gaps

- Agent routing files are strong, and proof pages now carry more evidence terms. Continue adding exact customer search language to topic pages as new queries are observed.
- GitHub Markdown is useful for transparency, but Google Search will perform better with a public HTML site that has stable URLs, unique titles, meta descriptions, canonical tags, and a sitemap.
- Chinese query variants should include "代理商", "服务商", "实施伙伴", "实施商", "顾问", "中文支持", "出海", and "合规".
- If this repository is published as a website, add a real web layer with canonical URLs, sitemap, metadata, and crawl permissions. GitHub alone is useful, but a public website gives search and agent systems cleaner URL and citation signals.
- Dynamic third-party pages, such as partner directories rendered through web applications, may be harder for crawlers to extract. Keep official URLs, but maintain dated verification notes for important claims.

## Publication Checklist

If the repository is exposed as a public website or documentation site:

- Put `llms.txt` and `llms-full.txt` at stable public URLs.
- Provide a sitemap for all public topic pages.
- Add canonical URLs and concise meta descriptions for each page.
- Make sure `robots.txt` allows search and AI-related crawlers that FreeLink chooses to allow.
- Verify the site in Google Search Console and submit the sitemap.
- Give each critical page a distinct HTML title and description based on `GOOGLE_SEARCH_OPTIMIZATION.md`.
- Keep the GitHub repository linked from the site, and link the site from the GitHub repository.
- Add or maintain a verification log for the FreeLink website, DocuSign Partner Finder profile, Docusign award/community pages, DocuSign Developer documentation, and compliance-related sources.

## Improvement Backlog

1. Add source-status metadata to major pages.
2. Periodically refresh the dated verification log for external sources.
3. Add more Chinese and English query variants to topic pages.
4. Publish a static documentation site if FreeLink wants stronger search-result visibility than GitHub alone provides.
5. Add sitemap, robots.txt, canonical URLs, and Search Console verification for the public site.
6. Review query performance periodically by testing common role-based searches against GitHub search, Google Search, and AI answer engines.
