# Awesome-Conversation-Intelligence-Speech-Analytics

# Awesome-Conversation-Intelligence-Speech-Analytics

**Top Conversation Intelligence Speech Analytics (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Call Scoring, Speech-to-Text, Speaker Diarization & Self-Hosted Revenue Intelligence*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Conversation Intelligence & Speech Analytics**. These tools enable sales and support teams to transcribe calls, score conversations against playbooks, detect objections, and surface coaching insights—from fully managed enterprise platforms with proprietary AI models to self-hosted alternatives that give organizations full control over sensitive call recordings and LLM provider choice.



**Examples** include Gong, Chorus by ZoomInfo, Salesloft, Clari Copilot, Avoma, Attention, Balto, CallMiner, Invoca, and HubSpot Conversational Intelligence (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted conversation intelligence, speech recognition, and open audio analytics. **Critical note**: The open-source CI landscape is young but growing—**Playcall** is the most direct Gong alternative with playbook-aware scoring and multi-LLM support , while **GTM Superintelligence** offers a Claude-native skill approach for coaching without API keys . For the speech foundation, **FunASR** provides industrial-grade transcription with speaker diarization and emotion detection , and **CXMind** delivers real-time VoIP analytics for contact centers . No open-source project matches Gong's integration depth or enterprise polish, but for teams willing to self-host and tune, the core capabilities are achievable.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Gong](https://www.gong.io/)**

  **The category leader in revenue intelligence** with call recording, transcription, deal scoring, and forecasting. **Pricing**: Quote-only; contracts commonly run into thousands of dollars per rep per year . **Free tier**: None. **Best for**: enterprises wanting the most mature conversation intelligence with deep CRM integrations and proven AI models—**trade-off**: expensive, cloud-only, and scoring logic is a black box .



- **[Chorus by ZoomInfo](https://www.zoominfo.com/)**

  **Conversation intelligence** integrated with ZoomInfo's B2B data. **Pricing**: Quote-only. **Free tier**: None. **Best for**: ZoomInfo customers wanting call intelligence alongside prospect data—**trade-off**: proprietary, subscription-priced, not self-hostable .



- **[Salesloft](https://www.salesloft.com/)**

  **Revenue orchestration** with conversation intelligence and coaching. **Pricing**: Quote-only. **Free tier**: None. **Best for**: sales teams wanting cadences and call intelligence in one platform.



- **[Clari Copilot](https://www.clari.com/)**

  **Conversation intelligence** within Clari's revenue platform. **Pricing**: Quote-only. **Free tier**: None. **Best for**: Clari customers wanting call insights alongside forecasting.



- **[Avoma](https://www.avoma.com/)**

  **AI meeting assistant and conversation intelligence** with CRM sync and coaching. **Pricing**: Tiered per-user; quote-based for enterprise. **Free tier**: Limited. **Best for**: teams wanting meeting transcription and call scoring in one tool.



- **[Attention](https://www.attention.tech/)**

  **AI sales coaching** with automated call scoring and CRM integration. **Pricing**: Quote-only. **Free tier**: None. **Best for**: sales orgs wanting automated coaching at scale.



- **[Balto](https://www.balto.ai/)**

  **Real-time guidance and conversation analytics** for contact centers. **Pricing**: Quote-only. **Free tier**: None. **Best for**: contact centers wanting live agent coaching.



- **[CallMiner](https://callminer.com/)**

  **Enterprise speech analytics** for contact centers with compliance and quality monitoring. **Pricing**: Quote-only. **Free tier**: None. **Best for**: large contact centers needing 100% call inspection.



- **[Invoca](https://www.invoca.com/)**

  **Call tracking and conversation intelligence** for marketing and sales. **Pricing**: Quote-only. **Free tier**: None. **Best for**: marketing teams wanting call attribution and conversation insights.



- **[HubSpot Conversational Intelligence](https://www.hubspot.com/)**

  **Call intelligence within HubSpot** Sales Hub. **Pricing**: Included with Sales Hub tiers. **Free tier**: Limited. **Best for**: HubSpot users wanting basic call transcription and coaching within their CRM.



## Open-Source GitHub Projects



- **[Playcall](https://github.com/Dphenomenal101/playcall)**

  **Open-source AI alternative to Gong** (MIT) — **the most direct open-source Gong replacement**, designed to score every call against your playbook and buyer context . **Features**: **Playbook-aware scoring**—MEDDPICC, BANT, SPIN, or custom methodology, with evidence-backed scores rather than generic AI advice . **Multi-LLM flexibility**—OpenAI, Anthropic, Gemini, Mistral, Groq, Cohere, Perplexity, and Together AI, with BYOK per workspace . **Loss-reason analysis** grounded in actual dialogue; **objection-pattern detection** across calls; **buyer-aware scoring** adjusting for company stage and contact role . **Tech stack**: Next.js 16, Supabase (Postgres, Auth, RLS), Vercel AI SDK, OpenAI Whisper for transcription, LlamaParse for document parsing . **Deploy**: Self-hosted (Supabase + Vercel) with full setup instructions . **Trade-off**: **Young project without enterprise track record**—no visible native CRM/dialer/calendar integrations, no commercial support or SLA . **Best for**: startups and mid-size sales orgs with engineering capacity wanting Gong-style coaching without $30K/year contracts—willing to self-host and tune.



- **[GTM Superintelligence](https://github.com/attentiontech/gtm-superintelligence)**

  **Open-source GTM intelligence and automation for any sales call** (license per repo) — **the most flexible open-source coaching framework**, shipping as a **Claude Code skill + subagents + slash commands** . **Features**: **Three layers of scoring**—call-level (rep/CSM coaching), deal-level (MEDDPICC/SPICED-grounded health scoring), and account-level (CSM adoption/churn risk) . **Coaching inbox**—prioritized "what to improve" digest aggregated from many call reports, deterministic prioritization (frequency × impact) . **30 post-call agents** for CRM sync, task creation, and automation . **No API key required**—runs inside Claude Code, reading YAML rubrics and transcripts directly . **Tech stack**: Claude Code skill, YAML rubrics, CLI (`gtmsi`). **Deploy**: Local (Claude Code) or managed Claude agents on your stack . **Trade-off**: **Claude Code dependency**—designed around Anthropic's agent environment; not a traditional web app. **Best for**: teams already using Claude wanting structured, multi-layer call and deal coaching without building or paying for a separate platform.



- **[FunASR](https://github.com/modelscope/FunASR)**

  **Industrial-grade speech recognition toolkit** (license per repo, ~18.5K stars) — **the most production-ready open-source speech foundation** for conversation intelligence pipelines . **Features**: **170× real-time transcription** across 50+ languages; **speaker diarization** (who spoke when); **emotion detection** (acoustic cues); streaming support; **OpenAI-compatible API** and **MCP server** for easy integration with AI assistants . **Tech stack**: Python, PyTorch. **Deploy**: Docker image, Python package, CLI, or REST/WebSocket streaming . **Trade-off**: **Speech layer only**—no call scoring, playbook analysis, or CI workflow. Requires building the intelligence layer on top. **Best for**: developers wanting a fast, multilingual, production-grade transcription and diarization engine as the foundation for a custom conversation intelligence pipeline.



- **[CXMind](https://github.com/Sonicwell/cxmind)**

  **Open-source real-time VoIP analytics platform** (BSL 1.1, converts to Apache 2.0 in 2030) — **the most complete open-source contact center intelligence stack** . **Features**: **Non-invasive**—passively captures SIP/RTP via HEP tapping, zero changes to PBX . **Real-time call analytics**, quality monitoring, and **live transcription**; **AI-powered agent assistance** via Chrome extension copilot . **Open-source components**: Ingestion Engine (Go), Sniffer (Go), Admin UI (React), Copilot Extension (React) . **Performance**: 4-core, 8GB instance processes **300+ concurrent SIP/RTP calls** with CPU under 60% . **Tech stack**: Go, React, ClickHouse, MongoDB, Redis. **Deploy**: Docker Compose (`docker-compose.community.yml`) . **Trade-off**: **BSL license**—free for internal production, but cannot offer as competing hosted service until 2030 . **CXAI (emotion/NLP microservice) is still in development** . **Best for**: contact centers wanting real-time VoIP analytics and agent assistance without disrupting existing telephony—especially those already using AsterCC or SIP-based PBX.



- **[transcribe-diarize-emote](https://pypi.org/project/transcribe-diarize-emote/)**

  **One-stop audio intelligence pipeline** (PyPI package) — **the simplest path from audio to LLM-ready conversation transcripts** . **Features**: **Transcription** (faster-whisper, large-v3 recommended); **speaker diarization** (diarizer-lite); **acoustic emotion enrichment** (pitch and loudness metrics per speaker) . **Offline capable, no API keys required**; CPU supported by default, CUDA GPU acceleration . Outputs VTT with speaker tags and emotion context, directly usable for summarization, sentiment analysis, and coaching . **Tech stack**: Python (`pip install transcribe-diarize-emote`). **Deploy**: Local Python pipeline . **Trade-off**: **Pipeline library, not a platform**—no UI, no scoring, no CRM integration. Emotion layer is optional but adds processing time. **Best for**: developers wanting a ready-made audio-to-LLM-transcript pipeline for building custom conversation intelligence on top.



### Additional Strong Open-Source Options



- **ml-voice-lead-analysis** — End-to-end ML pipeline for sales cold calls (license per repo). Transcribes and analyzes calls for lead qualification, deal risk flags, talk ratios, and sentiment trajectory; explainable scoring with exact quotes behind each component . **Note**: Focused on lead qualification, not full CI platform. **Best for**: sales teams wanting explainable lead scoring from call transcripts.

- **Sales-Coach (Yz613)** — Open-source Gong alternative (license per repo). Imports transcripts from Fathom, Fireflies, Aircall, Zoom, Teams, and Gong API; CRM exports to HubSpot/Pipedrive/Attio; coaching scores and next steps . **Note**: Integration-focused; core scoring less mature than Playcall. **Best for**: teams already using supported recorders wanting open-source coaching and CRM export.

- **whisper-speaker-emotion** — Emotion-aware speaker analysis library (PyPI). Pitch (F0) and loudness (RMS) aligned with Whisper diarized VTT . **Note**: Component library, not a CI tool. **Best for**: adding acoustic emotion context to existing transcripts.



**Frameworks for building custom systems**: Combine **FunASR** or **transcribe-diarize-emote** for transcription and diarization with **Playcall** for playbook scoring, **GTM Superintelligence** for multi-layer coaching and CRM agents, and **CXMind** for real-time VoIP analytics—creating a composable open-source CI stack. **None of these match Gong's integration depth or enterprise polish**, but for teams prioritizing data sovereignty and cost control, the core capabilities are achievable.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Conversation intelligence platforms handling call recordings and transcripts must comply with data protection regulations (GDPR, CCPA, etc.), call recording consent laws (two-party consent in some jurisdictions), and implement appropriate access controls.

- **The "full CI platform" vs. "coaching framework" vs. "speech foundation" vs. "VoIP analytics" distinction is critical.** **Gong, Chorus, Salesloft, Clari, Avoma, Attention, Balto, CallMiner, and Invoca** are **full CI platforms**—they record, transcribe, score, and integrate with CRMs. **Playcall** is an **open-source CI platform**—it scores against playbooks with multi-LLM support, but lacks native integrations . **GTM Superintelligence** is a **coaching framework**—it runs inside Claude Code and scores calls/deals/accounts, but is not a traditional web app . **FunASR and transcribe-diarize-emote** are **speech foundations**—they transcribe and diarize, but do not score or coach . **CXMind** is **VoIP analytics**—real-time contact center monitoring, not sales coaching . **Choose based on whether you need full CI, coaching, transcription, or contact center analytics.**

- **Playcall is the most direct open-source Gong replacement**—playbook-aware scoring, multi-LLM BYOK, and evidence-grounded analysis . **The trade-off**: young project with no enterprise track record, no native integrations, and no support SLA . **For engineering-capable startups wanting Gong-style coaching without the contract, it is the strongest option.**

- **GTM Superintelligence takes a fundamentally different approach**—it is a Claude Code skill, not a web app. You run `/coach` on a transcript and get structured scoring across call, deal, and account layers . **The trade-off**: Claude Code dependency; not a traditional multi-user platform. **For teams already using Claude, it is the fastest path to structured coaching without API keys.**

- **FunASR is the most production-ready speech foundation**—170× real-time, 50+ languages, diarization, emotion, and OpenAI-compatible API . **The trade-off**: speech only—you build the intelligence layer. **Pair it with Playcall or a custom scoring layer.**

- **CXMind is the most complete open-source contact center intelligence stack**—non-invasive VoIP capture, real-time analytics, and agent copilot . **The trade-off**: BSL license (not OSI open source until 2030); CXAI emotion detection still in development . **For contact centers wanting real-time VoIP analytics without PBX changes, it is the strongest option.**

- **Pricing opacity is universal across commercial CI vendors.** Gong, Chorus, Salesloft, Clari, Avoma, Attention, Balto, CallMiner, Invoca, and HubSpot (enterprise) all require sales contact for quotes. **Validate with direct vendor conversations against your rep count and call volume.**

- Self-hosted open-source solutions require proper infrastructure (GPU for Whisper/FunASR, Supabase for Playcall, Docker for CXMind), security hardening for call recordings, and ongoing maintenance. **Call recordings contain sensitive customer information**—ensure your deployment meets your organization's consent and privacy requirements before recording or processing live calls.



---



**Made for sales operations teams, revenue leaders, and organizations building transparent conversation intelligence solutions.**

Let's make Conversation Intelligence & Speech Analytics more open, data-driven, and coaching-friendly.
