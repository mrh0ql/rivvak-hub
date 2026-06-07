# Rivvak Services Documentation

> **Internal reference for scoping, pricing, and delivering each service category.**

---

## Service Catalog

### 1. Landing Pages

**What it is:** A single-page marketing site designed to convert visitors into leads or customers.

**Tech stack:** HTML/CSS/JS (vanilla), deployed on Vercel or Netlify.

**Typical scope:**
- Hero section with headline + CTA
- 3–5 feature/benefit sections
- Social proof (testimonials, logos, stats)
- Pricing section
- FAQ accordion
- Contact form or email CTA
- Full dark/light mode
- Mobile-first, fully responsive

**Deliverables:**
- Single `index.html` file (or multi-file if CMS needed)
- Deployed to live URL
- Source code pushed to client's repo (if requested)

**Pricing:**
| Scope | Price |
|---|---|
| Simple (3–4 sections) | $300–400 |
| Standard (5–7 sections) | $500–700 |
| Premium (7+ sections, animations, CMS) | $800–1,200 |

**Delivery time:** 1–3 business days

---

### 2. Web Applications

**What it is:** A functional, interactive web app — dashboard, tool, SaaS MVP, internal tool.

**Tech stack:** Next.js + TypeScript + Tailwind, Supabase or PostgreSQL, deployed on Vercel.

**Typical scope (MVP):**
- User authentication (email/password or OAuth)
- Core feature (1–3 main views)
- Database schema + API routes
- Basic admin view
- Deployed to production

**Deliverables:**
- Full codebase pushed to client's GitHub repo
- Live deployment URL
- Environment variable documentation
- README with setup instructions

**Pricing:**
| Scope | Price |
|---|---|
| Simple tool (no auth, 1–2 views) | $800–1,200 |
| MVP (auth + core features) | $1,500–2,500 |
| Full SaaS (auth + billing + core) | $3,000–6,000 |

**Delivery time:** 3–10 business days depending on complexity

---

### 3. AI Automations

**What it is:** A custom workflow powered by AI (typically OpenAI) — content generation, data processing, classification, summarization, or decision-making pipelines.

**Tech stack:** Python or Node.js, OpenAI API, deployed on Vercel/Railway/server.

**Typical scope:**
- Trigger (webhook, schedule, manual)
- AI processing step (prompt + model call)
- Output destination (email, database, Slack, Airtable, etc.)
- Error handling + logging
- Documentation

**Deliverables:**
- Complete source code
- Deployment + env var setup
- Prompt documentation
- Testing evidence

**Pricing:**
| Scope | Price |
|---|---|
| Single automation (1 trigger → 1 output) | $500–800 |
| Multi-step pipeline | $800–1,500 |
| Complex AI system (multiple models/steps) | $1,500–3,000 |

**Delivery time:** 2–5 business days

---

### 4. Telegram Bots

**What it is:** A custom Telegram bot — command-based, AI-powered, notification-only, or CRM-integrated.

**Tech stack:** Python (python-telegram-bot) or Node.js (grammy/telegraf), deployed on Railway or Vercel.

**Types:**
- **Command bot:** Responds to `/commands`, does specific actions
- **Notification bot:** Pushes alerts/updates to users or channels
- **AI conversational bot:** Natural language powered by OpenAI
- **CRM bot:** Captures leads, logs to Airtable/Notion/Sheet

**Deliverables:**
- Full source code
- Bot token setup guide
- Deployment instructions
- Command reference doc

**Pricing:**
| Scope | Price |
|---|---|
| Simple notification/command bot | $350–500 |
| AI conversational bot | $500–900 |
| Full CRM/lead-capture bot | $700–1,200 |

**Delivery time:** 2–4 business days

---

### 5. API Integrations

**What it is:** Connecting two or more external services via their APIs — syncing data, triggering actions, or automating workflows between platforms.

**Common integrations:**
- Stripe → Notion (payment → task/record)
- Airtable → Slack (record change → notification)
- Shopify → custom database
- Webhook receiver → multi-destination fan-out
- Google Sheets → any API

**Deliverables:**
- Integration code (deployed)
- Webhook setup documentation
- Error monitoring
- Test evidence with real data

**Pricing:**
| Scope | Price |
|---|---|
| Simple 2-way sync | $400–600 |
| Multi-service orchestration | $600–1,000 |
| Real-time event pipeline | $800–1,500 |

**Delivery time:** 2–4 business days

---

### 6. Monthly Retainer

**What it is:** Ongoing development, maintenance, and improvement work billed monthly.

**What's included:**
- Agreed hours of development work per month
- Priority response time
- Monthly strategy call (optional)
- Documentation of all work done
- Code reviews and architecture advice

**Not included:**
- Infrastructure/hosting costs (billed to client)
- Third-party API costs
- Work clearly outside agreed scope without pre-approval

**Tiers:**
| Tier | Hours | Price |
|---|---|---|
| Starter | ~5 hrs | $400/mo |
| Standard | ~10 hrs | $700/mo |
| Growth | ~18 hrs | $1,200/mo |

**See:** `playbooks/retainer.md` for full retainer management guide.

---

## Scoping Rules

1. **Never start without a confirmed spec** — if requirements are vague, write them out and get client approval
2. **Document edge cases upfront** — "What should happen if X?" for every non-obvious scenario
3. **Time estimates are binding** — if you think it's 5 hours, quote 8 to absorb unknowns
4. **Complexity multipliers:**
   - Each additional API integration: +$100–200
   - Mobile-responsive requirements (if not standard): +$100
   - Rush delivery (<48h): +50%
   - Post-delivery changes outside scope: billed at $80/hr

---

## Quality Standards

Every delivery must meet these standards before handoff:

- [ ] Tested against real data (not just test data)
- [ ] Error states handled gracefully (no blank screens, no raw errors)
- [ ] Deployed to live environment, not just local
- [ ] README or documentation written
- [ ] Code pushed to version control
- [ ] All credentials stored in environment variables (never hardcoded)
- [ ] Mobile responsive (for web deliverables)
- [ ] Checked in both light and dark mode (for web deliverables)
