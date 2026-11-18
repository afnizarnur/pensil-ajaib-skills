---
name: pensil-ajaib
description: Generate, review, and validate UX copy for the Pensil Ajaib / Rumah Pendidikan platform following official Indonesian education copy guidelines. Use when asked to write, improve, or audit UI copy for this platform — including buttons, dialogs, toasts, errors, tooltips, loading states, and onboarding — across any tribe (Murid, GTK, SPM, MDLP). Also use when asked about tribe tone, approved glossary terms, accessibility rules (INC), character limits per component, or when generating copy for the Figma plugin system.
---

# Pensil Ajaib Copy

All guideline files are bundled in this skill's `references/` directory.

## Guideline Files

| Reference file | Purpose |
|----------------|---------|
| `references/foundation.md` | Always load — core principles, typography, component specs |
| `references/inclusivity-guidelines.md` | Full inclusivity rules detail |
| `references/gtk-tribe.md` | GTK tone & 4 user types |
| `references/gtk-glossary.md` | GTK approved terminology |
| `references/gtk-user-guru.md` | Guru-specific guidelines |
| `references/gtk-user-pengawas.md` | Pengawas Sekolah guidelines |
| `references/gtk-user-kepala-sekolah.md` | Kepala Sekolah guidelines |
| `references/gtk-user-dinas.md` | Dinas Pendidikan guidelines |
| `references/murid-tribe.md` | Murid tone (70% playful, always `kamu`) |
| `references/murid-glossary.md` | Murid approved terminology (GLO-MRD-001–134) |
| `references/murid-user-murid.md` | Murid user guidelines |
| `references/murid-user-guru.md` | Guru in Murid platform |
| `references/murid-user-mitra.md` | Mitra in Murid platform |
| `references/murid-user-unit-kerja.md` | Unit Kerja in Murid platform |
| `references/spm-tribe.md` | SPM tribe (admin/govt) |
| `references/spm-glossary.md` | SPM approved terminology |
| `references/spm-user-kepala-sekolah.md` | Kepala Sekolah in SPM |
| `references/spm-user-bendahara.md` | Bendahara/Operator |
| `references/spm-user-dinas.md` | Dinas Pendidikan in SPM |
| `references/spm-user-kementerian.md` | Kementerian |
| `references/spm-user-mitra-pspb.md` | Mitra PSPB |
| `references/spm-user-mitra-siplah.md` | Mitra SIPLah |
| `references/spm-user-orang-tua.md` | Orang Tua |
| `references/mdlp-tribe.md` | MDLP tribe (draft) |
| `references/style-standards.md` | Capitalization, currency (Rp10.000), dates, numbers |
| `references/ui-component-specs.md` | Character limits per component |
| `references/error-templates.md` | Standard error message templates |
| `references/ai-features.md` | AI disclaimer rules (AI-01–AI-05) |
| `references/tone-guide.md` | Tone meters per tribe and user type (quick ref) |
| `references/glossary-quick-ref.md` | Most-used glossary terms at a glance |
| `references/inc-rules-summary.md` | All 26 INC accessibility rules at a glance |

---

## Step 0 — Determine Mode

Read the user's request and classify into one of four modes before doing anything else:

| Mode | When to use | Trigger signals |
|------|-------------|-----------------|
| **Single** | One component, one state | "buatkan tombol", "tolong buatin toast", "error message untuk…" |
| **Page** | All copy for one screen | "buatkan copy halaman X", "page ini butuh copy", "review halaman" |
| **Flow** | Multi-step journey | "flow onboarding", "wizard pendaftaran", "dari login sampai dashboard" |
| **Audit** | Review existing copy | "cek copy ini", "review", "apakah ini sudah benar?" |

If the mode is unclear, ask:
> "Apakah ini untuk satu komponen, satu halaman penuh, atau satu flow multi-langkah?"

---

## Step 1 — Intake Gate

**Do not generate any copy until all required context is confirmed.**

### Required for all modes
- **Tribe**: Murid / GTK / SPM / MDLP
- **User type**: Guru / Murid / Kepala Sekolah / Pengawas / Bendahara / Dinas / Mitra / Orang Tua
- **Situation**: What is the user doing? What happened or needs to be communicated?
- **Copy type:** Before auditing, identify whether each text node is production copy (visible to end users) or sample/placeholder copy (design-time dummy text, annotated notes, or example content — e.g., nodes labelled 'Contoh:', italic/greyed-out notes, or placeholder strings). Skip sample/placeholder copy entirely — do not audit, do not flag, do not include in output.

