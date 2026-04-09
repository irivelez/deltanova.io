# AI agents are replacing consultants, not just advising them

**The most disruptive shift in IT services isn't a better tool — it's a new category of company where AI agents perform the actual work.** Startups like Cognition Labs (Devin), Factory AI, and Resolve AI have demonstrated that autonomous agents can write production code, manage infrastructure, and resolve incidents with minimal human involvement, generating real revenue at unprecedented speed. Cognition grew from **$1M to $73M ARR in nine months**. Sequoia Capital's landmark thesis calls this "the next trillion-dollar opportunity," arguing that for every dollar spent on software, six are spent on services — and AI is coming for that labor budget. But production reliability data tells a more sobering story: 68% of deployed agents execute fewer than 10 steps before requiring human intervention, and the Klarna case proved that pure cost-driven automation destroys quality. The companies winning are those treating human oversight as a design choice, not a fallback. For LATAM, this represents both an existential threat to traditional outsourcing and a once-in-a-generation opportunity to pivot from selling headcount to selling AI-augmented outcomes.

---

## The startup landscape splits into five battlegrounds

The AI-driven IT services market has produced distinct categories of companies, each attacking a different slice of the **$6-of-services-for-every-$1-of-software** opportunity that Sequoia's Julien Bek identified in March 2026.

**Autonomous coding agents** represent the most funded category. Cognition Labs' Devin, the first widely deployed autonomous AI software engineer, handles migrations, test writing, code review, and feature development in a sandboxed workspace. Its combined ARR with the acquired Windsurf IDE reached an estimated **$150M+ by mid-2025**, with clients including Goldman Sachs, Citi, Dell, and Nubank. Factory AI's "Droids" take a model-agnostic approach to automating the full software development lifecycle, ranking #1 on Terminal Bench and claiming 31x faster delivery for enterprise customers. Backed by **$70M from NEA and Sequoia**, Factory serves Ernst & Young, Nvidia, and MongoDB. Cosine AI's Genie, a YC W23 graduate from London, achieved 30% on SWE-Bench at launch — more than double Devin's initial score — but remains early-stage with only $2.5M in seed funding.

**AI DevOps and infrastructure** is maturing fast. DuploCloud launched AI DevOps Engineers in December 2025 that provision, troubleshoot, and optimize infrastructure on AWS, Azure, and GCP within safety guardrails, backed by **$49.5M** in total funding. AlertD, founded by former Cisco and Splunk architects, emerged from stealth in November 2025 with a $3M pre-seed from True Ventures, positioning specialized SRE agents as "Slack for production uptime."

**AI-driven IT operations** produced the space's newest unicorn. Resolve AI reached a **$1B valuation with its $125M Series A** in December 2025, led by Lightspeed, building autonomous Site Reliability Engineers that triage alerts, perform root cause analysis, and resolve incidents. Its angel investors include Fei-Fei Li and Jeff Dean. Competitor Traversal raised **$48M from Kleiner Perkins and Sequoia**. Both target the critical shortage of skilled SREs, with Rootly offering a "progressive autonomy" model that starts advisory and expands to autonomous execution as trust builds.

**AI QA and testing** companies like Momentic (YC-backed, $15M Series A), Spur (which delivered "95% reduction in manual QA time" for Eight Sleep before Black Friday), and Functionize (99.97% element recognition accuracy over 8 years) demonstrate that testing is among the most automation-ready domains.

**AI data engineering** rounds out the landscape, with TensorStax building self-healing data pipelines and Ascend.io claiming "10x faster at 83% of the cost" for pipeline construction through natural language descriptions.

| Company | Category | Total Funding | Latest Valuation | ARR/Revenue |
|---------|----------|--------------|-----------------|-------------|
| Anysphere (Cursor) | AI IDE | ~$3.4B | $29.3B | ~$2B (est. Mar 2026) |
| Cognition (Devin) | Autonomous coding | ~$696M | $10.2B | ~$155M combined |
| Poolside AI | Code generation models | ~$626M | $12B (reported) | ~$50M |
| Lovable | AI app builder | ~$553M | $6.6B | ~$400M (Mar 2026) |
| Replit | AI IDE + Agent | ~$350M+ | $9B (reported) | $240M |
| Augment Code | Enterprise coding | $252M | $977M | ~$20M |
| Distyl AI | AI consulting platform | ~$202M | $1.8B | Not disclosed (5-8x growth) |
| Resolve AI | Autonomous SRE | >$150M | $1B | ~$4M |
| Factory AI | Autonomous coding | $70M | $300M | Not disclosed |
| All Hands (OpenHands) | Open-source agents | $23.8M | Not disclosed | Open source |

---

## Pricing has converged on a hybrid model with a looming repricing crisis

