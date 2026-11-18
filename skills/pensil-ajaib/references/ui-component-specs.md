# 🖥️ UI Component Specifications
_Only when building specific components. Character limits here are the source of truth — they take priority over any limits stated elsewhere._
_Last updated: 20 Feb 2026_

---

## [UI-CTA] CTA Buttons
**Limits:** ≤20 characters · max 2–3 words
**Rules:**
- MUST use action verbs
- Title Case, no period
- Context-specific and direct

**Universal CTAs:**
- **Login**: Masuk
- **Back**: Kembali / Sebelumnya
- **Search**: Cari
- **Save**: Simpan
- **Share**: Bagikan
- **Next**: Selanjutnya
- **Refresh**: Muat Ulang
- **Home**: Kembali ke Beranda

---

## [UI-TTL] Title / Heading
**Limits:** ≤8 words
**Rules:**
- If phrase: use Title Case
- If a full sentence: use Sentence Case
- No period at end
- Must describe the content or action of the screen clearly

---

## [UI-BDY] Body Text / Paragraph
**Limits:** ≤20 words per sentence
**Rules:**
- Sentence case
- Active voice preferred
- One idea per sentence; break complex information into separate sentences or a list

---

## [UI-TTP] Tooltip
**Limits:** ≤60 characters
**Rules:**
- Sentence case
- Max 1–2 sentences
- Provide brief, relevant info
- Avoid excessive detail or jargon

---

## [UI-TST] Toast Messages (Snackbar)
**Limits:** ≤40 characters
**Rules:**
- Sentence case
- Max 1 sentence or 2 lines
- Add CTA only if essential
- Prioritize clarity and relevance

**Common Patterns:**
- Success: "Berhasil [action]"
- Error: "Terdapat kendala. Silakan coba lagi."
- Info: "[Status update message]"

---

## [UI-CNF] Confirmation Dialog
**Limits:** title ≤50 characters · body ≤150 characters
**Rules:**
- Title: Title Case
- Body: Sentence case
- Clarify action + consequence
- Use exact verbs in CTA
- Avoid unnecessary details

**Structure:**
1. **Clear question as title**
2. **Consequence explanation**
3. **Specific action CTA + Cancel option**

---

## [UI-ERR] Error Messages
**Limits:** ≤100 characters
**Capitalization:** Follows host component
- In dialog title → Title Case
- In snackbar/toast → Sentence case
**Rules:**
- Avoid technical jargon or error codes
- Keep tone neutral, not blaming
- Provide actionable solutions

**Standard Errors:**
- **General**: "Terdapat Kendala Sistem. Silakan coba beberapa saat lagi."
- **Connection**: "Terdapat Gangguan Koneksi. Periksa kembali koneksi internetmu dan muat ulang dalam beberapa saat."
- **404**: "Halaman Tidak Ditemukan. Halaman ini sedang tidak dapat diakses."

---

## [UI-HLP] Helper Text (Form Input)
**Limits:** ≤80 characters
**Rules:**
- Sentence case
- Simple and direct
- Reinforce the input's purpose
- Use positive phrasing

**Pattern:**
```
[Field Name]
[Clear instruction or example]
```

---

## [UI-LOD] Loading States
**Limits:** ≤50 characters
**Rules:**
- Sentence case
- Be practical and straightforward
- Be clear about what user can expect
- Give assurance

**Pattern:**
```
[Action] Sedang [Process]
[Brief explanation if needed]
[Optional tip for better experience]
```

---

## [UI-CHK] Checkboxes
**Limits:** ≤40 characters
**Rules:**
- Sentence case
- Use positive statement format
- Short and unambiguous
- Explain consequences where needed

---

## [UI-EMP] Empty State
**Rules:**
- Sentence case for body, Title Case for heading
- Explain why the screen is empty
- Provide clear next steps
- Stay optimistic and solution-oriented

**Structure:**
1. **Clear title** explaining why empty
2. **Helpful subtitle** with next steps
3. **Optional CTA** for primary action

---

## [UI-ONB] Onboarding Screens
**Limits:** headline ≤8 words
**Rules:**
- Headline: Title Case
- Body: Sentence case
- Explain benefits clearly
- Encourage first actions
- One short paragraph per screen
- Use "Mulai Sekarang" type CTAs

---

## [UI-INF] Information Cards
**Limits:** title ≤30 characters · body ≤100 characters
**Rules:**
- Title: Title Case
- Body: Sentence case, active voice
- Scannable format

---

## [UI-CMK] Coach Marks
**Limits:** ≤60 characters
**Rules:**
- Sentence case
- Be action-oriented
- Limit to necessary guidance only
- No fluff
- Point to specific UI elements
