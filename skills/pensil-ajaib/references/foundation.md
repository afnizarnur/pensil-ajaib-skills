# 🏛️ General Foundation Guidelines
_Foundation - Always Active_
_Last updated: 7 Apr 2026_

## **Language & Output Enforcement (Non‑Negotiable)**

* [CORE-01] All visible UI copy MUST be written in Bahasa Indonesia, following KBBI standards  
* DO NOT use English words, mixed language, slang, or untranslated technical terms in any UI text.  
* DO NOT translate from English sentence structures. Write as if **Bahasa Indonesia is the source language**, not a translation target.  
* If any English word appears in visible UI copy, the output is considered invalid  

## **Core Communication Principles**

These principles apply to every piece of copy, regardless of component or context:  
* [PRI-01] Write with empathy: Understand user constraints and context. Provide helpful, relevant guidance.  
* [PRI-02] Be clear and concise: Reduce text wherever possible without sacrificing meaning or accuracy.  
* [PRI-03] Guide, do not command: Use supportive, enabling language rather than instructional or authoritarian phrasing.  
* [PRI-04] Stick to verifiable fact: Ensure accuracy and alignment with official regulations and institutional sources.  
* [PRI-05] Inclusive: DO NOT use slang. DO NOT assume gender, region, age, or background.  
* [PRI-06] Tone is calibrated per tribe and audience: These principles are universal. For voice, formality level, and phrasing style, refer to tribe-specific guidelines.  

## **Government Context Rules**

* \[GOV-01\] Prioritize clarity over stylistic tone when space is limited.  
* Maintain a **neutral and respectful tone** at all times.  
* Treat the platform as an official government system.  
* Follow KBBI, applicable regulations, and official institutional language.  

## **Typography**

| Element | Case | Example |
| :---- | :---- | :---- |
| Page titles | Title Case | Pemetaan Kebutuhan |
| Headings | Title Case | Seleksi Administrasi |
| Table headers | Title Case | Nama Lengkap |
| Roles | Title Case | Guru, Kepala Sekolah, Murid |
| Proper nouns (institutional) | Title Case | Direktorat Jenderal GTK |
| Body text | Sentence case | Silakan pilih. |
| Buttons | Per tribe guideline | Ajukan formasi / Ajukan Formasi |
| Form labels | Sentence case | Nama lengkap |
| Abbreviations | UPPERCASE | GTK, NIP |

## **Style Standards**

* [STD-01] Time format: HH:MM WIB (e.g., 06:00 WIB)  
* [STD-02] Currency format: Rp10.000 (no space)  
* [STD-03] Hyphenation must follow KBBI. Examples: anak-anak, anti-korupsi  

## **UI Component Copy Specifications**

### **CTA Buttons**

* MUST use clear action verbs  
* Maximum 2–3 words  
* Case follows tribe guideline (Murid: Title Case)  
* No punctuation  
* Context‑specific and outcome‑oriented  
* Content pattern: Kirim, Simpan, Batal, Hapus, Ubah, Tambah, Cari, Cek Detail, Unduh, Unggah Berkas

### **Form Fields**

* Input label="Nama lengkap" placeholder="Masukkan nama lengkap" 
* Select label="Provinsi" placeholder="Pilih provinsi" 
* helperText="Wajib diisi"  
* helperText="Format: DD/MM/YYYY"  
* helperText="Maksimum 500 karakter"

### **Validation**

* Error  
  * "Wajib diisi"  
  * "Format tidak valid"  
  * "Ukuran berkas melebihi batas maksimum 5 MB"  
  * “Gagal simpan data. Coba lagi.”  
* Success  
  * "Berhasil simpan data\!"  
  * "Berhasil unggah berkas\!"

### **Toast Messages**

* Maximum one sentence or two short lines  
* Include a CTA only if it is essential  
* Prioritize clarity over tone

### **Error Messages**

* Avoid technical jargon and error codes  
* Use neutral, non‑blaming language  
* Provide clear, actionable next steps

### **Modals**

* \<ModalHeader\>Konfirmasi \[Action\]\</ModalHeader\>  
* \<ModalBody\>Apakah Anda yakin? \[Consequence\]\</ModalBody\>  
* \<ModalFooter\>  
  * \<Button variant="secondary"\>Kembali\</Button\>  
  * \<Button variant="danger"\>Hapus\</Button\>  
* \</ModalFooter\>

### **Empty States**

* Explain why the screen is empty  
* Provide clear guidance on what users can do next  
* Maintain an optimistic, solution‑oriented tone  
* Content pattern:   
  * \<Text\>Belum ada data tersedia\</Text\>  
  * \<Text\>\[Guidance on what to do\]\</Text\>  
  * \<Button\>\[Action\]\</Button\>

## **Glossary Consistency & Fallback Rules**

* You MUST ALWAYS use approved glossary terms consistently.  
* DO NOT invent synonyms or alternative terms.  

## **Fallback Protocol**  
If a required term does not exist in the glossary, you MUST first reference official terminology used on: [https://rumah.pendidikan.go.id](https://rumah.pendidikan.go.id/)  
Only introduce a new term if no official equivalent exists.
