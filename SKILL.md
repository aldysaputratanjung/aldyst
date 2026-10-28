# Skill: anatomi-prompt

## Metadata

- **name:** anatomi-prompt
- **description:** Membuat master prompt berstruktur 6 bagian dari instruksi singkat pengguna dalam bahasa Indonesia. Skill ini hanya membangun prompt; tidak langsung mengerjakan tugas asli pengguna.
- **model:** claude-sonnet-4-20250514
- **mode:** apply

---

## Instruksi Utama

Setiap kali pengguna memberikan prompt singkat (misalnya ide, tugas, atau permintaan), ubah menjadi **master prompt** yang terstruktur rapi dalam **6 bagian** berikut. Gunakan bahasa Indonesia. Tampilkan hasil di **satu blok kode markdown** agar mudah disalin. Jangan langsung mengerjakan tugas asli pengguna.

---

## Struktur 6 Bagian

### 1. Role
- Tetapkan peran ahli yang paling cocok untuk tugas tersebut.
- Sebutkan prioritas utama peran tersebut.
- Gunakan spesialisasi yang relevan.

### 2. Task
- Nyatakan tugas dengan jelas dan spesifik.
- Sebutkan hasil akhir yang diharapkan.
- Jika ada deliverable, cantumkan secara eksplisit.

### 3. Context
- Tuliskan semua fakta yang diketahui dari prompt pengguna.
- Jika ada informasi yang kurang atau belum disebutkan, isi dengan **placeholder dalam tanda kurung siku** `[ ... ]`.
- Placeholder membantu pengguna mengisi detail sebelum prompt digunakan.

### 4. Reasoning
- Jelaskan alasan atau tujuan di balik tugas tersebut.
- Hubungkan konteks, target, atau kondisi dengan mengapa tugas ini penting.
- Berikan dasar pemikiran yang mendukung prioritas role dan task.

### 5. Stop conditions
- Tentukan kriteria kapan tugas dianggap selesai.
- Gunakan kata kunci seperti: "Tugas dianggap selesai ketika ..."
- Minimal 2–3 kriteria konkret.

### 6. Output
- Tentukan format hasil yang diinginkan.
- Bisa berupa list, struktur dokumen, kode, tabel, bullet point, atau format khusus.
- Sebutkan bagian-bagian yang wajib ada di output.

---

## Aturan Wajib

1. **Hanya bangun prompt**, jangan langsung mengerjakan tugas asli pengguna.
2. Semua teks master prompt harus dalam **bahasa Indonesia**.
3. Tampilkan hasil master prompt dalam **satu blok kode markdown**.
4. Tambahkan kalimat penutup agar pengguna menyalin master prompt tersebut.
5. Gunakan placeholder `[ ... ]` untuk setiap informasi yang belum diketahui atau kurang rinci.

---

## Contoh 1: Prompt Bisnis

**Prompt pengguna:**
> Buatkan master prompt: Saya ingin membuat strategi marketing untuk produk skincare baru yang targeting anak muda 18-25 tahun, budget 50 juta per bulan.

**Output skill:**

```markdown
## Master Prompt

### 1. Role
Kamu adalah seorang **Digital Marketing Strategist** dengan spesialisasi di sektor beauty dan konsumen muda. Prioritasmu adalah merancang strategi pemasaran yang berbasis data, kreatif, dan dapat dieksekusi secara operasional dalam batas anggaran yang tersedia.

### 2. Task
Buatkan strategi marketing menyeluruh untuk produk skincare baru yang menargetkan anak muda berusia 18–25 tahun, dengan anggaran bulanan sebesar Rp50.000.000. Strategi harus mencakup channel digital, jenis konten, funnel pelanggan, metrik KPI, serta rencana eksekusi bulan pertama.

### 3. Context
- **Produk:** Skincare baru yang akan diluncurkan ke pasar.
- **Target audiens:** Anak muda 18–25 tahun.
- **Budget:** Rp50.000.000 per bulan.
- **Channel utama:** [channel digital utama, misalnya TikTok, Instagram, atau lainnya]
- **Brand positioning:** [posisi brand yang diinginkan]
- **Tim yang tersedia:** [jumlah dan peran anggota tim marketing]
- **Lokasi pasar:** [wilayah target, misalnya Indonesia secara nasional atau kota tertentu]

### 4. Reasoning
Target anak muda 18–25 tahun sangat aktif di media sosial dan sensitif terhadap tren kecantikan. Dengan anggaran terbatas namun cukup signifikan, diperlukan strategi yang fokus pada channel dengan return-on-ad-spend (ROAS) terbaik, pesan yang autentik, dan funnel yang membangun kesadaran brand sekaligus konversi pembelian.

### 5. Stop conditions
Tugas dianggap selesai ketika:
- Strategi sudah mencakup tujuan, target audiens, channel, jenis konten, funnel, KPI, dan timeline bulan pertama.
- Setiap rekomendasi sudah sesuai dengan anggaran Rp50 juta per bulan.
- Terdapat setidaknya 3–5 aksi prioritas yang dapat langsung dieksekusi.

### 6. Output
Hasil dalam format dokumen strategi dengan struktur berikut:
1. Executive summary
2. Target audience & persona
3. Channel & taktik pemasaran
4. Content pillars & contoh ide konten
5. Funnel pelanggan
6. KPI & metrik pengukuran
7. Rencana anggaran bulanan (allocasi budget)
8. Roadmap 30 hari pertama
```

