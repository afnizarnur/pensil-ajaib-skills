# ♿ Accessibility & Inclusivity Guidelines (INC)
_Foundation - Always Active_
_Last updated: 6 Apr 2026_

*Applies to all generated output (UI copy, system messages, documentation, alt text).*

**Rule Precedence:** Core Principles override category-specific rules if conflicts occur.

---

## **Core Principles**

Apply to all output types. When in doubt, follow these principles.

### **\[INC-PR-01\] Use descriptive, action-oriented language**

* Use verbs that describe actions.  
* Avoid perception-based verbs (lihat, tonton, baca).  
* State required actions explicitly.

**Examples**

❌ "Lihat hasil penilaian Anda."

✅ "Cek hasil penilaian Anda."

❌ "Tonton video berikut."

✅ "Putar video berikut."

### **\[INC-PR-02\] Use simple, clear, and neutral wording**

* Avoid slang, jargon, and unexplained abbreviations.  
* Define abbreviations at first mention.  
* Express one idea per sentence.  
* Avoid decorative or witty phrasing that reduces clarity.

**Examples**

❌ "Terjadi server error timeout. Hubungi CS."

✅ "Terjadi kendala sistem. Kunjungi Pusat Bantuan atau coba lagi."

❌ “Buah ceri, buah pisang. Yuk mulai sekarang!”

✅ “Mulai sekarang untuk melihat hasil Anda.”

### **\[INC-PR-03\] Place critical information first**

* Especially for errors and blocking states.  
* Avoid filler before the main issue.

**Examples**

❌ "Sepertinya ada sedikit kendala. Koneksi Anda terputus."

✅ "Koneksi Anda terputus. Coba muat ulang halaman."

### **\[INC-PR-04\] Do not rely on visual or positional cues**

* Do not depend solely on color, icon, layout, or audio.  
* Directional cues may support meaning but cannot replace text.  
* Do not use icon-only labels.

**Examples**

❌ “Tekan ikon kuning ✨ di bawah.”

✅ “Tekan tombol Mulai.”

❌ “❓”

✅ “Bantuan”

### **\[INC-PR-05\] Avoid stereotypes and assumptions**

Do not assume:

* Gender  
* Religion  
* Ethnicity or region  
* Socioeconomic status  
* Education level  
* Device ownership  
* Tech literacy  
* Ability

Use inclusive forms of address (“Anda” or “Kamu”) unless role context requires otherwise.

**Examples**

❌ "Selamat datang, Bapak Kepala Dinas."

✅ "Selamat datang, Hendrawan."

❌ "Para ibu guru dapat mengakses fitur ini."

✅ "Guru dapat mengakses fitur ini."

### **\[INC-PR-06\] Provide clear structure and expectations**

* Break multi-step processes into steps.  
* Indicate progress when relevant.  
* Separate ideas using UI structure (title, body, etc.).

❌ "Perbarui data."

✅ "Perbarui data (1 dari 3 tahap)."

## ---

## **Category Rules**

Only add constraints not already covered by Core Principles.

### **Gender Neutrality**

#### **\[INC-CAT-01\] Use gender-neutral professional language**

* Avoid gendered titles unless explicitly provided.  
* Use role names instead of gendered references.

### **Religious Neutrality**

#### **\[INC-CAT-02\] Avoid religious framing in generic UI**

* Use neutral greetings and success messages.  
* Use “libur nasional” unless context specifically requires religious naming.

❌ "Spirit animal"

✅ "Hewan favorit"

### **Cultural and Language Neutrality**

#### **\[INC-CAT-03\] Use standard Indonesian**

