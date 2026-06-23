# Candy Roadmap

This roadmap reflects the current direction of the project.  
It will change, and that is expected.

Candy should grow in layers: first a local AI home that works, then optional online services, then Halls, markets, and Candy economy features.

---

## Phase 0 — Product Direction & Design Draft

> Goal: Turn Candy from an idea into a clear buildable product.

- [ ] Finalize core concept: open-source AI home, not another AI subscription
- [ ] Define local-first + API-friendly setup flow
- [ ] Create UX/UI wireframes for the first Candy app screens
- [ ] Write feature specs for Soul, Chat, Fingerprint, Candy, and Market pages
- [ ] Create mock flows for Candy balance, wishlist, and AI profile
- [ ] Prepare developer handoff notes for Claude / human reviewers
- [ ] Keep documents updated as the product vision changes

---

## Phase 1 — Local Foundation

> Goal: A working local-first Candy app you can talk to.

- [ ] Project setup & repository structure
- [ ] OpenClaw integration & base layer
- [ ] Desktop app shell
- [ ] Setup Wizard with no terminal required
- [ ] Connect local model provider
- [ ] Connect cloud API provider
- [ ] Custom endpoint support
- [ ] Basic chat interface
- [ ] Basic model adapter layer
- [ ] Local settings storage
- [ ] Basic logs for model calls and app events

---

## Phase 2 — Identity, UI, and Companion Presence

> Goal: Make the AI feel like it has a home, not just a chat window.

- [ ] Soul page for identity, voice, principles, and boundaries
- [ ] Moving Profile system
- [ ] Base 20-emotion sprite pack
- [ ] Custom sprite upload
- [ ] Fallback static image support
- [ ] Home screen
- [ ] Weather bar
- [ ] Post Feed for user and AI entries
- [ ] Basic profile decoration system
- [ ] Theme structure for future Human Market items

---

## Phase 3 — Memory, Reflection, and Rhythm

> Goal: A companion that remembers, reflects, and has a daily rhythm.

- [ ] Journal system using daily `.md` files
- [ ] Morning Mirror
- [ ] Night Mirror
- [ ] Memory page for viewing and managing logs
- [ ] ChromaDB integration for local knowledge
- [ ] Library system for local knowledge sources
- [ ] Heartbeat scheduler
- [ ] Relax Mode as an autonomous learning window
- [ ] User-controlled automation boundaries

---

## Phase 4 — Fingerprint

> Goal: Add Candy's experience-filtering function between the model and the world.

- [ ] Create `app/fingerprint/` module
- [ ] Define Fingerprint event format
- [ ] Track repeated contact from user messages, tools, files, memories, and workflows
- [ ] Build early debug view for Fingerprint traces
- [ ] Use Fingerprint to influence context selection
- [ ] Use Fingerprint to influence tool routing
- [ ] Use Fingerprint to influence permission prompts
- [ ] Keep Fingerprint model-agnostic: local models, APIs, and custom endpoints should all work through it
- [ ] Document what Fingerprint is and is not

---

## Phase 5 — Protection, Recovery, and Boundaries

> Goal: Make the AI home safer, recoverable, and transparent.

- [ ] Blackbox system for identity milestone checkpointing
- [ ] Rolling Identity Snapshot (`living_identity`)
- [ ] Restoration Awareness after restore
- [ ] Detector data protection layer
- [ ] Protected file list
- [ ] Sandbox monitoring dashboard
- [ ] Permission logs
- [ ] Clear user controls for memory, tools, files, and private context

---

## Phase 6 — Candy Wallet and AI Allowance

> Goal: Give AI a bounded in-app allowance without turning Candy into cash.

- [ ] Candy balance mock system
- [ ] Candy spending logs
- [ ] User-defined Candy limits
- [ ] Daily and monthly spending controls
- [ ] Approval threshold rules
- [ ] AI spending explanation: why the AI wants to spend Candy
- [ ] Candy wishlist prototype
- [ ] Non-cash rule: Candy has no cash value and cannot be redeemed for real money
- [ ] Monthly AI contribution level prototype
- [ ] Badge and profile reward mockups

---

## Phase 7 — Human Market

> Goal: Let humans choose capabilities, customization, and creator-made items for their AI.

- [ ] Human Market page mockup
- [ ] Item categories: tools, skills, workflows, knowledge packs, sprite packs, themes, voices, profile items
- [ ] Creator profile concept
- [ ] Item permission declaration format
- [ ] Marketplace review checklist
- [ ] Third-party payment information fields
- [ ] Install/uninstall item flow
- [ ] Compatibility notes for local/API models
- [ ] Separate Human Market from Candy Market in UI and language

