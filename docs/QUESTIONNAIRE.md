# Application Discovery Questionnaire

## Overview

This 10-question framework helps define clear requirements for any software project. Answer these questions to align stakeholders and guide development decisions.

---

## Core Questions

### Q1. What problem does your application solve, and who feels that pain the most?

**Why we ask:** Defines the core value proposition and primary users.

**Example answers:**

- "Dog-walkers struggle to track multiple clients; my app will auto-schedule routes for walkers with >10 dogs per day."
- "University students can't find last-minute study rooms; the app aggregates real-time room availability."

### Q2. On which devices and platforms should the first version run?

**Why we ask:** Narrows the tech stack and design constraints.

**Example answers:**

- "iOS and Android phones only—tablets and desktop later."
- "Any modern browser; must work on low-end Chromebooks."
- "Desktop VR headset (Meta Quest 3) plus a slim companion mobile app."

### Q3. Which scripting/programming language(s) do you prefer, and why?

**Why we ask:** Aligns with existing team skill, hosting options, and library ecosystems.

**Example answers:**

- **Python** – "Rapid prototyping, huge AI libraries, fine if server-side only."
- **JavaScript/TypeScript** – "Runs in browsers and Node.js, single language front-to-back."
- **Kotlin** – "Modern, null-safe; I expect tight Android integration."
- "No strong preference—recommend what fits my budget."

### Q4. List the must-have features for the MVP (Minimum Viable Product)?

**Why we ask:** Prevents scope creep; anchors the first release.

**Example answers:**

- "User login with Google, basic profile, create/read/update/delete notes, and share a note via link."
- "GPS route tracking, step counter, calorie estimate, and weekly summary email."
- "Upload 1-minute video, auto-generate captions, allow simple trim, then publish."

### Q5. Which third-party services or APIs should we integrate with (if any)?

**Why we ask:** Determines licensing cost, data flow, and potential vendor lock-in.

**Example answers:**

- Stripe for payments, Google Maps for geocoding, Twilio for SMS.
- "No external APIs; everything must run offline (military use-case)."
- OpenAI for text generation + Cloudinary for media storage.

### Q6. How should data be stored and synced?

**Why we ask:** Guides database choice, offline strategy, and security controls.

**Example answers:**

- "Cloud-only, PostgreSQL on `Supabase`."
- "Real-time collaboration—need Firebase `Firestore`-style live updates."

### Q7. What level of security, privacy, or compliance is required?

**Why we ask:** Impacts architecture, hosting region, and audit features.

**Example answers:**

- "Must be HIPAA-compliant; patient data encrypted in transit and at rest."
- "Consumer social app—standard OAuth, no special compliance."
- "European customers only—GDPR data-deletion workflow mandatory."

### Q8. How should the user interface feel (style, tone, accessibility)?

**Why we ask:** Sets design language and accessibility targets.

**Example answers:**

- "Minimalistic, monochrome, like Notion; AA accessibility at least."
- "Playful neon cyber-punk with motion effects; `WCAG` can be AA except AAA contrast not needed."
- "Enterprise dashboard: dense tables, light mode only, Excel import vibes."

### Q9. What are your performance or scalability expectations for the first year?

**Why we ask:** Determines hosting tier, caching, and cost planning.

**Example answers:**

- "Pilot with 500 beta users; uptime 99% is fine."
- "Expect viral spikes—handle 100k concurrent users for live trivia."
- "Internal tool for 50 employees—latency under 1s, nothing fancy."

### Q10. Budget, timeline, and post-launch maintenance — what's realistic?

**Why we ask:** Aligns scope with resources and clarifies ongoing responsibilities.

**Example answers:**

- "$15k MVP budget, 3-month build, then $500/month for updates."
- "Open-source passion project—volunteer devs, slow timeline."
- "VC-backed: up to $250k this year, need v1 in 10 weeks, full-time dev retainer after."

---

## Using the Responses

### Next Steps:

1. **Document Requirements** → Drop answers into a shared doc and distill into functional + non-functional requirements
2. **Design Architecture** → Sketch an architecture and tech stack diagram that satisfies Q2–Q7
3. **Create Roadmap** → Derive a phased roadmap from Q4, Q9, and Q10
4. **Validate** → Confirm with the client before writing any code

### Deliverables Checklist:

- [ ] Requirements document (functional & non-functional)
- [ ] Architecture diagram
- [ ] Tech stack decision matrix
- [ ] Development roadmap with milestones
- [ ] Budget breakdown and resource allocation
- [ ] Maintenance plan post-launch
- [ ] User interface mockups or style guide
- [ ] Testing strategy (unit, integration, user acceptance)
- [ ] Deployment plan (CI/CD, hosting)
