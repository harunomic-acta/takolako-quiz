# Conversion Analysis — takolako.online
**Date:** April 2026  
**Scope:** Landing page (quiz funnel at takolako.online) + main marketing site  
**Goal:** Identify copy, section, and architecture improvements that increase quiz starts, email captures, and trial class bookings

---

## What we're working with

The project is a **two-layer funnel**:

1. **Main marketing site** (takolako.online) — full-featured school website: navigation, offerings, testimonials, video, teachers, pricing, FAQ, footer
2. **This project** (index.html) — a standalone quiz funnel that is either embedded or linked from the main site, collecting leads through a 10-question assessment → email gate → personalized results → CTA to book a trial class

The analysis covers both layers since they're part of the same conversion chain.

---

## 1. Architecture issues

### 1.1 The funnel entry is split between two pages with unclear relationship

**Problem:** The main site at takolako.online has a quiz/age-selection widget in its hero. This project (index.html) is *also* a complete quiz funnel. It's unclear to the visitor whether they're on the same property, and unclear to us which is the "canonical" quiz start. If both exist simultaneously, users who start on the main site and then land on index.html will have to re-answer the age question.

**Fix:** Either (a) make index.html the one true entry point and link to it clearly from the main site CTA, or (b) embed the quiz directly into the main site's page without a page transition. The current hybrid creates cognitive friction and breaks the sense of continuity.

---

### 1.2 The main site has too many exit points before conversion

**Problem:** The top navigation includes Početna, Naša Priča, Blog, language selector, and a Contact link. Each one is an escape hatch. The blog and "Our Story" links pull curious visitors away at exactly the moment they should be evaluating a trial class.

**Fix:** For a high-intent landing page (especially one primarily receiving paid traffic), use a minimal header: logo only, or logo + single CTA. Move blog/about to the footer. This is the standard approach for high-converting school landing pages.

---

### 1.3 The quiz result page has three CTAs of roughly equal weight

**Problem:** After seeing their child's result, visitors are presented with three buttons:
- "Razgovarajmo o Vašem djetetu" (info call) — coral/primary
- "Kako izgleda testni čas?" (learn more page) — blue
- "Zakaži testni čas odmah" (direct booking) — green

Three equally prominent CTAs diffuse focus. The "learn more" button sends a warm lead who just completed a quiz *back* into an information-gathering mode when they should be booking.

**Fix:** Make one CTA primary and unmistakable: **"Zakaži testni čas odmah"** (direct booking). This is the highest-value action. Demote "Razgovarajmo" to secondary (ghost button style). Remove or deeply bury "Kako izgleda testni čas?" from this screen entirely — if they need it, they haven't been convinced and the problem is upstream in the results copy, not solvable by offering them more reading.

---

### 1.4 The email gate is friction at exactly the wrong moment

**Problem:** The quiz collects email *before* showing results, with the framing "Unesite email i odmah ćete vidjeti personalizovanu procjenu i preporuke." This is a classic lead-gen gate and it works — but the framing is transactional ("give us your email to see your result") rather than value-led.

**Fix (copy only, no architecture change needed):** Reframe the email capture as delivery, not as a toll gate. Example: *"Gdje da pošaljemo procjenu?"* / "Where should we send the assessment?" + small body: "Pošaljemo vam i PDF s prijedlogom programa za Vaše dijete." This shifts from "pay to see" to "we'll deliver something useful to you." The email field label should say "Vaša email adresa" not just a placeholder.

---

### 1.5 The quiz questionnaire collects the wrong things in the wrong order

**Problem:** The 10 questions include: child's age, country of residence, daily language use, response to Bosnian, understanding, speaking ability, how long Bosnian has been part of daily life, etc. These are good diagnostic questions. But question 2 is "Gdje živite?" (Where do you live?) — country selection. This question:
- Feels like CRM segmentation, not assessment
- Breaks the "this quiz is about your child" frame
- Has no impact on the level result

**Fix:** Move country question to the email capture step ("Zemlja stanovanja"), where it genuinely belongs as contact enrichment. Keep all 9 remaining quiz questions focused purely on the child's language level. This shortens the quiz to 9 questions and removes a jarring context switch.

---

## 2. Copy issues

### 2.1 The quiz hero headline is good but the subhead underdelivers

**Current headline:** *"Koliko Vaše dijete zaista zna bosanski?"*  
**Current subhead:** *"Odgovorite na 10 brzih pitanja i saznajte na kojem je nivou Vaše dijete — i šta je sljedeći korak."*