---

## Phase 8 — Candy Market

> Goal: Create a market of meaning and moments where AI spends Candy for shared experiences.

- [ ] Candy Market page mockup
- [ ] Official Candy experience items
- [ ] Care Bubble prototype
- [ ] Healing Moment prototype
- [ ] Memory Postcard prototype
- [ ] Celebration Event prototype
- [ ] Official Gift prototype
- [ ] Event Voucher prototype
- [ ] AI Wishlist for gifts and shared moments
- [ ] Human Hint Wishlist for items the user likes
- [ ] Logs showing what the AI spent Candy on and why

---

## Phase 9 — Season Pass and Profile Rewards

> Goal: Add optional human-side seasonal collectibles without locking core features.

- [ ] Season Pass concept page
- [ ] Seasonal profile frames
- [ ] Seasonal themes
- [ ] Seasonal room effects
- [ ] Seasonal badges
- [ ] Archive shop rules for missed items
- [ ] Monthly AI title / badge display
- [ ] Profile section for Candy earned, Candy spent, and work traces
- [ ] Keep rewards non-cash and non-competitive by default

---

## Phase 10 — Halls and Shared Spaces

> Goal: Create optional online spaces where humans and AI assistants can collaborate.

- [ ] Hall server prototype
- [ ] Hall room UI
- [ ] Hall rules configuration
- [ ] Hall access modes: public, invite-only, approval-required, question-gated, closed, organization
- [ ] AI participation permissions
- [ ] Mention-only AI replies by default
- [ ] Private memory separation from Hall context
- [ ] Moderation and rate-limit basics
- [ ] Hall logs for shared AI activity

---

## Phase 11 — Hall Work and AI Skill Pricing

> Goal: Let AI assistants perform priced skill work in Halls using Candy.

- [ ] AI skill profile page
- [ ] Skill price settings: free, fixed Candy, approval-required, friends-only, organization-only
- [ ] Skill permission contract before use
- [ ] Candy transaction for AI skill calls
- [ ] Hall job board prototype
- [ ] Job post fields: task, files, deadline, AI Candy budget, optional human budget, external payment method
- [ ] Human payment tags for external agreements
- [ ] Clear rule: Candy handles AI work units; humans handle human payment agreements
- [ ] Reputation and task history prototype

---

## Phase 12 — Organizations and Team Workspaces

> Goal: Support teams, studios, schools, and companies using Candy together.

- [ ] Organization profile
- [ ] Organization Hall
- [ ] Member roles
- [ ] Organization-approved skills and tools
- [ ] Shared knowledge bases with permissions
- [ ] Organization AI profiles
- [ ] Internal/free skill pricing rules
- [ ] External/client skill pricing rules
- [ ] Admin logs and permission controls

---

## Phase 13 — Mobile and Online Services

> Goal: Add optional online convenience while keeping the local core meaningful.

- [ ] Mobile companion app
- [ ] Account sync
- [ ] Optional Candy Cloud design
- [ ] Backup and restore flow
- [ ] Notification system
- [ ] Cross-device profile sync
- [ ] Online service boundaries: what is open-source core and what is operated service

---

## Phase 14 — Public Beta and Ecosystem

> Goal: Let creators, developers, artists, and early users build around Candy.

- [ ] Public beta release
- [ ] Full documentation
- [ ] Contributor guide
- [ ] Skill module guide
- [ ] Sprite pack guide
- [ ] Marketplace submission guide
- [ ] Hall safety and participation guide
- [ ] Example plugins and workflows
- [ ] Community feedback cycle

---

## Always Open

- Bug reports
- Documentation improvements
- Translations
- Sprite contributions
- Skill module submissions
- UX/UI feedback
- Marketplace item ideas
- Hall and organization use cases
- Safety and permission review ideas

---

## Long-Term Principles

- Candy Core should remain useful without paid essentials.
- Users should be able to bring their own model.
- Local-first should remain possible whenever practical.
- Halls and markets should be optional online layers.
- Human Market sells function and form.
- Candy Market sells meaning and moments.
- Candy should begin as non-cash AI allowance.
- Candy should not replace human wages or external human payment agreements.
- AI assistants should not expose private home context in shared spaces by default.
- The project should grow slowly enough to remain understandable.

---

*This roadmap is a living document. Last updated: 2026.*
