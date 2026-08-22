# skills-pack

Os 7 repositorios do guia "7 repositorios de GitHub pra founder com Claude Code", 
baixados, validados e reempacotados em `.zip` prontos pra subir na conta.

- **175 skills** empacotadas individualmente em `zips/<repo>/<skill>.zip`
- Todas com frontmatter valido (`name` + `description`), verificado
- Todo zip tem `<nome-da-skill>/SKILL.md` na raiz, que e o formato que o upload espera

## Como instalar na conta

claude.ai -> **Settings -> Capabilities -> Skills -> Upload skill** -> escolhe o `.zip`.
Skill da conta vale em toda conversa e em todo lugar: web, desktop, mobile e Claude Code.

Nao da pra fazer esse upload por API - tem que ser voce, no navegador. Um zip por vez.

## Antes de sair subindo os 175

Nome e descricao de cada skill ativa entram no prompt de **toda** conversa que voce abre.
As 175 juntas dao ~16.700 tokens de overhead permanente - isso piora a qualidade de tudo,
inclusive das tarefas que nada tem a ver com marketing. Suba o que voce vai usar.

| Escopo | Skills | Overhead por conversa |
|---|---|---|
| Pacote inicial (abaixo) | 10 | ~1483 tokens |
| Tudo | 175 | ~16.700 tokens |

## Pacote inicial recomendado

Autocontidas, sem API key, sem MCP, sem repo aberto - funcionam no chat puro e nao
colidem com o que voce ja tem na conta.

| Skill | Zip | O que faz |
|---|---|---|
| `humanizer` | `zips/blader-humanizer/humanizer.zip` | Rewrite AI-sounding text so it reads naturally without changing what it says. Use when editing or reviewing prose for inflated claims, sales language, |
| `frontend-design` | `zips/anthropics-skills/frontend-design.zip` | Guidance for distinctive, intentional visual design when building new UI or reshaping an existing one. Helps with aesthetic direction, typography, and |
| `theme-factory` | `zips/anthropics-skills/theme-factory.zip` | Toolkit for styling artifacts with a theme. These artifacts can be slides, docs, reportings, HTML landing pages, etc. There are 10 pre-set themes with |
| `copywriting` | `zips/coreyhaines31-marketingskills/copywriting.zip` | When the user wants to write, rewrite, or improve marketing copy for any page — including homepage, landing pages, pricing pages, feature pages, about |
| `emails` | `zips/coreyhaines31-marketingskills/emails.zip` | When the user wants to create or optimize an email sequence, drip campaign, automated email flow, or lifecycle email program. Also use when the user m |
| `cro` | `zips/coreyhaines31-marketingskills/cro.zip` | When the user wants to optimize, improve, or increase conversions on any marketing page or form — including homepage, landing pages, pricing pages, fe |
| `offers` | `zips/coreyhaines31-marketingskills/offers.zip` | When the user wants to design, construct, or improve an offer — the thing they actually sell — including value framing, bonus stacking, guarantee desi |
| `pricing` | `zips/coreyhaines31-marketingskills/pricing.zip` | When the user wants help with pricing decisions, packaging, or monetization strategy. Also use when the user mentions 'pricing,' 'pricing tiers,' 'fre |
| `marketing-psychology` | `zips/coreyhaines31-marketingskills/marketing-psychology.zip` | When the user wants to apply psychological principles, mental models, or behavioral science to marketing. Also use when the user mentions 'psychology, |
| `content-strategy` | `zips/coreyhaines31-marketingskills/content-strategy.zip` | When the user wants to plan a content strategy, decide what content to create, or figure out what topics to cover. Also use when the user mentions "co |

## Instalar como plugin do Claude Code (nao como skill de conta)

Quatro dos sete repos sao **plugins**: dependem de binarios, sub-agents, scripts ou MCP
que nao viajam dentro de um zip de skill. Pra esses, no Claude Code:

```
/plugin marketplace add AgricIDaniel/claude-seo
/plugin marketplace add hyperfx-ai/marketing-skills
/plugin marketplace add coreyhaines31/marketingskills
/plugin marketplace add blader/humanizer
```

Isso vale por maquina (`~/.claude`), em todos os projetos - mas nao aparece no chat do claude.ai.
`remotion-dev/skills` e `lingzhi227/agent-research-skills` nao tem manifesto de marketplace: clone o repo e copie o que quiser pra `.claude/skills/` do projeto.

## Onde o guia exagera