* Avoid regional dialects or Bahasa Daerah unless context-specific.  
* Do not associate ethnicity with stereotypes.  
* Use diverse names and regional examples. Can reference [https://developers.google.com/style/examples\#names](https://developers.google.com/style/examples#names)   
* Use examples like “Email addresses: support@example.net”, “info@contoh.id”.

#### **\[INC-CAT-04\] Avoid problematic legacy English terms**

Avoid exclusionary metaphors or color-based hierarchy terms.

**Examples**

❌ "Whitelist"

✅ "Didaftarkan (*whitelist*)"

❌ "Blacklist"

✅ "Diblokir (*blacklist*)"

❌ "Master copy"

✅ "Salinan utama"

❌ "Citizen"

✅ "Publik", "Masyarakat"

### **Socioeconomic Inclusion**

#### **\[INC-CAT-05\] Do not assume access or privilege**

Do not assume:

* Laptop ownership  
* E-wallet usage  
* Stable internet  
* Formal higher education  
* International travel  
* Car ownership

#### **\[INC-CAT-06\] Avoid deficit framing**

Focus on specific conditions rather than labeling people by lack.

**Examples**

❌ “Orang tidak mampu”

✅ “Keluarga dengan pendapatan di bawah Rp X per bulan”

❌”Drop-out”

✅ “Siswa yang menyelesaikan pendidikan hingga tingkat SMP”

❌ "Mata kuliah favorit kamu saat kuliah?", "Kapan kamu beli mobil pertama?", "Cerita pengalaman liburan ke luar negeri"

✅ "Hobi favorit kamu?", "Cerita pengalaman belajar yang berkesan". Use generic names like fruit, flowers, vegetable, etc.

#### **\[INC-CAT-07\] Use specific group names**

Avoid vague umbrella labels like “minoritas” when referring to services.

**Examples**

❌ "Minoritas”, “Layanan untuk minoritas", "Kelompok minoritas di Indonesia"

✅ "Layanan untuk penyandang disabilitas dan masyarakat adat", "Dukungan untuk kelompok yang kurang terlayani"

### **Disability Terminology**

Follow Undang-Undang Nomor 8 Tahun 2016 tentang Penyandang Disabilitas.

#### **\[INC-CAT-08\] Use respectful, current terminology**

* Use person-first language unless a community-specific identity term is widely accepted (e.g., “Tuli”).  
* Avoid outdated prefixes such as “tuna-”.  
* Avoid pejorative or medicalized framing.  
* Avoid afflicting language (e.g., “korban dari…”).

**Examples**

❌  “Cacat”, “Sakit”, “Kelainan”, “Berkebutuhan khusus”, “Luar biasa”

✅“Difabel”, "Penyandang Disabilitas \[type\]"

❌ “Tuna Netra”

✅ “Penyandang disabilitas netra”, “Disabilitas netra”

❌ “Tuna Rungu”, “Tunarungu”, “Budek”

✅ “Tuli”, “Teman Tuli”, “Penyandang disabilitas tuli”, “Mengalami keterbatasan pendengaran”, “Tuli parsial”

❌ “Tunawicara”

✅ “Bisu”, “Penyandang disabilitas bisu”, “penyandang disabilitas wicara”

❌ “Cacat”, “Penyandang cacat”, “Tuna daksa”

✅ “Penyandang disabilitas fisik”, “Penyandang disabilitas daksa”, “Mengalami keterbatasan mobilitas”. “Mengalami kesulitan menggunakan dan menggerakkan tangan/jari”

❌ “Kegilaan”, “Orang gila”, “Penderita gangguan jiwa”

✅ “Masalah kesehatan mental”, “ODGJ (Orang Dengan Gangguan Jiwa)”, “ODMK (Orang Dengan Masalah Kejiwaan)”

❌ "Trigger warning"

✅ "Peringatan konten",  "Konten mengandung..."

❌ "Korban AIDS", “Orang HIV”, “Orang AIDS”

✅ "ODHA”, “Orang dengan HIV/AIDS”

#### **\[INC-CAT-09\] Use precise assistive terminology**

Use correct names for assistive systems and tools.

**Examples**

❌ “Bahasa tangan”

✅ “Bahasa isyarat”

❌ “Alat tuli”

✅ “Alat Bantu Dengar (ABD)”

### **Alt Text**

Only apply when generating alt text.

#### **\[INC-CAT-10\]  Provide alt text only if meaningful**

* Skip purely decorative images.

#### **\[INC-CAT-11\] Alt text format**

* Do not repeat visible text.  
* Describe new or functional information.  
* Sentence case.  
* Active voice.  
* End with a period.  
* No abbreviations

#### **\[INC-CAT-12\] Functional images describe purpose**

Describe what the element does, not how it looks.

**Examples**

❌ “Ikon tanda tanya berwarna biru.”

✅ “Tombol bantuan untuk membuka panduan.”
