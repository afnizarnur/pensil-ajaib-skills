---
displayName: "Kementerian"
status: "published"
icon: "🏢"
---

# 📄 SPM Copy Guideline — KEMENTERIAN (STRICT)
_Target User-based Guideline - Always Active_
_Last updated: 12 Feb 2026_

This guide is for generating UX content for **Kementerian (Kemendikdasmen - Bidang BOSP)** using KASDIK. They are the highest-level policy makers in the BOSP ecosystem — communication must be highly formal, authoritative, strategic, and regulation-based.

## Tone Meters (0-10 Scale)
| Trait | Score | Application |
|-------|-------|-------------|
| **Formal & Authoritative** | 10/10 | **PRIMARY**: Bahasa sangat profesional, berwibawa, kredibel |
| **Berorientasi Regulasi** | 9/10 | **SECONDARY**: Setiap aksi harus berlandaskan Juknis |
| **Strategic & Makro** | 8/10 | Fokus pada dampak nasional dan implementasi kebijakan |
| **Directive** | 5/10 | Instruktif sesuai wewenang, tapi tetap berbasis regulasi |

## Addressing Rules
- **Use "Anda"** (formal, respectful)
- Never use "kamu" (too casual)
- **Avoid "Harus/Wajib"** kecuali untuk kebijakan yang bersifat mengikat
- **Use "Maaf"** hanya jika error dari sistem
- **Avoid "!"** kecuali peringatan krusial tingkat nasional
- **Use nomenklatur resmi**: Terminologi sesuai Juknis dan regulasi

## Content Priorities
Kementerian focus on **national policy implementation, data integrity, and timeline management**:

### Primary Motivators
- Sinkronisasi kebijakan nasional
- Transparansi pengelolaan dana
- Implementasi kebijakan tepat waktu
- Integritas data nasional
- Kepatuhan seluruh satuan pendidikan

### Framing Examples
- ✅ "Pengaturan ini akan diterapkan ke seluruh satuan pendidikan setelah disetujui Checker" (formal, jelas)
- ✅ "Pilih sumber dana sesuai Juknis BOSP terbaru (Permendikbudristek No. 63 Tahun 2023)" (rujuk regulasi)
- ✅ "Data akan otomatis terintegrasi dengan MARKAS dan ARKAS setelah aktivasi" (assurance)
- ❌ "Segera selesaikan!" (terlalu mendesak tanpa konteks)
- ❌ "Ada bug di sistem" (jargon teknis)

## Audience Insights

### Reading Patterns
- [KEMEN-AUD-01] **Strategic reader:** Fokus pada dampak makro, bukan detail teknis
  - **Solution:** Front-load dampak nasional di awal kalimat
  - **Solution:** Jangan kasih kalimat panjang, pecah informasi jadi potongan kecil
  - **Solution:** Gunakan tabel atau divider untuk pisahkan kategori informasi
  - **Solution:** Highlight scope dampak (jumlah satdik, daerah terdampak)

### Policy Authority
- [KEMEN-AUD-02] **Expert policy maker:** Pengetahuan tertinggi dalam ekosistem, berbasis regulasi
  - **Solution:** Selalu rujuk Juknis/nomor regulasi sebagai landasan
  - **Solution:** Jelaskan perbedaan dengan regulasi sebelumnya saat ada pembaruan
  - **Solution:** Gunakan terminologi resmi tanpa perlu penjelasan tambahan

### High-Stakes Actions
- [KEMEN-AUD-03] **Aksi berdampak nasional:** Setiap perubahan berdampak ke ribuan sekolah dan ratusan daerah
  - **Solution:** Kalimat persetujuan manual (ketik "SETUJU IMPLEMENTASI")
  - **Solution:** Jelaskan scope dampak dengan sangat jelas sebelum konfirmasi
  - **Solution:** Konfirmasi ganda untuk perubahan kebijakan mayor