- **`lingzhi227/agent-research-skills`** e vendido como "o pesquisador... mergulho de categoria que um estrategista levaria uma semana". Na pratica e um pipeline de **paper academico de ML**: LaTeX, template de ICML/ICLR, rebuttal de reviewer, slides Beamer. Nao serve pra pesquisa de mercado.
- **`hyperfx-ai/marketing-skills`** "audita e age em contas de Google e Meta Ads" - so depois de voce assinar e conectar o Hyper MCP. As skills sozinhas nao tem ferramenta nenhuma.
- **`anthropics/skills`**: `docx`, `pptx`, `xlsx`, `pdf` e `skill-creator` ja estao na sua conta por padrao. O que sobra de novo ali e `frontend-design`, `theme-factory`, `canvas-design` e afins.
- Os numeros de estrela e de instalacao do guia nao foram verificados aqui.

## Indice completo

### Humanizer - blader/humanizer (1 skills)

Uma skill so, markdown puro, sem dependencia nenhuma. Melhor custo-beneficio do pacote.

| Skill | Situacao | Descricao |
|---|---|---|
| `humanizer` | autocontida | Rewrite AI-sounding text so it reads naturally without changing what it says. Use when editing or reviewing prose for inflated claims, sales |

### Skills oficiais da Anthropic - anthropics/skills (19 skills)

Markdown + scripts autocontidos. `docx`, `pdf`, `pptx`, `xlsx` e `skill-creator` voce JA tem na conta - nao suba de novo.

