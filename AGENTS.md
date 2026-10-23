# AGENTS.md: Wrought Systems website

This file guides any AI agent (or human) that designs, builds, or maintains the
Wrought Systems website. Read it fully before making changes. When something here
conflicts with a request in a task, follow the task, then propose an update to this file.

---

## 1. The company

| | |
|---|---|
| **Legal name** | Wrought Systems (Pty) Ltd |
| **Registration no.** | 2026/833481/07 (CIPC, South Africa) |
| **Registered** | 20 October 2026 |
| **Brand name** | **Wrought** (in conversation), **Wrought Systems** (formal) |
| **Primary domain** | `wrought.systems` |
| **Secondary domain** | `wrought-systems.com` (redirects to the primary domain, if registered) |
| **GitHub org** | `wroughtsystems` |
| **Founder** | Pieter Engelbrecht, known as **chesedo** in the Rust community |

### What we do

A Rust consultancy. We build and rescue serious systems software for companies
that need it done right: backend services, infrastructure, tooling, performance
work, and architecture.

The founder has 5+ years of production Rust experience, including work for Shuttle
(a Rust-native cloud startup) and for Redis. That track record is the main
credibility signal. Use it, but don't inflate it.

### The model: senior-led teams

This is what sets Wrought apart. Explain it clearly on the site.

- Pieter leads and oversees every engagement as architect.
- Developers he has mentored work on projects **under his oversight**, pairing
  with him rather than being placed alone with clients.
- Clients get senior judgment with more capacity than one person can give.
- Developers get real Rust experience, which grows the local talent pool.

Never describe this as outsourcing, staff augmentation, or "resources".

### The mission

- Build excellent software for clients worldwide.
- Grow Rust developers in **South Africa and Africa**, and help the region thrive.
- Pieter sees himself as a **steward** of the company, with God as its owner. The
  business exists to have whatever impact God intends through it.

---

## 2. The name: "Wrought"

"Wrought" works on two levels. The site should honour both.

**For clients:** craftsmanship. *Wrought* iron is worked by hand. Carefully made
software. There's also a quiet nod to iron and Rust.

**The deeper meaning:** *"What hath God wrought!"* (**Numbers 23:23**, KJV). In
context, it's a declaration that God's promises come to pass. He does this by
working *through* people. The Hebrew verb is *pa'al* (to do, make, work).

The same phrase was the **first message Samuel Morse sent over his telegraph line
in 1844**, the start of electronic communication. Use this as a bridge between the
faith story and the tech story.

**How to show it:**

- Put the faith element in **one deliberate, sincere place**: an About or "Why
  Wrought?" section, and optionally a small footer line: *"What hath God wrought!"
  (Numbers 23:23)*.
- Don't hide it, and don't preach it. State it plainly and briefly, as the reason
  for the name.
- Don't put Bible verses on service or pricing pages.
- **Never use "Rust" as part of the company name or logo.** The Rust Foundation has
  trademark rules. Saying "Rust consultancy" in descriptive copy is fine.

---

## 3. Audience

Optimise for, in this order:

1. **Engineering leaders at international tech companies** (CTOs, VPs of
   Engineering, staff engineers) evaluating a Rust partner. They scan quickly,
   distrust marketing fluff, and want evidence.
2. **Founders and startups** needing Rust expertise they can't hire full time.
3. **Rust developers** (especially in Africa) interested in working with or
   learning from Wrought. This is a secondary audience; serve them with one
   page, not the whole site.

Most clients are **outside South Africa**. Write for an international reader. Show
prices, if any, in USD or EUR, and mention time-zone overlap with Europe (South
Africa is UTC+2).

---

## 4. Voice and tone

- **Calm, precise, confident.** We're craftspeople, not salespeople.
- Short sentences. Concrete claims. Technical where it helps.
- Show, don't assert. Prefer "Cut p99 latency from 800 ms to 40 ms" over "We
  deliver blazing-fast solutions."
- **Banned words:** blazing, rockstar, ninja, synergy, cutting-edge, world-class,
  revolutionary, "solutions" as a noun on its own.
- Use honest humility. Don't claim team size, clients, or results we don't have.
- **Spelling:** British/South African English (organisation, colour), unless Pieter
  says otherwise.

---

