# TasteAI Studio x Elastic — Turn Traffic Into Conversations

TasteAI Studio is a **production-grade conversational AI platform** for building, deploying, and scaling intelligent bots on your website—powered by **Elastic ES|QL and Elastic Agent Builder**, where each chatbot is backed by a dedicated Elastic agent with indexed documents for semantic search, intelligent query answering, and intent-based human handoff detection, enabling reliable, observable, human-in-the-loop workflows from day one.

We focus on one simple idea:
👉 **Bots should solve problems end-to-end with intelligent search and accurate query answering via Elastic — not break when things get complex.**
---

## Inspiration

## 🤖 When Bots Fail Quietly

Bots rarely fail with errors or crashes — they fail *silently*, right when users need them the most.

### 🍕 Food Delivery App: A Common Story

- User orders food after a long day 
- Delivery arrives late and cold  
- User opens customer support   
- A chatbot appears 
- User explains the issue  
- Bot responds with scripted replies 
- User asks for a human agent 
- Bot refuses and keeps looping  
- User feels unheard 
- Trust drops  
- User churns 

**Key problem:**  
When bots can’t understand intent or don’t know when to step aside, they stop helping and start blocking users.

---

## ⚕️ AI-Powered Medical App: When Escalation Matters

- User shares symptoms in an AI-powered medical app 
- App responds using data, models, and probabilities   
- Answers feel generic or incomplete  
- User concern increases  
- User asks to speak to a specialist 
- No clear escalation path 
- No button, no handoff  
- Automated responses repeat 
- User feels ignored and unsafe  

**Why this is critical:**  
In healthcare, the cost of being unheard is far higher than frustration.

---

## ❤️‍🩹 The Takeaway

- AI that tries to handle everything  
  → becomes a barrier  

- AI that knows **when to hand off to a human**  
  → becomes trustworthy support  

The best AI isn’t the one that answers every question — it’s the one that knows when a human expert needs to take over.

TasteAI Studio was built to fix this.

We wanted a system where:
- Bots handle **80–90% of conversations**
- Humans seamlessly step in when needed
- Teams can **observe, analyze, and improve** continuously
- Deployment is **one copy-paste away**
- Users can embed a chatbot on their website without technical knowledge in 5-6 minutes.
- Enabling human handoff intelligence seamlessly

---

## What It Does

## Bot Creation (No-Code + Pro-Level Control)