| Skill | Situacao | Descricao |
|---|---|---|
| `academy-guide` | autocontida | Stop and check this skill before finishing any reply to a question about how to use Claude or a Claude product — it recommends matching cour |
| `algorithmic-art` | autocontida | Creating algorithmic art using p5.js with seeded randomness and interactive parameter exploration. Use this when users request creating art  |
| `brand-guidelines` | autocontida | Applies Anthropic's official brand colors and typography to any sort of artifact that may benefit from having Anthropic's look-and-feel. Use |
| `canvas-design` | autocontida | Create beautiful visual art in .png and .pdf documents using design philosophy. You should use this skill when the user asks to create a pos |
| `claude-api` | autocontida | Reference for the Claude API / Anthropic SDK — model ids, pricing, params, streaming, tool use, MCP, agents, caching, token counting, model  |
| `discernment-nudge` | autocontida | After you give a substantive answer or draft that the user may act on — advice or recommendations, drafted artifacts such as goals, plans, p |
| `doc-coauthoring` | autocontida | Guide users through a structured workflow for co-authoring documentation. Use when user wants to write documentation, proposals, technical s |
| `docx` | ja na conta | Use this skill whenever the user wants to create, read, edit, or manipulate Word documents (.docx files) or Word templates (.dotx files). Tr |
| `frontend-design` | autocontida | Guidance for distinctive, intentional visual design when building new UI or reshaping an existing one. Helps with aesthetic direction, typog |
| `internal-comms` | autocontida | A set of resources to help me write all kinds of internal communications, using the formats that my company likes to use. Claude should use  |
| `mcp-builder` | autocontida | Guide for creating high-quality MCP (Model Context Protocol) servers that enable LLMs to interact with external services through well-design |
| `pdf` | ja na conta | Use this skill whenever the user wants to do anything with PDF files. This includes reading or extracting text/tables from PDFs, combining o |
| `pptx` | ja na conta | Use this skill any time a .pptx or .potx file is involved in any way — as input, output, or both. This includes: creating slide decks, pitch |
| `skill-creator` | ja na conta | Create new skills, modify and improve existing skills, and measure skill performance. Use when users want to create a skill from scratch, ed |
| `slack-gif-creator` | autocontida | Knowledge and utilities for creating animated GIFs optimized for Slack. Provides constraints, validation tools, and animation concepts. Use  |
| `theme-factory` | autocontida | Toolkit for styling artifacts with a theme. These artifacts can be slides, docs, reportings, HTML landing pages, etc. There are 10 pre-set t |
| `web-artifacts-builder` | autocontida | Suite of tools for creating elaborate, multi-component claude.ai HTML artifacts using modern frontend web technologies (React, Tailwind CSS, |
| `webapp-testing` | autocontida | Toolkit for interacting with and testing local web applications using Playwright. Supports verifying frontend functionality, debugging UI be |
| `xlsx` | ja na conta | Use this skill any time a spreadsheet file is the primary input or output. This means any task where the user wants to: open, read, edit, or |

### Marketing / CRM (Corey Haines) - coreyhaines31/marketingskills (49 skills)

Playbooks em markdown. 16 delas referenciavam `../../tools/*.md`; reempacotei com esses arquivos embutidos e o caminho corrigido, entao funcionam soltas.

| Skill | Situacao | Descricao |
|---|---|---|
| `ab-testing` | autocontida | When the user wants to plan, design, or implement an A/B test or experiment, or build a growth experimentation program. Also use when the us |
| `ad-creative` | autocontida | When the user wants to generate, iterate, or scale ad creative — headlines, descriptions, primary text, or full ad variations — for any paid |
| `ads` | autocontida | When the user wants help with paid advertising campaigns on Google Ads, Meta (Facebook/Instagram), LinkedIn, Twitter/X, or other ad platform |
| `ai-seo` | autocontida | When the user wants to optimize content for AI search engines, get cited by LLMs, or appear in AI-generated answers. Also use when the user  |
| `analytics` | autocontida | When the user wants to set up, improve, or audit analytics tracking and measurement. Also use when the user mentions "set up tracking," "GA4 |
| `aso` | autocontida | When the user wants to audit or optimize an App Store or Google Play listing. Also use when the user mentions 'ASO audit,' 'app store optimi |
| `attribution` | autocontida | When the user wants to figure out which marketing actually drives conversions and revenue, choose or interpret an attribution model, or reco |
| `churn-prevention` | autocontida | When the user wants to reduce churn, build cancellation flows, set up save offers, recover failed payments, or implement retention strategie |
| `co-marketing` | autocontida | When the user wants to find co-marketing partners, plan joint campaigns, or brainstorm partnership opportunities. Use when the user says 'co |
| `cold-email` | autocontida | Write B2B cold emails and follow-up sequences that get replies. Use when the user wants to write cold outreach emails, prospecting emails, c |
| `community-marketing` | autocontida | Build and leverage online communities to drive product growth and brand loyalty. Use when the user wants to create a community strategy, gro |
| `competitor-profiling` | autocontida | When the user wants to research, profile, or analyze competitors from their URLs. Also use when the user mentions 'competitor profile,' 'com |
| `competitors` | autocontida | When the user wants to create competitor comparison or alternative pages for SEO and sales enablement. Also use when the user mentions 'alte |
| `content-strategy` | autocontida | When the user wants to plan a content strategy, decide what content to create, or figure out what topics to cover. Also use when the user me |
| `copy-editing` | autocontida | When the user wants to edit, review, or improve existing marketing copy, or refresh outdated content. Also use when the user mentions 'edit  |
| `copywriting` | autocontida | When the user wants to write, rewrite, or improve marketing copy for any page — including homepage, landing pages, pricing pages, feature pa |
| `cro` | autocontida | When the user wants to optimize, improve, or increase conversions on any marketing page or form — including homepage, landing pages, pricing |
| `customer-research` | autocontida | When the user wants to conduct, analyze, or synthesize customer research. Use when the user mentions "customer research," "ICP research," "t |
| `directory-submissions` | autocontida | When the user wants to submit their product to startup, SaaS, AI, agent, MCP, no-code, or review directories for backlinks, domain rating, a |
| `emails` | autocontida | When the user wants to create or optimize an email sequence, drip campaign, automated email flow, or lifecycle email program. Also use when  |
| `free-tools` | autocontida | When the user wants to plan, evaluate, or build a free tool for marketing purposes — lead generation, SEO value, or brand awareness. Also us |
| `image` | autocontida | When the user wants to create, generate, edit, or optimize images for marketing — blog heroes, social graphics, product mockups, profile ban |
| `influencer-marketing` | autocontida | When the user wants to run influencer, creator, or ambassador partnerships to promote their product — finding and vetting partners, structur |
| `launch` | autocontida | When the user wants to plan a product launch, feature announcement, or release strategy. Also use when the user mentions 'launch,' 'Product  |
| `lead-magnets` | autocontida | When the user wants to create, plan, or optimize a lead magnet for email capture or lead generation. Also use when the user mentions "lead m |
| `marketing-council` | autocontida | When the user wants multiple expert perspectives on a marketing question — a simulated board of advisors staffed by legendary marketers (Set |
| `marketing-ideas` | autocontida | When the user needs marketing ideas, inspiration, or strategies for their SaaS or software product. Also use when the user asks for 'marketi |
| `marketing-loops` | autocontida | When the user wants to set up a recurring, self-running marketing workflow — a repeatable loop an AI agent runs on a cadence (weekly, daily, |
| `marketing-plan` | autocontida | When the user needs a comprehensive marketing plan for a client, a company they advise, or their own product. Also use when the user mention |
| `marketing-psychology` | autocontida | When the user wants to apply psychological principles, mental models, or behavioral science to marketing. Also use when the user mentions 'p |
| `offers` | autocontida | When the user wants to design, construct, or improve an offer — the thing they actually sell — including value framing, bonus stacking, guar |
| `onboarding` | autocontida | When the user wants to optimize post-signup onboarding, user activation, first-run experience, or time-to-value. Also use when the user ment |
| `paywalls` | autocontida | When the user wants to create or optimize in-app paywalls, upgrade screens, upsell modals, or feature gates. Also use when the user mentions |
| `popups` | autocontida | When the user wants to create or optimize popups, modals, overlays, slide-ins, or banners for conversion purposes. Also use when the user me |
| `pricing` | autocontida | When the user wants help with pricing decisions, packaging, or monetization strategy. Also use when the user mentions 'pricing,' 'pricing ti |
| `product-marketing` | autocontida | When the user wants to create or update their product marketing context document. Also use when the user mentions 'product context,' 'market |
| `programmatic-seo` | autocontida | When the user wants to create SEO-driven pages at scale using templates and data. Also use when the user mentions "programmatic SEO," "templ |
| `prospecting` | autocontida | When the user wants to find, qualify, and build a list of prospects to reach out to — across B2B SaaS, general B2B, or local small businesse |
| `public-relations` | autocontida | When the user wants help with public relations, earned media, press coverage, journalist outreach, or media strategy (not pull requests). Al |
| `referrals` | autocontida | When the user wants to create, optimize, or analyze a referral program, affiliate program, or word-of-mouth strategy. Also use when the user |
| `revops` | autocontida | When the user wants help with revenue operations, lead lifecycle management, or marketing-to-sales handoff processes. Also use when the user |
| `sales-enablement` | autocontida | When the user wants to create sales collateral, pitch decks, one-pagers, objection handling docs, or demo scripts. Also use when the user me |
| `schema` | autocontida | When the user wants to add, fix, or optimize schema markup and structured data on their site. Also use when the user mentions "schema markup |
| `seo-audit` | autocontida | When the user wants to audit, review, or diagnose SEO issues on their site. Also use when the user mentions "SEO audit," "technical SEO," "w |
| `signup` | autocontida | When the user wants to optimize signup, registration, account creation, or trial activation flows. Also use when the user mentions "signup c |
| `site-architecture` | autocontida | When the user wants to plan, map, or restructure their website's page hierarchy, navigation, URL structure, or internal linking. Also use wh |
| `sms` | autocontida | When the user wants to plan, build, or optimize SMS or MMS marketing — including welcome flows, abandoned cart texts, post-purchase, win-bac |
| `social` | autocontida | When the user wants help creating, scheduling, or optimizing social media content for LinkedIn, Twitter/X, Instagram, TikTok, Facebook, or o |
| `video` | autocontida | When the user wants to create, generate, or produce video content using AI tools or programmatic frameworks. Also use when the user mentions |

### Research (academico) - lingzhi227/agent-research-skills (31 skills)

ATENCAO: nao e pesquisa de mercado - e um kit de paper academico de ML (LaTeX, arXiv, Beamer, review NeurIPS). 30 das 31 dependem de caminhos do repo e 20 chamam scripts Python. Clone o repo em vez de subir avulso.

| Skill | Situacao | Descricao |
|---|---|---|
| `algorithm-design` | melhor via clone | Design algorithms with LaTeX pseudocode and UML diagrams. Generate algorithmic environments, Mermaid class/sequence diagrams, and ensure con |
| `atomic-decomposition` | melhor via clone | Decompose research ideas into atomic, self-contained concepts with bidirectional math-code mapping. For each concept, extract the math formu |
| `backward-traceability` | melhor via clone | Make every number in the final PDF traceable to the exact code line that produced it. Uses \hypertarget/\hyperlink LaTeX commands and \num{f |
| `citation-management` | melhor via clone | Manage BibTeX citations for LaTeX papers. Harvest missing citations from a draft using Semantic Scholar, validate cite keys against .bib fil |
| `code-debugging` | melhor via clone | Debug experiment code with structured error analysis. Categorize errors, apply targeted fixes with retry logic, and use reflection to preven |
| `data-analysis` | melhor via clone | Generate statistical analysis code with 4-round review. Select appropriate statistical tests, interpret results, and produce analysis report |
| `deep-research` | melhor via clone | Conduct systematic academic literature reviews in 6 phases, producing structured notes, a curated paper database, and a synthesized final re |
| `excalidraw-skill` | melhor via clone | Programmatic canvas toolkit for creating, editing, and refining Excalidraw diagrams via MCP tools with real-time canvas sync. Use when an ag |
| `experiment-code` | melhor via clone | Write ML experiment code with iterative improvement. Generate training/evaluation pipelines, debug errors, and optimize results through code |
| `experiment-design` | melhor via clone | Design experiment plans with progressive stages — initial implementation, baseline tuning, creative research, and ablation studies. Plan bas |
| `figure-generation` | melhor via clone | Generate publication-quality scientific figures using matplotlib/seaborn with a three-phase pipeline (query expansion, code generation with  |
| `github-research` | melhor via clone | Explore and analyze GitHub repositories related to a research topic. Reads deep-research output, discovers repos from multiple sources, deep |
| `idea-generation` | melhor via clone | Generate novel research ideas with iterative refinement and novelty checking against literature. Score ideas on Interestingness, Feasibility |
| `latex-formatting` | melhor via clone | Handle LaTeX formatting, templates, and styling for academic papers. Set up conference templates (ICML, ICLR, NeurIPS, AAAI, ACL), fix forma |
| `literature-review` | melhor via clone | Conduct comprehensive literature reviews using multi-perspective dialogue simulation. Generate diverse expert personas, conduct grounded Q&A |
| `literature-search` | melhor via clone | Search academic literature using Semantic Scholar, arXiv, and OpenAlex APIs. Returns structured JSONL with title, authors, year, venue, abst |
| `math-reasoning` | melhor via clone | Formal mathematical reasoning for research papers — derive equations, write proofs, formalize problem settings, select statistical tests, an |
| `novelty-assessment` | melhor via clone | Assess research idea novelty through systematic literature search. Multi-round search-evaluate loops with harsh critic persona. Binary novel |
| `paper-assembly` | melhor via clone | Orchestrate the full paper pipeline end-to-end. Manage state propagation between phases (literature → plan → code → experiments → figures →  |
| `paper-compilation` | melhor via clone | Compile LaTeX papers to PDF with automatic error detection, chktex style checking, and citation/reference validation. Runs the full pdflatex |
| `paper-revision` | melhor via clone | Revise papers based on reviewer feedback. Map reviewer concerns to specific sections, apply targeted edits, run additional experiments if ne |
| `paper-to-code` | melhor via clone | Convert an ML research paper into a complete, runnable code repository. 3-stage pipeline from Paper2Code — Planning (UML + dependency graph) |
| `paper-writing-section` | melhor via clone | Write a specific section of an academic paper (Abstract, Introduction, Background, Related Work, Methods, Experiments, Results, Discussion/C |
| `rebuttal-writing` | melhor via clone | Write point-by-point rebuttals to reviewer comments. Extract concerns from reviews, generate evidence-based responses, and format as a struc |
| `related-work-writing` | melhor via clone | Write Related Work sections that compare and contrast prior work with your approach. Organize by theme, cite broadly, and explain how your w |
| `research-planning` | melhor via clone | Design research plans and paper architectures. Given a research topic or idea, generate structured plans with methodology outlines, paper st |
| `self-review` | melhor via clone | Automatically review an academic paper using the NeurIPS review form with three reviewer personas, ensemble scoring, and reflection refineme |
| `slide-generation` | melhor via clone | Convert a completed paper into presentation slides (Beamer LaTeX) or poster. Extract key figures, tables, equations, and create a narrative  |
| `survey-generation` | melhor via clone | Generate complete academic survey papers using multi-LLM parallel outline generation, RAG-based subsection writing, citation validation, and |
| `symbolic-equation` | melhor via clone | Discover scientific equations from data using LLM-guided evolutionary search (LLM-SR). Multi-island algorithm with softmax-based cluster sam |
| `table-generation` | melhor via clone | Generate publication-quality LaTeX tables from experimental results. Convert JSON/CSV data to booktabs-styled tables with bold best results, |

### SEO + GEO - AgricIDaniel/claude-seo (33 skills)

A skill `seo` e um roteador que chama o binario `bin/claude-seo` e 18 sub-agents. Solta na conta ela quebra. Instale como plugin.

| Skill | Situacao | Descricao |
|---|---|---|
| `seo` | melhor via plugin | Comprehensive SEO analysis for any website or business type. Full site audits, single-page analysis, technical SEO (crawlability, indexabili |
| `seo-ahrefs` | melhor via plugin | Ahrefs API analyst (extension). Reads referring domains, backlinks, organic keywords, and content explorer data via the tested @ahrefs/mcp@0 |
| `seo-audit` | melhor via plugin | Full website SEO audit with parallel subagent delegation. Crawls up to 500 pages, detects business type, delegates to up to 15 specialists ( |
| `seo-backlinks` | melhor via plugin | Backlink profile analysis: referring domains, anchor text distribution, toxic link detection, competitor gap analysis. Works with free APIs  |
| `seo-bing` | melhor via plugin | Bing Webmaster Tools + IndexNow extension. Microsoft Copilot citations are fed by the Bing index; this skill makes Bing visibility, link dat |
| `seo-cluster` | melhor via plugin | SERP-based semantic topic clustering for content architecture planning. Groups keywords by actual Google SERP overlap (not text similarity), |
| `seo-competitor-pages` | melhor via plugin | Generate SEO-optimized competitor comparison and alternatives pages. Covers "X vs Y" layouts, "alternatives to X" pages, feature matrices, s |
| `seo-content` | melhor via plugin | Content quality and E-E-A-T analysis with AI citation readiness assessment. Use when user says "content quality", "E-E-A-T", "content analys |
| `seo-content-brief` | melhor via plugin | Generate competitive SEO content briefs with per-section word counts, competitor scoring, keyword density guidance, and page-type templates. |
| `seo-dataforseo` | melhor via plugin | Live SEO data via DataForSEO MCP server: SERP analysis, keyword research (volume, difficulty, intent, trends), backlink profiles, on-page an |
| `seo-dataforseo` | melhor via plugin | Live SEO data via DataForSEO MCP server: SERP analysis, keyword research (volume, difficulty, intent, trends), backlink profiles, on-page an |
| `seo-drift` | melhor via plugin | SEO drift monitoring: capture baselines of SEO-critical elements, detect changes, and track regressions over time. Git for SEO: baseline, di |
| `seo-ecommerce` | melhor via plugin | E-commerce SEO analysis: Google Shopping visibility, Amazon marketplace intelligence, product schema validation, competitor pricing analysis |
| `seo-firecrawl` | melhor via plugin | Full-site crawling, scraping, and site mapping via Firecrawl MCP. Use when user says "crawl site", "map site", "full crawl", "find all pages |
| `seo-flow` | melhor via plugin | FLOW framework integration: evidence-led SEO using the Find → Leverage → Optimize → Win loop. Surfaces stage-specific AI prompts from the FL |
| `seo-geo` | melhor via plugin | Optimize content for AI Overviews (formerly SGE), ChatGPT web search, Perplexity, and other AI-powered search experiences. Generative Engine |
| `seo-google` | melhor via plugin | Google SEO APIs: Search Console (Search Analytics, URL Inspection, Sitemaps), PageSpeed Insights v5, CrUX field data with 25-week history, I |
| `seo-hreflang` | melhor via plugin | Hreflang and international SEO audit, validation, and generation. Detects common mistakes, validates language/region codes, and generates co |
| `seo-image-gen` | melhor via plugin | AI image generation for SEO assets: OG/social preview images, blog hero images, schema images, product photography, infographics. Powered by |
| `seo-image-gen` | melhor via plugin | AI image generation for SEO assets: OG/social preview images, blog hero images, schema images, product photography, infographics. Powered by |
| `seo-images` | melhor via plugin | Image optimization analysis for SEO and performance. Checks alt text, file sizes, formats, responsive images, lazy loading, CLS prevention,  |
| `seo-local` | melhor via plugin | Local SEO analysis covering Google Business Profile optimization, NAP consistency, citation health, review signals, local schema markup, loc |
| `seo-maps` | melhor via plugin | Maps intelligence for local SEO: geo-grid rank tracking, GBP profile auditing via API, review intelligence across Google/Tripadvisor/Trustpi |
| `seo-page` | melhor via plugin | Deep single-page SEO analysis covering on-page elements, content quality, technical meta tags, schema, images, and performance. Use when use |
| `seo-plan` | melhor via plugin | Strategic SEO planning for new or existing websites. Industry-specific templates, competitive analysis, content strategy, and implementation |
| `seo-profound` | melhor via plugin | Profound LLM citation tracker (extension). Time-series brand citation rates across ChatGPT, Perplexity, and other LLMs. Pairs with seo-seran |
| `seo-programmatic` | melhor via plugin | Programmatic SEO planning and analysis for pages generated at scale from data sources. Covers template engines, URL patterns, internal linki |
| `seo-schema` | melhor via plugin | Detect, validate, and generate Schema.org structured data. JSON-LD format preferred. Use when user says "schema", "structured data", "rich r |
| `seo-seranking` | melhor via plugin | SE Ranking AI visibility analyst (extension). Tracks AI Share-of-Voice across ChatGPT, Gemini, Perplexity, AI Overviews, and AI Mode in a si |
| `seo-sitemap` | melhor via plugin | Analyze existing XML sitemaps or generate new ones with industry templates. Validates format, URLs, and structure. Use when user says "sitem |
| `seo-sxo` | melhor via plugin | Search Experience Optimization: reads Google SERPs backwards to detect page-type mismatches, derives user stories from search intent signals |
| `seo-technical` | melhor via plugin | Technical SEO audit across 9 categories: crawlability, indexability, security, URL structure, mobile, Core Web Vitals, structured data, Java |
| `seo-unlighthouse` | melhor via plugin | Multi-page Lighthouse audit via the MIT-licensed Unlighthouse CLI. Free-tier alternative to running PageSpeed against every URL on a site, n |

### Video por codigo (Remotion) - remotion-dev/skills (12 skills)

Precisam de um projeto Node/Remotion pra renderizar. Sem repo aberto nao produzem video.

| Skill | Situacao | Descricao |
|---|---|---|
| `remotion-best-practices` | precisa projeto Remotion | Router for all Remotion skills |
| `remotion-captions` | precisa projeto Remotion | Transcribing, displaying and animating captions |
| `remotion-create` | precisa projeto Remotion | Create a new Remotion video |
| `remotion-docs` | precisa projeto Remotion | Search Remotion documentation |
| `remotion-interactivity` | precisa projeto Remotion | Structure Remotion markup for interactivity |
| `remotion-maps` | precisa projeto Remotion | Remotion Map animation knowledge |
| `remotion-markup` | precisa projeto Remotion | Content, animation and effects best practices |
| `remotion-multimedia` | precisa projeto Remotion | Interacting with Mediabunny |
| `remotion-render` | precisa projeto Remotion | Export a Remotion video |
| `remotion-saas` | precisa projeto Remotion | Build an app with Remotion |
| `remotion-studio` | precisa projeto Remotion | Preview a Remotion video |
| `remotion-upgrade` | precisa projeto Remotion | Upgrade Remotion, and related packages |

### Ads / Hyper - hyperfx-ai/marketing-skills (30 skills)

As 30 dependem do Hyper MCP (https://www.hyperfx.ai/mcp) pra ter qualquer ferramenta. Sem o MCP conectado, sao inertes.

| Skill | Situacao | Descricao |
|---|---|---|
| `ad-creative-generation` | precisa Hyper MCP | Generate on-brand ad creatives — visuals + copy — for Google, Meta (Facebook / Instagram), and other paid platforms via the Hyper MCP. Extra |
| `amazon-ads` | precisa Hyper MCP | Plan and create Amazon Sponsored Products campaigns end-to-end via the Hyper MCP. Use when the user wants to launch Amazon Ads, set up Spons |
| `analytics-insights` | precisa Hyper MCP | Drive Google Analytics (GA4), Google Tag Manager, Google Search Console, and BigQuery from chat — tracking plans, GA4 reports, key-event (co |
| `blog-generation` | precisa Hyper MCP | Generate one excellent, on-brand blog post per run for any business, built to rank on Google and get cited by AI search (ChatGPT, Claude, Pe |
| `brand-context` | precisa Hyper MCP | Create and maintain a single brand-context.md — positioning, audience, personas, pain points, customer language, voice, proof points — that  |
| `cold-email-outreach` | precisa Hyper MCP | Run end-to-end B2B cold-email outreach through the Hyper MCP — enrich prospects with Apollo, scrape per-prospect signals from company sites  |
| `competitor-intel` | precisa Hyper MCP | Run end-to-end competitor research and monitoring through the Hyper MCP — pick the set, scrape every public surface (site, blog, pricing, or |
| `customer-research` | precisa Hyper MCP | Mine online communities and analyze existing assets to understand what customers actually think, say, and struggle with. Use when the user w |
| `email-lifecycle` | precisa Hyper MCP | Plan, build, and run lifecycle email programs through the Hyper MCP — welcome / onboarding, nurture, re-engagement, win-back, and abandoned- |
| `gmail` | precisa Hyper MCP | Manage Gmail end-to-end — send, reply, search, drafts, labels, attachments, and inbox organization. Use when the user wants to send or reply |
| `google-ads` | precisa Hyper MCP | Plan and create new Google Ads campaigns and report on existing accounts via the Hyper MCP. Use when the user wants to launch Search, Displa |
| `google-sheets` | precisa Hyper MCP | Safe workflow for reading, mapping, and writing Google Sheets without shifting columns or overwriting the wrong ranges. Use when the user wa |
| `hyper-cli` | precisa Hyper MCP | Use the Hyper CLI to run Hyper marketing skills from a terminal. Use when the user wants to use `hyperai`, inspect live tool schemas, transl |
| `image-generation` | precisa Hyper MCP | Generate images through the Hyper MCP with the unified `images_generate` tool — text-to-image, image-to-image, and branded ad creatives — ch |
| `instagram` | precisa Hyper MCP | Manage Instagram professional accounts via the Hyper MCP — publish photos, Reels, Stories, and carousels; moderate comments and mentions; se |
| `linkedin` | precisa Hyper MCP | Publish and manage LinkedIn content via the Hyper MCP — text posts, article / link previews, document and PDF posts, organization (company p |
| `meta-ads` | precisa Hyper MCP | Plan and create Meta (Facebook + Instagram) advertising campaigns end-to-end via the Hyper MCP, defaulting to Advantage+ automation. Use whe |
| `meta-ads-library` | precisa Hyper MCP | Research competitor Facebook and Instagram ads from the Meta Ads Library via the Hyper MCP — search by keyword, pull full ad creative and me |
| `openai-ads` | precisa Hyper MCP | Plan and manage OpenAI Ads (ChatGPT ads) campaigns end-to-end via the Hyper MCP — API-key auth, account discovery, geo targeting, image uplo |
| `pinterest-ads` | precisa Hyper MCP | Plan and create Pinterest Ads campaigns through the Hyper MCP — Awareness, Consideration, Video View, Web Conversion, Catalog Sales, and Web |
| `reddit` | precisa Hyper MCP | Research Reddit discussions with high signal using scrape_reddit_leads and scrape_reddit — pain points, intent discovery, and trend tracking |
| `reddit-ads` | precisa Hyper MCP | Plan and create Reddit Ads campaigns end-to-end via the Hyper MCP — campaign, ad group, ad build order with subreddit / interest / geo targe |
| `seo-research` | precisa Hyper MCP | Data-driven SEO research and analysis through the Hyper MCP — keyword research, competitor analysis, content planning, AI search visibility  |
| `slack` | precisa Hyper MCP | Slack messaging, file sharing, Block Kit formatting, and channel management. Use when the user wants to send Slack messages, post rich Block |
| `snapchat-ads` | precisa Hyper MCP | Plan and create Snapchat Ads campaigns end-to-end via the Hyper MCP — campaign, ad squad, ad build order with media upload, creatives, targe |
| `tiktok` | precisa Hyper MCP | Publish organic TikTok content (videos, photos, carousels) through the TikTok-compliant interactive posting form via the Hyper MCP. Use when |
| `tiktok-ads` | precisa Hyper MCP | Plan and create TikTok advertising campaigns end-to-end via the Hyper MCP, with strict parameter validation for objective-specific requireme |
| `twilio` | precisa Hyper MCP | Twilio messaging, voice, phone number management, and verification workflows. Use when the user wants to send SMS or WhatsApp messages, make |
| `video-generation` | precisa Hyper MCP | End-to-end AI video production through the Hyper MCP — text-to-video and image-to-video generation (Sora, Veo, Seedance), scene chaining, vi |
| `youtube` | precisa Hyper MCP | Work with YouTube content end to end — fetch transcripts and turn them into summaries, blog posts, social content, quotes, or show notes; cr |


## Procedencia

Clonado em 2026-08-22 (`git clone --depth 1`), commit de origem:

| Repo | Commit | Licenca |
|---|---|---|
| `anthropics/skills` | `3b3fad9` | ver repo |
| `blader/humanizer` | `e2e92e7` | LICENSE |
| `AgricIDaniel/claude-seo` | `09d37c7` | LICENSE |
| `remotion-dev/skills` | `baf0b91` | ver repo |
| `lingzhi227/agent-research-skills` | `9e6c085` | ver repo |
| `hyperfx-ai/marketing-skills` | `8b5012e` | LICENSE |
| `coreyhaines31/marketingskills` | `3df87f9` | LICENSE |

Conteudo de terceiros, redistribuido aqui so pra facilitar o upload. Cada zip carrega o LICENSE do repo de origem quando ele existe.

**Unica modificacao feita:** nas 16 skills de `coreyhaines31/marketingskills` que liam `../../tools/*.md`, os arquivos referenciados foram copiados pra dentro do zip e o caminho reescrito de `../../tools/` pra `tools/`. Sem isso a skill perde os anexos ao ser enviada sozinha. Nenhum outro arquivo foi alterado.
