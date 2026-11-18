# 📏 Style Standards Reference
_Formatting rules only. For tone and principles, see `Core Guidelines/general-foundation.md`. For component-specific rules including character limits and capitalization, see `Reference/ui-component-specs.md`._
_Last updated: 20 Feb 2026_

---

## Capitalization Rules

- [STD-01] **Body text**: Sentence case
- [STD-02] **Headings**: Title Case
- [STD-03] **Form labels**: Title Case
- **CTA buttons, error messages, and other components**: Follow component-specific rules — see `Reference/ui-component-specs.md`

---

## Time Format

- [STD-04] **Standard**: HH:MM WIB
- **Examples**: 06:00 WIB · 14:30 WIB · 23:59 WIB
- **Avoid**: 6:00 WIB (missing leading zero) · 14.30 WIB (dot as separator)

---

## Currency Format

- [STD-05] **Standard**: Rp10.000 (no space between Rp and number)
- **Examples**: Rp5.000 · Rp125.000 · Rp1.500.000
- **Avoid**: Rp 10.000 · Rp10,000 · IDR 10.000

---

## Hyphenation Rules

- [STD-06] Follow KBBI standards. When unsure, check kbbi.kemdikbud.go.id before inventing a form.
- **Examples**:
  - anak-anak ✅
  - anti-korupsi ✅
  - non-formal ✅
  - pro-aktif ❌ → proaktif ✅
  - multi-media ❌ → multimedia ✅

---

## Number Formatting

- [STD-07] **Thousands separator**: Use period (.)
- [STD-08] **Decimal separator**: Use comma (,)
- **Examples**: 1.000 · 1.500,50
- **Avoid**: 1,000 · 1.500.50

---

## Date Formatting

- [STD-09] **Long format**: 15 Agustus 2024
- [STD-10] **Short format**: 15/08/2024
- **Avoid**: Aug 15, 2024 · 15 Aug 2024 · 15/8/24 (abbreviated month or year)

---

## Percentage

- [STD-11] **Format**: 75% (no space between number and symbol)
- **In UI labels and data displays**: Use %
- **In body copy sentences**: Write "75 persen"

---

## Lists

- [STD-12] Use • for unordered lists
- [STD-13] Use 1. 2. 3. for ordered/sequential lists
- Do not mix bullet styles within the same list

---

## Quotation Marks

- [STD-14] **Standard**: "teks yang dikutip"
- [STD-15] **Nested quotes**: 'kutipan dalam kutipan'
- **Avoid**: English-style curly quotes " " or straight quotes ' ' outside of code blocks

---

## Dashes & Hyphens

- [STD-16] **Range (en dash –)**: 2024–2025 · Senin–Jumat · 08:00–17:00
- [STD-17] **Compound word (hyphen -)**: anak-anak · non-formal
- **Avoid**: Using hyphen for ranges · using em dash (—) in UI copy

---

## Ellipsis

- [STD-18] **In prose**: ... (three periods, no space before)
- [STD-19] **In UI truncation**: Use OS/component-native truncation — do not manually add ellipsis in copy
- **Avoid**: "dan lain-lain..." (dll. already implies continuation)

---

## Abbreviations

- [STD-20] **dll.** always ends with a period
- [STD-21] **Educational levels**: PAUD, SD, SMP, SMA, SMK (always uppercase, no periods)
- [STD-22] **Kemendikdasmen**: Not abbreviated in formal UI copy or official documents
- [STD-23] **Timezones (WIB, WITA, WIT)**: Always uppercase, always explicit in time displays

---

## File Extensions

- [STD-24] **In code/technical contexts**: Always lowercase (.pdf, .docx, .xlsx)
- [STD-25] **In UI copy**: "berkas PDF" or "dokumen PDF" — format name uppercase, extension lowercase in filenames