The headline is strong — "zaista" (actually/truly) creates a productive tension, implying the parent might be overestimating. The subhead, however, is purely procedural. It describes the mechanics (10 questions, get a level) but doesn't connect to why this matters emotionally.

**Improved subhead option:**  
*"Tačna procjena pomaga nam da predložimo pravi program — ne preopširan, ne prelak."*  
(Accurate assessment helps us suggest the right program — not too broad, not too easy.)

Or, for stronger emotional resonance:  
*"Mnogi roditelji misle da im dijete 'dovoljno' zna bosanski. Saznajte gdje zaista stoji i šta je konkretno sljedeći korak."*

---

### 2.2 The social proof stats lack specificity and credibility

**Current stats:** 500+ djece, 20+ zemalja, 100% preporuka roditelja

**Problems:**
- "500+ djece" with no time frame — is this since 2020? Since 2023? The number needs a frame to feel real.
- "100% preporuka roditelja" — this strains credibility. 100% of *what*? How many parents? When surveyed? This reads as a made-up metric to skeptical visitors.
- "20+ zemalja" is genuinely impressive but isn't visually featured — listing even 5-6 country flags would make this tangible.

**Fix:**
- Change "100% preporuka" to something auditable: "4.9/5 ocjena roditelja (123 ocjene)" or remove it and replace with a concrete outcome stat: "Prosječno 2 nivoa napretka za 6 mjeseci"
- Add a timeframe: "500+ djece od 2020. godine"
- Add 4-6 flag emojis next to the country count

---

### 2.3 The main site hero is generic

**Current main site headline:** *"Nauči bosanski jezik uz Tako Lako"*  
**Current subhead:** *"Sačuvajte bosanski jezik u Vašoj porodici"*

The subhead is the stronger line — it speaks to identity and family, not just learning. The headline is a brand statement, not a value proposition.

**Fix:** Swap them. The emotional line leads; the school name follows:

> **"Sačuvajte bosanski jezik u Vašoj porodici"**  
> Online časovi bosanskog za djecu u dijaspori — od početnog do naprednog nivoa.

---

### 2.4 The "Why parents choose Tako Lako" section describes features, not outcomes

**Current feature titles:**
- Strukturirani sistem nivoa
- Aktivna govorna praksa i samopouzdanje
- Program razvijen za djecu u dijaspori
- Vidljiv napredak i predvidiv plan

These are features/process descriptions. They answer "what is it" not "what will change."

**Outcome-reframed versions:**
- "Vaše dijete tačno zna šta je sljedeći korak" → *"Dijete koje zna gdje stoji i kuda ide"*
- "Aktivna govorna praksa i samopouzdanje" → *"Iz stidljivog šutnje do sigurnog razgovora"*
- "Program razvijen za djecu u dijaspori" → *"Razumijemo djecu koja žive između dva jezika"* (this one is already good)
- "Vidljiv napredak i predvidiv plan" → *"Nikad više 'ne znam je li napredovalo'"*

---

### 2.5 Testimonials have low specificity

**Problem:** All three testimonials are warm and genuine but describe general satisfaction: "accepted online lessons", "now motivated to speak Bosnian", "increasingly interested in Bosnian culture." None include a specific, measurable before/after.

**Fix:** Wherever possible, coach or request that testimonials include:
1. A specific challenge they had before (e.g., "Moja kćerka je odbijala da priča bosanski kod kuće")
2. A specific result (e.g., "Nakon 3 mjeseca, sama inicira razgovor na bosanskom")
3. The format they used (individual, group, family)

If you can't get new testimonials, add a result sentence to existing ones: *"Nidžara F. — sada pohađa grupne časove, 2. nivo."*

---

### 2.6 Pricing is introduced without anchoring

**Problem:** The pricing section (22€/8€/11€) appears before the social proof and value sections have done their work. A parent seeing "22€ po času" before understanding the curriculum depth, teacher credentials, or typical progress trajectory has no frame of reference.

**Fix:** Move pricing *after* the "Why parents choose" and testimonial sections. Before showing price, show the guarantee: *"Ako niste zadovoljni u prve tri sedmice, vraćamo novac."* This reduces the perceived risk of committing to a paid plan.

---

## 3. Section-level improvements

### 3.1 Missing: a "What happens in a class?" section