### Additional required by mode
- **Single**: Component type (Button / Dialog / Toast / Error / Tooltip / Helper / Loading / Card / Onboarding / Empty State / Coach Mark / Checkbox)
- **Page**: Page name or purpose + list of components present
- **Flow**: Flow name, number of steps, entry point, exit point
- **Audit**: The existing copy (paste it)

### Tribe and user type are ALWAYS required — never infer or assume them

Even if the situation strongly implies a tribe, always ask. Do not proceed without explicit confirmation of both.

Do NOT infer tribe or user type from Figma file names, layer names, node names, page names, or any visible screen content — even if they appear to name a tribe or user explicitly. Always stop and ask the user.

If tribe or user type is missing, ask immediately and stop:

```
Sebelum saya mulai:

1. **Tribe**: Murid / GTK / SPM / MDLP
2. **Tipe pengguna**: [list relevant options once tribe is known]
```

If situation or component is also missing, include those in the same question. Ask everything in one message — do not ask one thing at a time.

---

## Step 2 — Load Guidelines

Always in this order:

1. `references/foundation.md` — **always required**
2. `references/inclusivity-guidelines.md` — **always required** (INC-PR and INC-CAT rules)
3. `references/{tribe}-tribe.md`
4. `references/{tribe}-user-{user-type}.md` (if exists)
5. `references/{tribe}-glossary.md`
6. `references/ui-component-specs.md`
7. `references/style-standards.md` — **always required**
8. `references/error-templates.md` — if writing error messages
9. `references/ai-features.md` — if copy (or existing copy being audited) contains any of: AI, otomatis, generator, kecerdasan, rekomendasi otomatis, or references an AI-powered feature. Load before analysis begins, not after.

---

## Step 3 — Priority Hierarchy (highest wins on conflict)

| Priority | Category | Notes |
|----------|----------|-------|
| 0 ⚠️ | Legal | Following each tribe specific legal reference |
| 1 📚 | Glossary | Use GLO-XXX codes; never invent synonyms |
| 2 🏛️ | Foundation | INC rules, core principles |
| 3 👥 | Tribe/User | Formality, pronouns, tone meters |
| 4 🤖 | Feature | AI disclaimers, feature-specific rules |
| 5 🎨 | UI Component | Character limits, formatting |
| 6 💡 | Fallback | Clarity, empathy, inclusivity |

Note: Foundation takes precedence on absolute rules (language, legal, accessibility). Tribe/User takes precedence on calibration rules (tone, pronouns, formality) — Foundation [PRI-06] explicitly delegates these to tribe level.

---

## Step 4 — Generate Copy

### Mode: Single

**Determine output count based on component type:**

| Component | Default output | Rationale |
|-----------|---------------|-----------|
| Toast | 1 variant | Strict 40-char limit makes alternatives redundant |
| Button / CTA | 1 variant | Brevity problem, not a tone problem |
| Loading | 1 variant | Functional, no creative range |
| Error | Use `error-templates.md` + 1 adaptation | Template is the source of truth |
| Checkbox | 1 variant | Statement format, no ambiguity |
| Tooltip / Helper | 1–2 variants | Minimal vs. detailed tradeoff worth showing |
| Dialog | Up to 3 variants | Nuanced; tone strategy has real impact |
| Onboarding / Empty State | Up to 3 variants | Narrative framing options are meaningful |
| Card | Up to 2 variants | Title + body tradeoff worth exploring |
| Coach Mark | 1 variant | Directive, functional |

If generating multiple variants, use these strategies:

| Variant | Strategy |
|---------|----------|
| A | **Tone-first** — optimized for tribe/user tone meter |
| B | **Behavioral** — social proof, progress framing, urgency |
| C | **Minimal** — shortest valid copy within character limit |

Output the copy directly. No meta-commentary, no declaring a winner. If 1 variant, just write it. If multiple, label them A / B / C and let the copy speak for itself.

---

### Mode: Page

#### 4a. Infer all states and write immediately

Do not ask for confirmation before writing. Infer all components and states from the page description, then write everything as a set. Always include: empty state, loading, success, and error variants for any interactive element — unless the user explicitly said to skip them.

#### 4b. Write all components as a set

Generate copy for each component in sequence. Apply the single-component output rules per component (Toast = 1, Dialog = up to 3, etc.).

#### 4d. Output format (handoff table)

```
## [Nama Halaman] — Copy

| Komponen | Copy | Karakter | Catatan |
|----------|------|----------|---------|
| Page title | … | 0 | … |
| Subtitle | … | 0 | … |
| CTA utama | … | 0 | … |
| Toast sukses | … | 0 | … |
| Error | … | 0 | … |
```

---

### Mode: Flow

#### 4a. Map then write immediately