## 5. Site structure (starting point)

| Page | Purpose |
|---|---|
| **Home** | One-sentence positioning, the senior-led model, proof (past clients and work), a clear contact call to action |
| **Services** | What we do: build, rescue or review, architecture, performance, training or mentoring |
| **Work** | Case studies or past engagements, only with client permission |
| **About / Why Wrought** | Pieter's story, the name, the mission, the stewardship view |
| **Join** | For Rust developers who want to grow with Wrought |
| **Writing** | Technical articles (they can live on chesedo.me with links here, or move here; see §9) |
| **Contact** | Email and/or a booking link. Keep it simple, with no long forms |

Start small. A strong single-page site beats five thin pages.

---

## 6. Design direction

- **Feel:** a forge and a workshop. Solid, warm, crafted, quiet. Think wrought iron,
  not neon.
- **Palette:** dark iron/charcoal neutrals, warm off-white, and **one** accent: a
  warm forge orange or a muted rust tone. Use the accent sparingly.
- **Typography:** one confident serif or slab-serif for headings (craft), and a clean
  sans-serif for body. A monospace font only for code.
- **Layout:** generous whitespace, strong grid, few elements. No stock photos of
  people pointing at screens.
- **Logo:** to be designed. A simple wordmark "wrought" is a good default. It should
  work in one colour and at favicon size.
- **Dark mode:** support it. Many visitors are engineers.

---

## 7. Technical requirements

- **Stack:** prefer a static site. Pieter's existing site (chesedo.me) uses **Zola +
  Tailwind CSS**, so default to that for consistency unless there's a good reason
  not to.
- **Performance is part of the brand.** Target Lighthouse ≥ 95 in every category.
  Ship little to no JavaScript, use optimised images, and self-host fonts or keep
  them to a minimum.
- **Accessibility:** WCAG 2.2 AA. Use semantic HTML, keyboard navigation, sufficient
  contrast, and alt text.
- **Responsive:** mobile first, with no horizontal scroll.
- **SEO:** unique titles and meta descriptions, Open Graph tags, `sitemap.xml`,
  canonical URLs, and structured data (Organization schema).
- **Privacy:** no invasive tracking. If analytics are needed, use a privacy-friendly,
  cookieless option.
- **Hosting:** static hosting with HTTPS and CI/CD from the GitHub repo
  (`wroughtsystems` org).

---

## 8. Legal and compliance content

**Footer must show:** "Wrought Systems (Pty) Ltd · Reg. No. 2026/833481/07 ·
South Africa".

**Never publish:**

- Pieter's ID number
- The registered office / home street address. Use "Pretoria, South Africa" only.
- Personal phone numbers, unless Pieter explicitly asks
- Tax reference numbers, bank details, or CIPC customer codes
- Client names, logos, or results **without written permission**

If a contact form collects personal data, add a short privacy notice that complies
with South Africa's POPIA (what's collected, why, and how to request deletion).

---

## 9. Relationship with chesedo.me

- **chesedo.me** is Pieter's personal brand: blog, talks, community presence.
- **wrought.systems** is the company.
- Cross-link them: the About page links to chesedo.me, and chesedo.me says
  "Founder of Wrought Systems".
- Decide with Pieter where technical writing lives. Don't duplicate posts without
  canonical tags.

---

## 10. Maintenance checklist

**On every change:**

- [ ] Builds without errors or warnings
- [ ] Links work, internal and external
- [ ] Lighthouse and accessibility targets still met
- [ ] Looks correct in light and dark mode, and at phone width
- [ ] No banned words, unverifiable claims, or private details (§4, §8)

**Quarterly:**

- [ ] Update dependencies
- [ ] Review case studies and services for accuracy
- [ ] Check domain renewals: `wrought.systems` renews at roughly $41/year after
      the first year

**Ask Pieter before:**

- Adding a client name, testimonial, logo, or result
- Changing the name story or faith wording
- Adding prices, tracking, or third-party scripts
- Making structural changes to navigation or domains

---

## 11. Open decisions

Record answers here as they're made:

- [ ] Logo and final colour palette
- [ ] Where technical writing lives (§9)
- [ ] Contact method: email only, or also a booking link
- [ ] Whether to publish indicative pricing
- [ ] Whether the "Join" page goes live at launch