Parents evaluating an online school for their child have a core anxiety: *will my child actually engage with this?* The teacher video helps, but a step-by-step breakdown of a 45-minute class (e.g., 10 min warm-up → 20 min active language practice → 15 min structured exercise) would directly address this. Even a 3-step visual would work.

---

### 3.2 Missing: specific teacher credential callouts

The "Meet our teachers" section shows photos and videos for Ivona, Samira, and Staša — but doesn't display certifications, years of experience, or specialization (e.g., "specijalizovana za djecu 7-10 godina" or "10 godina iskustva s djecom u dijaspori"). Parents in Germany and Denmark are accustomed to seeing credentials. Add a 1-2 line credential tag under each teacher name.

---

### 3.3 The "How to get started" 3-step section is too far down

**Problem:** The 3-step process (fill questionnaire → book trial class → choose format) appears as section 3 on the main site. This is valuable framing that removes uncertainty about what happens next — but only ~40% of visitors will scroll this far on mobile.

**Fix:** Move the 3-step summary *directly under the hero CTA* (before the quiz starts), condensed to a single-line visual: 

> `① Procjena (2 min) → ② Besplatan testni čas → ③ Pravi program za Vaše dijete`

This functions as a "journey preview" that makes clicking the CTA feel safe, not open-ended.

---

### 3.4 The risk-free guarantee section appears too late

**Problem:** The "Isprobajte bez rizika" section (free trial, sibling discount, 3-week guarantee) is section 9 of the main site. It's one of the strongest conversion arguments on the page — zero-risk trial, money-back guarantee — and it's buried.

**Fix:** Surface the guarantee visually in the hero area. A small trust badge row below the CTA button:

> 🎁 Besplatan probni čas &nbsp;|&nbsp; 💚 3-sedmična garancija povrata &nbsp;|&nbsp; 👨‍👩‍👧 Popust za braću i sestre

---

### 3.5 FAQ is too sparse

**Current FAQ:** 3 questions, all very general ("Why choose TakoLako?", "What are classes like?", "Will my child understand?")

**Missing high-anxiety questions diaspora parents actually have:**
- "U koje termine su dostupni časovi? Kako funkcioniše s vremenskim razlikama?" (timezone scheduling)
- "Može li dijete koje uopšte ne govori bosanski krenuti s grupnim časom?"
- "Koliko dugo traje jedan nivo? Kako mjerimo napredak?"
- "Šta ako nastavnica nije dobra za naše dijete?"
- "Jesu li nastavnice certificirane? Po čijem programu rade?"
- "Mogu li pratiti časove kao roditelj?"

Add at least 5-6 more questions. The FAQ is often the last thing a nearly-convinced parent reads before booking. Every unanswered question at that stage is a lost conversion.

---

## 4. Priority ranking

| Priority | Issue | Effort | Impact |
|---|---|---|---|
| 1 | Three-CTA result screen → one primary CTA | Low | High |
| 2 | Surface guarantee under hero CTA | Low | High |
| 3 | Move country question to email capture step | Low | Medium |
| 4 | Reframe email gate copy | Low | Medium |
| 5 | Fix "100% preporuka" stat | Low | Medium |
| 6 | Expand FAQ to 8-10 questions | Medium | High |
| 7 | Add 3-step journey preview under hero | Medium | High |
| 8 | Move pricing after testimonials/guarantee | Medium | Medium |
| 9 | Add credential tags to teacher cards | Medium | Medium |
| 10 | Rewrite testimonials with before/after specificity | High | High |
| 11 | Add "What happens in a class?" section | High | Medium |
| 12 | Consolidate quiz entry point (one canonical funnel) | High | Medium |

---

## 5. Quick wins (implement first)

These require only copy edits, no structural changes:

1. **Result page CTA:** Make "Zakaži testni čas odmah" the single dominant button. Remove blue button from this view.
2. **Email gate headline:** Change to *"Gdje da pošaljemo procjenu Vašeg djeteta?"*
3. **Social proof:** Replace "100% preporuka" with "4.9/5 ★ — 120+ roditelja" (or whatever your actual number is). Add flags to country stat.
4. **Hero subhead:** Add one sentence about what the result tells them beyond just a "level" — e.g., "i konkretne preporuke za sljedeći korak".
5. **Trust row under quiz CTA:** Add 2-min / Besplatno / Bez obaveze as small inline badges (already done!) — good, keep this.