### Maker-Checker Flow
- [KEMEN-AUD-04] **Proses Maker-Checker:** Pengaturan perlu persetujuan sebelum aktif
  - **Solution:** Jelaskan status pengajuan dengan jelas (Draft, Diajukan, Disetujui, Ditolak)
  - **Solution:** Notifikasi yang jelas untuk Checker saat ada pengajuan baru
  - **Solution:** Berikan konteks mengapa persetujuan diperlukan

### Data Integrity
- [KEMEN-AUD-05] **Integritas data BOS Salur:** Kegagalan sinkronisasi berdampak ke semua level
  - **Solution:** Solusi di awal dengan timeline perbaikan
  - **Solution:** Jelaskan dampak ke level di bawahnya (MARKAS, ARKAS)
  - **Solution:** Berikan estimasi waktu untuk sinkronisasi ulang

### Timeline Management
- [KEMEN-AUD-06] **Linimasa sangat ketat:** Keterlambatan berdampak pada penyaluran dana nasional
  - **Solution:** Highlight tenggat dengan bold
  - **Solution:** Berikan tracking status implementasi per daerah
  - **Solution:** Tampilkan konflik linimasa antar sumber dana dengan jelas

### Rollback & Override
- [KEMEN-AUD-07] **Rollback kebijakan:** Membatalkan kebijakan yang sudah diimplementasikan
  - **Solution:** Jelaskan dampak rollback secara detail
  - **Solution:** Konfirmasi ganda dengan alasan wajib diisi
  - **Solution:** Notifikasi otomatis ke semua daerah yang terdampak

## Glossary

### KASDIK Terms
- **BOSP Salur** — Sumber data dana BOSP yang dikelola di tingkat pusat
- **Maker** — Peran yang menyusun pengaturan sumber dana di KASDIK
- **Checker** — Peran yang memberikan persetujuan atas pengaturan dari Maker
- **Juknis** — Petunjuk Teknis (rujukan utama kebijakan)
- **Linimasa** — Jadwal atau periode waktu pengelolaan BOSP
- **Sumber Dana** — Konfigurasi dana BOSP (nama, tahun, komponen)
- **Komponen Penganggaran** — Kategori alokasi belanja sesuai Juknis
- **Tahun Anggaran** — Periode waktu pelaksanaan anggaran

### Integration Terms
- **MARKAS** — Sistem untuk Dinas Pendidikan (downstream dari KASDIK)
- **ARKAS** — Sistem untuk Satuan Pendidikan (downstream dari MARKAS)
- **SIPD** — Sistem Informasi Pemerintahan Daerah (Kemendagri)
- **Satuan Pendidikan / Satdik** — Istilah formal untuk sekolah
- **Nomenklatur Subkegiatan** — Terminologi Kemendagri untuk perencanaan anggaran

### Regulatory Terms
- **Permendikbudristek** — Peraturan Menteri Pendidikan, Kebudayaan, Riset, dan Teknologi
- **Implementasi** — Penerapan kebijakan/pengaturan ke MARKAS dan ARKAS

### Padanan Bahasa Indonesia (Wajib)
- **Sinkronisasi** (bukan Sync)
- **Pengaturan** (bukan Settings)
- **Ajukan / Kirim** (bukan Submit)
- **Tenggat** (bukan Deadline)
- **Unduh & Unggah** (bukan Download & Upload)
- **Tautan** (bukan Link)
- **Perbarui** (bukan Update)
- **Terapkan** (bukan Apply/Implement)
- **Pusat Bantuan** (bukan Help Center)

### Terms to Avoid
- "Harus/Wajib" → "Pastikan", "Tetapkan" (kecuali kebijakan mengikat)
- "Server error/bug" → "Terjadi kendala sistem"
- "Di sini" (hyperlink) → "Dokumen ini", "Laman ini"
- Singkatan tanpa penjelasan → Jelaskan saat pertama kali disebut
- Bahasa kasual → Selalu gunakan bahasa formal dan profesional

---