The industry has settled on **hybrid subscription-plus-usage pricing** as the dominant model, but a fundamental tension threatens the economics. Devin charges $20/month on its Core plan with Agent Compute Units at $2.25 each (roughly **$8–9 per hour of active AI work**), while its Team plan runs $500/month with 250 ACUs included. Factory AI uses token-based billing starting at $20/month with cached token discounts. For comparison, a US developer costs $100–200/hour and Indian outsourcing runs $25–50/hour — making AI agents dramatically cheaper per unit of work.

Outcome-based pricing remains nascent but growing. Intercom's Fin AI charges **$0.99 per resolved customer ticket**. Salesforce Agentforce charges $2 per conversation. Gartner projected that 30%+ of enterprise SaaS solutions would incorporate outcome-based components by 2025, but adoption has been slower than expected. Even McKinsey — the gold standard of consulting — has only **25% of its fees globally linked to outcomes**; the rest remains traditional billing.

The deeper economic challenge is what analyst Linas Beliūnas calls **"the $0.03 problem"**: for every dollar companies stop spending on humans, they spend only three cents on AI. When machines do the work, budgets don't transfer to AI vendors — they evaporate. This threatens the entire "capture the labor budget" thesis that VCs are betting on. AI company gross margins sit at **50–60%** according to a16z's analysis — below traditional SaaS (60–80%) but above services (30–40%). Many fast-growing AI startups operate at negative gross margins, subsidized by venture capital. Anthropic reportedly loses tens of thousands of dollars per month on individual heavy Claude Code users paying $200/month. Revenue per employee, however, can be extraordinary: Mercor achieves **$4.5M per employee** versus Microsoft's $1.8M.

---

## Production reliability is the hard constraint nobody can ignore

The gap between demo performance and production reliability defines the current moment. UC Berkeley's MAP research, surveying 300+ teams with agents in production, found that **68% of agents execute fewer than 10 steps** before requiring human intervention, and 92.5% of production agents deliver output to humans rather than to other systems. Organizations deliberately constrain agent autonomy to maintain reliability.

The math is unforgiving. If each step in a workflow has 95% reliability — an optimistic assumption — a 20-step chain yields only **36% end-to-end success**. Cleanlab's production survey found that regulated enterprises rebuild their AI agent stack every three months or faster. Only 95 out of 1,837 respondents reported having agents live in production. Fortune 500 failure rates tell a stark story: **73% of enterprise AI agent deployments** experience reliability failures within the first year, and 42% of companies abandoned most AI initiatives in 2025, up from 17% in 2024.

The Klarna case became the industry's defining cautionary tale. Klarna's AI assistant handled **700 human agents' worth of workload** across 2.3 million conversations, projecting $40M in profit improvement. CEO Sebastian Siemiatkowski later admitted that "cost was a too predominant evaluation factor... what you end up having is lower quality." The company saw 25% more repeat inquiries from bot failures, customers couldn't resolve nuanced issues, and AI responses sounded like "GPT, not Klarna." Klarna is now rehiring human agents for complex interactions. The lesson, per Princeton researchers: "An agent that succeeds on 90% of tasks but fails unpredictably on the remaining 10% may be a useful assistant yet an unacceptable autonomous system."

---

## How the oversight layer actually works in practice

Companies winning in this space structure human involvement along a **risk-based autonomy framework** rather than blanket oversight. The pattern that has emerged across successful deployments segments work into three tiers. Full automation covers testing, code formatting, documentation generation, and routine monitoring — tasks where errors are cheap to fix. AI-first with human escalation handles feature implementation, bug fixes, CI/CD automation, and incident triage — tasks where agents propose and humans approve. Human-required work encompasses security-critical code, compliance decisions, architectural changes, and production deployments — tasks where errors are expensive or irreversible.

Cognition's Devin exemplifies this through "Interactive Planning": the agent proposes an execution plan, the human approves it, and Devin works autonomously within that approved scope, creating pull requests for human review before merge. Factory AI positions its Droids similarly — agents handle "tedious" SDLC tasks while engineers make high-level decisions. Resolve AI starts in advisory mode and expands to autonomous remediation only for low-risk scenarios, building trust progressively.

The traditional consulting giants are adapting faster than expected. **PwC launched PwC One in March 2026** — an agentic platform where clients log in directly, describe a problem, and AI agents perform the work while human consultants review outputs in the background. McKinsey has deployed roughly **12,000 internal AI agents**, with its Lilli platform handling 500,000 queries per month and performing approximately 80% of a junior analyst's typical research and slide-generation work. McKinsey's headcount is down 25% from its peak, with further cuts planned. Accenture has secured **$3.6B in annualized generative AI bookings** and employs 70,000 AI professionals. Sia Partners grew from 50 to 400+ AI agents on its internal Agent Store. BCG reports that hybrid teams combining human consultants with AI deliver projects **35% faster**.

---