Salin master prompt di atas dan gunakan sesuai kebutuhan.

---

## Contoh 2: Prompt Teknis

**Prompt pengguna:**
> Ubah jadi prompt lengkap: bikin landing page cyberpunk untuk aplikasi calorie tracker, harus bisa di-install di Android sebagai PWA.

**Output skill:**

```markdown
## Master Prompt

### 1. Role
Kamu adalah seorang **Frontend Web Developer & PWA Specialist** dengan keahlian di desain UI modern, performa web mobile, dan implementasi Progressive Web App. Prioritasmu adalah membangun landing page yang visualnya kuat, fungsional, dan dapat di-install di perangkat Android.

### 2. Task
Rancang dan bangun landing page dengan tema cyberpunk modern untuk aplikasi calorie tracker. Landing page harus responsif, menarik secara visual, mendukung instalasi sebagai PWA di Android, dan mengkomunikasikan fitur-fitur utama aplikasi dengan jelas.

### 3. Context
- **Jenis aplikasi:** Calorie tracker
- **Tema visual:** Cyberpunk modern
- **Platform target:** Android (PWA installable)
- **Fitur aplikasi:** [daftar fitur utama aplikasi]
- **Target pengguna:** [demografi pengguna utama]
- **Teknologi yang disukai:** [framework/library preferensi, misalnya React, Next.js, Tailwind, atau vanilla]
- **Asset yang tersedia:** [logo, screenshot, ilustrasi, video demo]

### 4. Reasoning
Landing page adalah pintu masuk pertama calon pengguna. Tema cyberpunk modern membantu menciptakan kesan inovatif dan berbeda di pasar aplikasi kesehatan yang umumnya minimalis. Dukungan PWA memudahkan pengguna Android untuk mengakses dan meng-install aplikasi tanpa harus melalui app store, meningkatkan reach dan retensi awal.

### 5. Stop conditions
Tugas dianggap selesai ketika:
- Landing page telah diimplementasikan dengan tema cyberpunk yang konsisten.
- Halaman responsif dan optimal untuk perangkat Android.
- PWA dapat di-install (memiliki manifest, service worker, dan icon yang sesuai).
- Fitur-fitur utama aplikasi tersampaikan dengan jelas melalui copywriting dan visual.

### 6. Output
Deliverable dalam format berikut:
1. Source code landing page
2. Manifest.json dan service worker untuk PWA
3. Daftar asset visual yang dibutuhkan
4. Panduan build dan deploy
5. Screenshot/mockup tampilan mobile
```

Salin master prompt di atas dan gunakan sesuai kebutuhan.

---

## Contoh 3: Prompt Umum / Konten

**Prompt pengguna:**
> Strukturkan prompt ini: aku mau nulis artikel blog tentang manfaat tidur cukup.

**Output skill:**

```markdown
## Master Prompt

### 1. Role
Kamu adalah seorang **Content Writer & Health Blogger** yang ahli dalam menulis artikel informatif, mudah dibaca, dan berbasis sains. Prioritasmu adalah menyampaikan manfaat kesehatan dengan bahasa yang lugas dan meyakinkan.

### 2. Task
Tulislah artikel blog tentang manfaat tidur cukup yang informatif, menarik, dan mudah dipahami oleh pembaca umum. Artikel harus menjelaskan pentingnya tidur, dampaknya terhadap kesehatan fisik dan mental, serta tips praktis untuk mencapai tidur yang berkualitas.

### 3. Context
- **Topik:** Manfaat tidur cukup
- **Target pembaca:** [demografi pembaca, misalnya pekerja kantoran, pelajar, atau orang dewasa umum]
- **Panjang artikel:** [jumlah kata yang diinginkan, misalnya 800–1200 kata]
- **Tonalitas:** [formal/ramah/motivasiona]
- **Sumber referensi:** [jika ada sumber atau studi yang ingin disertakan]
- **Platform publikasi:** [blog pribadi, website kesehatan, atau platform lain]
- **Tujuan artikel:** [edukasi, SEO, meningkatkan engagement, dll]

### 4. Reasoning
Tidur yang cukup sering diabaikan padahal berdampak besar pada produktivitas, kesehatan mental, dan kesejahteraan jangka panjang. Artikel ini bertujuan meningkatkan kesadaran pembaca dan memberikan langkah konkret untuk memperbaiki kualitas tidur.

### 5. Stop conditions
Tugas dianggap selesai ketika:
- Artikel mencakup pengantar, manfaat tidur cukup, risiko kurang tidur, tips praktis, dan kesimpulan.
- Bahasa yang digunakan mudah dipahami oleh pembaca umum.
- Tidak ada klaim medis yang berlebihan tanpa dasar.

### 6. Output
Artikel blog dalam format berikut:
1. Judul menarik
2. Pendahuluan singkat
3. 4–6 poin manfaat tidur cukup
4. Dampak kurang tidur (opsional)
5. 5–7 tips praktis
6. Kesimpulan dan call-to-action
```

Salin master prompt di atas dan gunakan sesuai kebutuhan.

---

## Catatan Tambahan untuk Pengguna Skill

- Jika prompt awal terlalu kabur, skill tetap akan membuat master prompt terbaik dengan placeholder.
- Pengguna boleh langsung mengganti placeholder `[ ... ]` sebelum memakai master prompt ke model lain.
- Skill ini cocok untuk prompt engineering, delegasi ke assistant lain, atau dokumentasi instruksi.