![Bot Creation – No-Code & Pro-Level Control](https://res.cloudinary.com/dlpozcdw7/image/upload/v1770572831/TasteAI_-_Bot_Creation_m3gvfj.jpg)

TasteAI Studio makes it easy to build **production-ready AI bots** using a no-code interface, while still offering **deep control** for advanced use cases.

Instead of overwhelming users with scattered settings, bot creation is organized into **clear, purpose-driven sections**. Each section contributes to building bots that are reliable, scalable, and safe for real users.

---

### Core Configuration Sections

| Feature / Section               | What Information User Adds                              | What This Section Does (Flow + Elastic Usage)                                                                                                                                                          |
| ------------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Basic Information**           | Bot name, description, PDF document                     | PDF → Text Extraction → Chunking (3000 chars) → Documents indexed in **Elastic** → Elastic Agent created via API → ES|QL + semantic search used → Bot answers directly from indexed document knowledge |
| **Website & Knowledge Sources** | Website URL, selected pages                             | URL → Subpages fetched → User selects pages → Scraping → Chunking → Indexed into Elastic → Linked Elastic Agent queries indexed data using intelligent search → Accurate answers from website content  |
| **Voice Bot**                   | Enable voice, mic permission                            | User speaks → Browser Speech-to-Text → Query sent to Elastic-backed Agent → Relevant indexed context retrieved → Response returned → Browser Text-to-Speech plays reply                                |
| **Video Bot (Avatar)**          | Image upload, avatar prompt                             | Image processed → Avatar generated → Stored securely → During conversations, responses are powered by Elastic Agent retrieving relevant indexed knowledge                                              |
| **Language Support**            | Supported languages                                     | User query (any language) → Intent detection → Elastic intelligent search retrieves relevant documents → Response generated → Delivered in user’s selected language                                    |
| **Persona & Behaviour**         | Tone, personality, rules, keywords                      | Persona configuration linked to bot → Elastic Agent respects defined rules while retrieving from indexed docs → Consistent and controlled responses                                                    |
| **Conversation Flow Builder**   | Messages, questions, branches, confirmations, custom JS | User input → Flow logic determines next step → If knowledge needed, Elastic Agent performs indexed search using ES|QL → Hybrid structured + AI-driven responses                                        |
| **Integrations (Slack)**        | Slack workspace, channel selection                      | Slack message → Webhook event → Request sent to Elastic-linked Agent → Indexed knowledge queried → Response returned to Slack channel                                                                  |
| **Human Handoff & Escalation**  | Agent emails, escalation rules                          | Intent detection via Elastic Agent → Escalation trigger → Session context retrieved from indexed data → Available agent assigned (round-robin) → Real-time human chat takeover                         |

---

## Bot Capabilities (Post-Creation)

Each bot comes with powerful lifecycle tools:

![Post Bot Creation Capabilities](https://res.cloudinary.com/dlpozcdw7/image/upload/v1770575144/tasteAI_-_Bot_Features_cfgdhf.jpg)

| Feature                         | What info / config user adds                                              | What happens & how Elastic helps                                                                                                                                                                         |
| ------------------------------- | ------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Share the Bot**               | No extra setup. User generates a public sharable link.                    | Shareable link generated → User interacts with bot → Elastic Agent queries indexed documents using intelligent search → Accurate responses returned instantly → Teams can validate bot behavior quickly. |
| **Integrate Bot on Website**    | Website URL(s), page selection, UI preferences, visual/CSS customization. | Pages & subdomains indexed in Elastic → Embed code generated → Bot appears as floating widget → Elastic Agent uses ES|QL + semantic search to answer live queries directly from indexed knowledge.       |
| **UI Customization**            | Theme colors, fonts, layout via visual editor or custom CSS.              | UI configurations applied instantly → Embedded widget reflects brand identity → Elastic-powered logic continues retrieving relevant results independently of UI changes.                                 |
| **Sessions Page**               | No manual input. Auto-tracks conversations.                               | Every conversation stored as a session → Context indexed in Elastic → Quick retrieval using ES|QL → Enables structured session review and fast search across conversations.                              |
| **Analytics Dashboard**         | Date range, filters (handoff, success rate, agent stats).                 | Conversation data indexed in Elastic → ES|QL used for querying metrics → Structured analytics + search-driven insights → Clear visibility into bot and human performance.                                |
| **Edit Bot**                    | Update data sources, persona, flows, integrations.                        | Updated data re-indexed in Elastic → Linked Elastic Agent refreshed automatically → Queries now use updated indexed documents without rebuilding the entire bot.                                         |
| **Test the Bot**                | Select test flow: Conversational / Agentic / Human Handoff.               | Test query sent → Elastic Agent performs semantic search across indexed documents → Most relevant results retrieved → Flow behaves exactly like production.                                              |
| **Conversational Flow Testing** | Predefined questions, confirmations, branches.                            | Flow logic executes → If knowledge lookup required, Elastic Agent retrieves relevant indexed data → Structured flow + intelligent search combined seamlessly.                                            |
| **Agentic Query Flow**          | Knowledge sources (PDF, website, docs).                                   | User query → Elastic semantic search + ES|QL filtering → Relevant indexed documents retrieved → Agent composes accurate response from saved knowledge base.                                              |
| **Human Handoff Flow**          | Enable handoff, add agent emails.                                         | Intent detection handled via Elastic Agent → Escalation triggered → Conversation context retrieved from indexed session data → Available agent assigned (round-robin) → Smooth real-time takeover.       |

The bot appears as a **floating action widget** on your website and can be fully customized to match your brand.

---

## How We Use Elastic in the System

Elastic acts as the core intelligence and retrieval layer across the entire bot lifecycle — from knowledge indexing to live search, analytics, and human handoff detection. It powers intelligent search, structured querying, and real-time observability across every interaction.

| Feature                            | Where Used                | How It Works                                                                                                                               | Benefit / Result                                                              |
| ---------------------------------- | ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------- |
| **Knowledge Indexing**             | Bot creation & training   | Extract PDFs/websites → Chunk content (~3000 chars) → Index documents in **Elastic** → Create dedicated Elastic Agent via API              | Structured, searchable knowledge base for each bot                            |
| **Semantic Search & ES|QL**        | Training & query time     | User query → Elastic semantic search + ES|QL filtering → Retrieve most relevant indexed documents                                          | Meaning-based retrieval, not just keyword matching                            |
| **Live Question Answering**        | Every user interaction    | Query routed to linked Elastic Agent → Agent searches indexed docs → Returns best contextual match                                         | Fast, accurate, context-aware responses                                       |
| **Multilingual Handling**          | Query processing layer    | Query analyzed → Indexed knowledge retrieved via Elastic search → Response generated consistently across languages                         | Unified search across multilingual content                                    |
| **Voice Conversations**            | Voice query & response    | Browser STT → Query sent to Elastic Agent → Relevant indexed data retrieved → Response returned → Browser TTS                              | Seamless spoken interaction powered by intelligent search                     |
| **Persona & Behavior Enforcement** | Agent configuration layer | Bot rules and persona linked to Elastic Agent → Agent retrieves only relevant indexed content while respecting defined constraints         | Controlled, brand-aligned responses                                           |
| **Conversation Flow Intelligence** | AI + rule hybrid flows    | Flow logic executes → When knowledge lookup needed, Elastic Agent performs indexed search using ES|QL                                      | Structured flows combined with intelligent retrieval                          |
| **Human Handoff Detection**        | Escalation system         | Elastic Agent detects escalation intent → Retrieves session context from indexed conversation data → Triggers round-robin agent assignment | Smart escalation with full conversation context                               |
| **Session Storage & Analytics**    | Monitoring & insights     | Conversations indexed in Elastic → ES|QL used for filtering, metrics, and reporting                                                        | Real-time observability, searchable session history, and actionable analytics |

![How Elastic Search is used](https://res.cloudinary.com/dlpozcdw7/image/upload/v1772214525/usage_of_elastic_naqtiu.png)

--- 

## Real-World Example: Healthcare Bot 🏥

### Use Case: Hospital Website Assistant

A hospital uses TasteAI Studio to deploy a healthcare assistant that:

- Answers FAQs about doctors, OPDs, and insurance
- Books appointments
- Explains lab reports in simple language
- Detects urgency in patient queries

### Smart Human Handoff

When the bot detects:
- Medical emergencies
- Emotional distress
- Repeated failed answers

It **automatically escalates** the conversation.

### Enhanced Escalation System

- Priority-based routing (Emergency > Billing > General)
- Auto-assignment to available agents
- Skill-based matching (doctor, nurse, admin)
- Real-time sync with Slack or dashboard
- Full conversation context passed to the human

💬 *No “please repeat your issue” moments.*

---

## How We Built It

- **Frontend**: React + modern UI primitives for fast, clean UX
- **Backend**: Node.js + scalable APIs
- **AI Layer**: Multi-model support with structured prompting
- **Conversation Engine**: Hybrid flow-based + agentic reasoning
- **Escalation Engine**: Rule-based + AI confidence scoring
- **Analytics**: Session-level summaries and metrics
- **Integrations**: Slack, website embed, future CRM support

Everything is designed to be:
- Modular
- Observable
- Production-safe

---

## Challenges We Ran Into

- Designing AI systems that **fail gracefully**
- Making human handoff feel invisible to users
- Balancing no-code simplicity with advanced control
- Preventing hallucinations in regulated industries
- Scaling real-time conversations reliably

---

## Accomplishments We’re Proud Of

- Seamless AI → Human transitions
- Real-time escalation with context preservation
- Visual conversation flows + AI autonomy
- Website integration in under 5 minutes
- Analytics that actually help teams improve bots

---

## What We Learned

- Bots shouldn’t replace humans—they should **empower them**
- Escalation is not a fallback, it’s a feature
- Production bots need observability, not just intelligence
- Trust is built when bots know their limits

---

## What’s Next for TasteAI Studio

Upcoming features:
- CRM & ticketing integrations with Hubspot/JIRA
- Voice + video calling handoff by integrating with Google Meet and Zoom/ Creating a Novel Video/Voice Call System using WebRTC
- Auto-learning and training from resolved sessions
- Role-based agent dashboards
- Industry-specific bot templates (Healthcare, Finance, SaaS)
- Advanced policy-driven escalation workflows

---

## Final Thought

TasteAI Studio isn’t just a chatbot builder.

It’s a **conversation infrastructure** for teams that care about users, reliability, and real outcomes.

> Build bots that know when to talk—and when to listen.

---