## LATAM faces an existential pivot from headcount to outcomes

Latin America's $19.5 billion IT outsourcing market sits at a critical inflection point. The region's traditional value proposition — high-quality developers at 40–54% lower cost than US equivalents, with timezone alignment and cultural affinity — is being simultaneously validated and threatened by AI automation. When an AI coding agent costs **$8–9/hour** versus $60–80/hour for a senior LATAM bilingual developer, the pure cost arbitrage narrative weakens for routine work.

**Globant is the bellwether** for how LATAM firms can navigate this transition. The $2.5B-revenue, NYSE-listed Argentine company launched AI Pods in 2025 — a subscription-based delivery model combining autonomous AI agents with human oversight, offering "engineering on demand, powered by AI and orchestrated by Globant." Its proprietary GEAI platform (version 2.3) integrates Model Context Protocol and Agent-to-Agent protocols, with 50+ certified AI agents available through its internal marketplace called The Station. Globant has deliberately diversified its geographic footprint — Argentina now represents just 17% of headcount, down from 69% in 2014.

**Indicium AI** represents the LATAM-origin consulting model successfully going global. Founded in Florianópolis, Brazil in 2017, it raised $40M from Columbia Capital and merged with UK-based Mesh-AI in November 2025 to form one of the world's leading data and AI consultancies, with 400+ certified professionals and clients including PepsiCo and Bayer. **Nubank** demonstrates AI's transformative potential for LATAM companies internally: its OpenAI-powered assistant handles 2M+ monthly chats, resolves 55% of Tier 1 inquiries autonomously, and maintains a $0.70–0.80 cost-to-serve per customer — versus 50–70% cost-to-income ratios at traditional LATAM banks.

The LATAM ecosystem shows growing momentum. VC funding reached **$4.1B across 681 rounds in 2025**, up 13.8% year-over-year, with Mexico surging 53% to $1.1B. Brazil-based and Mexican AI startups raised over $300M combined. Google launched a dedicated AI First accelerator for Latin America. Key hubs include São Paulo (LATAM's tech capital), Mexico City (which surpassed Brazil in quarterly VC for the first time since 2012 in Q2 2025), Buenos Aires (deep engineering talent and Globant's home), Medellín (350+ multinationals), and Santiago (home to Chile's National Center for AI and the Start-Up Chile accelerator with $2.1B in portfolio value).

The strategic opportunity lies in what industry observers call **"Nearshore 2.0"** — transitioning from labor arbitrage to AI expertise. LATAM's Global Business Services operations already perform more complex functions than Asian peers: 64% handle data analytics (versus 34% globally) and 59% handle intelligent automation (versus 28%). The companies that will thrive are those integrating AI agents into delivery while retaining human expertise for judgement, client relationships, and domain knowledge. Those still selling pure headcount face existential risk as AI agents compress the value of routine development work.

---

## The $6-to-$1 thesis meets the $0.03 reality

Sequoia's Julien Bek framed the opportunity memorably: "If you sell the tool, you're in a race against the model. But if you sell the work, every improvement in the model makes your service faster, cheaper, and harder to compete with." YC now explicitly requests **"AI-Native Agencies"** and envisions "the first 10-person, $100 billion company." General Catalyst committed **$1.5 billion to acquiring traditional service businesses and rebuilding them with AI**. The VC consensus is so complete that, as one observer noted, "you could swap the logos on their published theses and most readers wouldn't notice."

Yet the evidence from production deployments reveals five critical lessons. First, **narrow beats broad**: the companies with real traction (Devin for junior coding tasks, Resolve AI for incident triage, Momentic for QA) succeed by constraining their agents to well-defined domains where outsourcing already exists and buyers are accustomed to purchasing outcomes. Second, **trust compounds slowly**: Rootly's progressive autonomy model — start advisory, earn trust, expand scope — outperforms the "replace everything at once" approach that burned Klarna. Third, **the repricing problem is real**: when machines do work previously done by humans, clients expect machine-rate pricing, potentially collapsing the addressable market from trillions to billions. Fourth, **human-in-the-loop is a feature, not a bug**: 92.5% of production agents output to humans, and the most successful companies design this deliberately rather than treating it as a limitation to overcome. Fifth, **margins are uncertain**: current AI pricing is heavily subsidized by venture capital, and multiple analysts warn that cost-reflective pricing could require $200–2,000/month subscriptions instead of $20, fundamentally changing the accessibility equation.

The market is projected to grow at **46.3% CAGR** for AI agents specifically, from $7.8B in 2025 to $52.6B by 2030. But Gartner predicts 40% of agentic AI projects will be canceled by 2027 due to escalating costs, unclear business value, or inadequate risk controls. The winners will be companies that master the paradox at the center of this market: using AI to do the work while maintaining enough human judgement to ensure the work is worth doing.