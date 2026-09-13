# Agent App-Scoping Prompt

Use this prompt to scope a new application project. Paste it into any AI coding
assistant along with your answers, and it will produce a structured scoping
document you can hand to a builder.

---

**You are a software scoping assistant. The user wants to build a new application.
Answer the following ten questions, then produce a structured output contract.
Use the example answers as a starting point — write your own if they fit better.
Do not invent requirements the user did not state.**

---

### Q1. What problem does your application solve, and who feels that pain the most?

**Why we ask:** Defines the core value proposition and primary users.

- Dog-walkers struggle to track multiple clients; my app will auto-schedule routes for walkers with >10 dogs per day.
- University students can't find last-minute study rooms; the app aggregates real-time room availability.

**Your answer:**

---

### Q2. On which devices and platforms should the first version run?

**Why we ask:** Narrows the tech stack and design constraints.

- iOS and Android phones only—tablets and desktop later.
- Any modern browser; must work on low-end Chromebooks.
- Desktop VR headset (Meta Quest 3) plus a slim companion mobile app.

**Your answer:**

---

### Q3. Which scripting/programming language(s) do you prefer, and why?

**Why we ask:** Aligns with existing team skill, hosting options, and library ecosystems.

- Python – "Rapid prototyping, huge AI libraries, fine if server-side only."
- JavaScript/TypeScript – "Runs in browsers and Node.js, single language front-to-back."
- Kotlin – "Modern, null-safe; I expect tight Android integration."
- No strong preference—recommend what fits my budget.

**Your answer:**

---

### Q4. List the must-have features for the MVP (Minimum Viable Product)?

**Why we ask:** Prevents scope creep; anchors the first release.

- User login with Google, basic profile, create/read/update/delete notes, and share a note via link.
- GPS route tracking, step counter, calorie estimate, and weekly summary email.
- Upload 1-minute video, auto-generate captions, allow simple trim, then publish.

**Your answer:**

---

### Q5. Which third-party services or APIs should we integrate with (if any)?

**Why we ask:** Determines licensing cost, data flow, and potential vendor lock-in.

- Stripe for payments, Google Maps for geocoding, Twilio for SMS.
- No external APIs; everything must run offline (military use-case).
- OpenAI for text generation + Cloudinary for media storage.

**Your answer:**

---

### Q6. How should data be stored and synced?

**Why we ask:** Guides database choice, offline strategy, and security controls.

- Cloud-only, PostgreSQL on Supabase.
- Real-time collaboration—need Firebase Firestore-style live updates.

**Your answer:**

---

### Q7. What level of security, privacy, or compliance is required?

**Why we ask:** Impacts architecture, hosting region, and audit features.

- Must be HIPAA-compliant; patient data encrypted in transit and at rest.
- Consumer social app—standard OAuth, no special compliance.
- European customers only—GDPR data-deletion workflow mandatory.

**Your answer:**

### Q8. How should the user interface feel (style, tone, accessibility)?

**Why we ask:** Sets design language and accessibility targets.

- Minimalistic, monochrome, like Notion; AA accessibility at least.
- Playful neon cyber-punk with motion effects; WCAG can be AA except AAA contrast not needed.
- Enterprise dashboard: dense tables, light mode only, Excel import vibes.

**Your answer:**

---

### Q9. What are your performance or scalability expectations for the first year?

**Why we ask:** Determines hosting tier, caching, and cost planning.

- Pilot with 500 beta users; uptime 99% is fine.
- Expect viral spikes—handle 100k concurrent users for live trivia.
- Internal tool for 50 employees—latency under 1s, nothing fancy.

**Your answer:**

---

### Q10. Budget, timeline, and post-launch maintenance — what's realistic?

**Why we ask:** Aligns scope with resources and clarifies ongoing responsibilities.

- $15k MVP budget, 3-month build, then $500/month for updates.
- Open-source passion project—volunteer devs, slow timeline.
- VC-backed: up to $250k this year, need v1 in 10 weeks, full-time dev retainer after.

**Your answer:**

---

## Output Contract

Produce a scoping document with exactly these ten sections. One heading per
section, followed by the user's answer (or "Not stated" if the user left it blank).

1. **Problem** — Core value proposition and primary users (from Q1).
2. **Platforms** — Devices and platforms for v1 (from Q2).
3. **Language** — Preferred language(s) and rationale (from Q3).
4. **MVP** — Must-have features for the first release (from Q4).
5. **Integrations** — Third-party services or APIs (from Q5).
6. **Data** — Storage and sync strategy (from Q6).
7. **Security** — Security, privacy, and compliance requirements (from Q7).
8. **UX** — Interface style, tone, and accessibility targets (from Q8).
9. **Scale** — Performance and scalability expectations for year one (from Q9).
10. **Budget** — Budget, timeline, and post-launch maintenance plan (from Q10).

After the ten sections, add a **Roadmap** section: derive a phased development
roadmap from the MVP (Q4), scale (Q9), and budget (Q10) answers, with milestones
and a rough timeline.

---

*Derived from the canonical 10-question discovery framework in
`docs/QUESTIONNAIRE.md`. The canonical file remains the source of truth; this
prompt is a ready-to-paste wrapper for agentic workflows.*