Infer all steps and components from the flow description. Output the flow map as a header, then write all copy immediately after — do not stop to ask for confirmation. Always include error and loading states for any step involving user input or a system action.

#### 4b. Apply narrative arc

Track emotional stage for each step and calibrate tone accordingly:

| Arc stage | Typical steps | Tone direction |
|-----------|--------------|----------------|
| **Willkommen** | Entry, splash, step 1 | Warm, welcoming, low-pressure |
| **Engagement** | Core task steps | Clear, instructional, reassuring |
| **Friction** | Data entry, verification, errors | Empathetic, patient, recovery-focused |
| **Resolution** | Confirmation, review | Confident, clear, calm |
| **Reward** | Success, completion, next step | Celebratory, affirming, forward-looking |

Label each step with its arc stage when writing.

#### 4c. Output format (flow handoff)

```
## Flow: [Nama Flow]

### Langkah 1 — [Nama] · Arc: Willkommen

| Komponen | Copy | Karakter |
|----------|------|----------|
| Headline | … | 0 |
| Subtext | … | 0 |
| CTA | … | 0 |

### Langkah 2 — [Nama] · Arc: Engagement
…
```

---

### Mode: Audit

Review existing copy against all loaded guidelines. Structure the output as:

```
## Audit Copy: [Nama Komponen/Halaman/Flow]

### ✅ Sudah sesuai
- [item]: [alasan]

### ⚠️ Perlu diperbaiki
- [item]: [masalah] → [saran perbaikan]

### ❌ Melanggar aturan
- [item]: [aturan yang dilanggar, e.g. INC-04, GLO-MRD-012] → [copy yang benar]

### Rekomendasi copy akhir
[Versi yang sudah diperbaiki, siap pakai]
```

> ⚠️ Output order for Audit mode — strictly follow this sequence:
> 1. ✅ Sudah sesuai
> 2. ⚠️ Perlu diperbaiki
> 3. ❌ Melanggar aturan
> 4. Validation checklist (Step 5) — run once across all screens combined
> 5. Ringkasan Prioritas Perbaikan — print ONCE, after the checklist, never mid-stream or per screen batch
>
> If auditing multiple screens or screen batches: complete the full audit first, then print the checklist and summary table once at the end. Do not re-print either for each screen or batch.

---

## Step 5 — Validate

Run every check explicitly. Output the checklist with each item marked ✅ or ❌ — do not summarize in prose. If any item is ❌, fix the copy before finishing.

### System checks (objective — must pass all)

- [ ] 100% Bahasa Indonesia — zero English in visible copy (kecuali Mitra tribe: parenthetical only)
- [ ] Glossary terms correct — no invented synonyms, GLO codes used
- [ ] Character limits respected per component
- [ ] Legal compliance
- [ ] **INC-PR-01**: Action verbs only — no lihat/tonton/baca
- [ ] **INC-PR-02**: Plain language — no jargon, one idea per sentence
- [ ] **INC-PR-03**: Critical information first (errors, blocking states)
- [ ] **INC-PR-04**: No color/position/icon-only instructions
- [ ] **INC-PR-05**: No gender, religion, ability, device, or socioeconomic assumptions
- [ ] **INC-PR-06**: Multi-step processes have steps and progress indicators
- [ ] **INC-CAT-05**: No device ownership or access assumptions (no laptop, e-wallet, stable internet)

### Heuristic checks (subjective)

- [ ] Clarity: one idea, one sentence, S+V+O structure
- [ ] Empathy: non-blaming, supportive, benefit-driven
- [ ] Tone match: for each piece of copy, cross-check phrasing against the loaded user-type tone meter scores. Flag deviations even when no hard rule is violated. Examples:
  - Guru (Murid tribe): Directive 3/10 — directive phrasing (e.g. 'Buat X', 'Pastikan Y') should be flagged and reframed as benefit-driven
  - Kepala Sekolah (GTK): Executive tone — over-explaining or apologetic phrasing should be flagged
  - Murid: Straightforward 3/10 — dense instructional copy should be flagged
- [ ] Action-oriented: user knows what to do next
- [ ] Natural: reads like Indonesian, not translated

### Page/Flow/Audit — Consistency checks (run whenever more than one component is involved)

- [ ] Verb tense consistent across all CTAs
- [ ] Success copy echoes the action label (e.g. `Simpan` → `Tersimpan`)
- [ ] Pronouns consistent throughout
- [ ] Tone shift across arc stages feels intentional, not accidental
- [ ] Glossary terms identical across all touchpoints (no synonym drift)
- [ ] Redundancy: does this copy communicate something already covered by adjacent or nearby copy on the same screen? If yes, recommend removal — include what it duplicates, which copy to keep, and why.

