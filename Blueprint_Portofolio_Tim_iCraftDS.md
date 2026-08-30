# BLUEPRINT WEBSITE PORTOFOLIO TIM
## iCraftDS Internship 2026

**Anggota Tim:** Bhadriko, Alfan, Iqbal  
**Konsep:** Modern Professional Tech Portfolio  
**Stack yang direkomendasikan:** HTML + Tailwind CSS v4 + JavaScript seperlunya  
**Target:** Website profil tim + CV individu + portofolio yang live dan responsif

---

# 1. KONSEP BESAR

Website diarahkan sebagai **modern professional tech portfolio**.

Karakter visual:

- Clean
- Modern
- Profesional
- Sedikit futuristic
- Banyak whitespace
- Card dengan rounded corner
- Typography besar dan tegas
- Aksen warna yang konsisten
- Tidak terlalu ramai
- Fokus pada tiga individu dan kemampuan mereka

Website harus terasa seperti:

> "Ini website portfolio sebuah tim profesional."

Bukan:

> "Ini website tugas mahasiswa."

Jangan menyalin website referensi iCraftDS secara 1:1. Ambil struktur, standar informasi, dan feel yang relevan, lalu bangun identitas visual tim sendiri.

---

# 2. STRUKTUR FULL WEBSITE

Urutan utama:

```text
NAVBAR
│
├── HOME
├── ABOUT
├── TEAM
├── PROJECTS
├── EXPERIENCE
└── CONTACT
│
▼
HERO
│
▼
ABOUT THE TEAM
│
▼
TEAM MEMBERS
│
├── BHADRIKO
├── ALFAN
└── IQBAL
│
▼
OUR EXPERTISE
│
▼
PROJECTS / PORTFOLIO
│
▼
EXPERIENCE & EDUCATION
│
▼
DOCUMENTS / CV
│
▼
CONTACT
│
▼
FOOTER
```

Karena requirement perusahaan meminta **CV individu**, CV tidak hanya ditampilkan sebagai PDF. Informasi utama setiap anggota harus dapat dibaca langsung di website, sedangkan PDF menjadi dokumen pendukung.

---

# 3. DESIGN SYSTEM

Semua anggota tim wajib mengikuti design system yang sama.

Jangan setiap halaman memilih warna, radius, font, atau spacing sendiri.

## 3.1 Background

Primary Background:

```text
#0A0A0B
```

Alternatif yang sedikit lebih soft:

```text
#0F1012
```

## 3.2 Surface

Card:

```text
#151619
```

Secondary Surface:

```text
#1B1D21
```

Border:

```text
rgba(255,255,255,0.08)
```

Gunakan border tipis. Jangan menggunakan border putih terang.

---

# 4. COLOR PALETTE

Gunakan satu accent color utama.

Rekomendasi:

```text
Primary:
#7C5CFC

Primary Hover:
#6847F5

Secondary:
#A78BFA
```

Neutral:

```text
White:
#FFFFFF

Text Primary:
#F5F5F5

Text Secondary:
#A1A1AA

Text Muted:
#71717A
```

Ringkasan:

```text
Background     #0A0A0B
Surface        #151619
Border         rgba(255,255,255,0.08)

Primary        #7C5CFC
Secondary      #A78BFA

Heading        #FFFFFF
Body           #A1A1AA
Muted          #71717A
```

Jika nantinya ditemukan warna identitas resmi iCraftDS yang lebih tepat dari website referensi, accent color dapat disesuaikan agar tetap selaras dengan identitas perusahaan.

---

# 5. TYPOGRAPHY

## 5.1 Font

Rekomendasi utama:

**Plus Jakarta Sans**

Alternatif:

**Inter**

## 5.2 Hierarchy

Desktop:

```text
Hero Heading:
64px / 72px
Weight 700-800

Section Heading:
42px / 52px
Weight 700

Card Heading:
22px / 28px
Weight 600-700

Body:
16px / 26px

Small:
14px / 20px
```

Mobile:

```text
Hero:
40px

Section:
32px

Card:
20px

Body:
15-16px
```

Gunakan hierarchy yang konsisten di seluruh website.

---

# 6. NAVBAR

Navbar harus sederhana, modern, dan tidak memakan banyak ruang.

Konsep desktop:

```text
┌─────────────────────────────────────────────────────┐
│  [LOGO]    About   Team   Projects   Experience    │
│                                      [Contact ↗]   │
└─────────────────────────────────────────────────────┘
```

Spesifikasi:

- Fixed atau sticky di bagian atas
- Lebar sekitar 90%
- Max-width sekitar 1200px
- Centered
- Background semi-transparan
- Backdrop blur
- Border tipis
- Z-index tinggi

Background:

```text
rgba(10,10,11,0.75)
```

Logo dapat berupa nama tim setelah nama tim ditentukan.

Contoh sementara:

```text
BHADRIKO × ALFAN × IQBAL
```

Mobile:

- Gunakan hamburger menu
- Menu muncul sebagai dropdown atau mobile drawer
- Jangan memaksakan semua menu tampil horizontal

---

# 7. HERO SECTION

Hero adalah bagian paling penting untuk membangun first impression.

Hindari pembuka yang terlalu generik seperti:

> "Halo, kami dari kelompok..."

Gunakan headline yang kuat.

Contoh:

```text
TEAM PORTFOLIO
iCraftDS INTERNSHIP

We Build.
We Learn.
We Create.

A team of three individuals with
different skills, united by one goal:
creating meaningful digital experiences.

[ Meet The Team ]
[ Our Projects ]
```

## 7.1 Hero Layout

Desktop dapat menggunakan dua kolom:

```text
┌────────────────────────────────────────────────────┐
│                                                    │
│  TEAM PORTFOLIO               TEAM VISUAL          │
│                                                    │
│  We Build.                    ┌───────────────┐    │
│  We Learn.                    │      01       │    │
│  We Create.                   │               │    │
│                               │   BHADRIKO    │    │
│  Description...               │   ALFAN       │    │
│                               │   IQBAL       │    │
│  [Meet Team] [Projects]       └───────────────┘    │
│                                                    │
└────────────────────────────────────────────────────┘
```

Visual sebelah kanan dapat diganti dengan:

- Foto ketiga anggota
- Komposisi portrait
- Abstract team graphic
- Typography nama anggota
- Elemen visual minimalis

Jangan menggunakan terlalu banyak elemen.

---

# 8. HERO VISUAL

Background hero dapat menggunakan:

- Radial gradient
- Subtle grid
- Blur blob
- Noise ringan

Konsep:

```text
Background:
#0A0A0B

             purple glow
                  ↓

        ╭────────────────╮
        │                │
        │   HEADLINE     │
        │                │
        ╰────────────────╯
```

Gradient harus subtle.

Tujuannya memberikan depth, bukan membuat halaman menjadi penuh warna.

Hindari efek neon yang terlalu kuat.

---

# 9. ABOUT THE TEAM

Setelah Hero, tampilkan pengenalan singkat tentang tim.

Judul:

```text
ABOUT US

Who We Are
```

Layout dua kolom:

```text
┌──────────────────────┬─────────────────────────┐
│                      │                         │
│   ABOUT OUR TEAM     │  TEAM PHILOSOPHY       │
│                      │                         │
│   paragraph          │  "Learn → Build →      │
│                      │   Improve"              │
│                      │                         │
└──────────────────────┴─────────────────────────┘
```

Konten:

- Siapa tim ini
- Apa tujuan tim
- Bagaimana cara bekerja
- Fokus kemampuan
- Nilai atau prinsip tim

Target panjang:

**80-120 kata**

Jangan membuat paragraf terlalu panjang.

---

# 10. TEAM MEMBERS

Ini merupakan salah satu bagian inti website.

Judul:

```text
MEET THE TEAM

Three people.
Three perspectives.
One team.
```

Layout desktop:

```text
┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│              │ │              │ │              │
│    PHOTO     │ │    PHOTO     │ │    PHOTO     │
│              │ │              │ │              │
├──────────────┤ ├──────────────┤ ├──────────────┤
│ BHADRIKO     │ │ ALFAN        │ │ IQBAL        │
│ Role         │ │ Role         │ │ Role         │
│              │ │              │ │              │
│ Short bio    │ │ Short bio    │ │ Short bio    │
│              │ │              │ │              │
│ View Profile │ │ View Profile │ │ View Profile │
└──────────────┘ └──────────────┘ └──────────────┘
```

## 10.1 Card Style

```text
Background:
#151619

Border:
1px solid rgba(255,255,255,0.08)

Border Radius:
24px
```

## 10.2 Hover State

Saat card di-hover:

- Card naik sedikit
- Border berubah ke accent
- Foto sedikit zoom
- Button berubah
- Shadow/glow tipis

Contoh transform:

```text
translateY(-4px)
```

Jangan menggunakan efek hover berlebihan.

---

# 11. PERSONAL PROFILE / CV

Requirement perusahaan meminta detail CV setiap anggota.

Setiap anggota harus memiliki:

```text
ABOUT
EDUCATION
EXPERIENCE
ORGANIZATION
PROJECTS
SKILLS
DOCUMENTS
CONTACT
```

Contoh:

## BHADRIKO

```text
BHADRIKO
Project / Organization / Design

About Me
────────

...

Education
─────────

2024 - Present
University ...

Experience
──────────

2025
Organization ...

2026
iCraftDS Internship

Skills
──────

[Project Management]
[Communication]
[UI/UX]
[Leadership]
...
```

Kemudian:

```text
[ Download CV ]
[ View Documents ]
```

Hal yang sama diterapkan pada Alfan dan Iqbal.

---

# 12. EXPERIENCE & EDUCATION

Gunakan timeline agar informasi CV lebih visual.

Contoh:

```text
EXPERIENCE

2026
│
├── iCraftDS Internship
│   Team Portfolio Project
│
2025
│
├── Organization / Project
│
2024
│
└── University
```

Desktop dapat menggunakan timeline horizontal.

Mobile menggunakan timeline vertical.

Informasi minimal:

- Tahun/periode
- Nama organisasi/perusahaan/proyek
- Jabatan/peran
- Deskripsi singkat
- Kontribusi utama

---

# 13. SKILLS

Hindari progress bar seperti:

```text
HTML █████████ 90%
CSS  ████████  80%
```

Format yang lebih modern adalah badge atau grouping.

Contoh:

```text
TECHNICAL

HTML • CSS • JavaScript • Tailwind


PROFESSIONAL

Communication • Leadership • Teamwork


TOOLS

Git • Figma • VS Code
```

Atau badge:

```text
┌─────────────┐
│ HTML        │
└─────────────┘

┌─────────────┐
│ CSS         │
└─────────────┘

┌─────────────┐
│ JavaScript  │
└─────────────┘
```

Skills harus sesuai kemampuan nyata masing-masing anggota.

Jangan memasukkan skill hanya agar terlihat banyak.

---

# 14. PROJECT SECTION

Section project membuat website terasa sebagai portfolio, bukan sekadar CV online.

Judul:

```text
SELECTED PROJECTS

A collection of things we've built,
designed, and worked on.
```

Layout:

```text
┌──────────────────────────────────────────┐
│                                          │
│            PROJECT IMAGE                │
│                                          │
├──────────────────────────────────────────┤
│ PROJECT NAME                             │
│                                          │
│ Short description...                     │
│                                          │
│ [UI/UX] [Web] [Development]              │
│                                          │
│ View Project ↗                           │
└──────────────────────────────────────────┘
```

Gunakan 3-6 project jika memang tersedia.

Jika anggota belum memiliki banyak project, jangan memaksakan jumlah project.

Lebih baik sedikit tetapi benar-benar relevan.

---

# 15. DOCUMENTS

Requirement perusahaan secara eksplisit menyebut kelengkapan dokumen.

Buat section:

```text
DOCUMENTS

Supporting documents
and professional profiles.
```

Card:

```text
┌─────────────────────────────┐
│ CV                          │
│ Curriculum Vitae            │
│                             │
│ PDF • 2026                  │
│                             │
│ Download ↗                  │
└─────────────────────────────┘
```

Dokumen dapat berupa:

- CV
- Certificate
- Portfolio
- Supporting document

Jangan upload dokumen yang mengandung data pribadi sensitif yang tidak diperlukan untuk penilaian.

---

# 16. CTA SECTION

Sebelum Contact, buat section CTA yang kuat.

Contoh:

```text
LET'S BUILD
SOMETHING
TOGETHER.

Have a project,
idea, or opportunity?

[ Get In Touch ↗ ]
```

CTA menjadi transisi dari portfolio ke contact.

Background dapat menggunakan accent gradient secara subtle.

---

# 17. CONTACT SECTION

Contact merupakan section terakhir sebelum footer.

Gunakan dua kolom.

```text
CONTACT

Let's connect.

Whether you want to talk about a project,
collaboration, or simply say hello,
we'd love to hear from you.


┌──────────────────────┐
│ Email                │
│ team@email.com       │
│                      │
│ Instagram            │
│ @teamname            │
│                      │
│ LinkedIn             │
│ Team Name            │
└──────────────────────┘
```

Sisi kanan:

```text
┌──────────────────────────────┐
│                              │
│ Name                         │
│ ┌──────────────────────────┐ │
│ │                          │ │
│ └──────────────────────────┘ │
│                              │
│ Email                        │
│ ┌──────────────────────────┐ │
│ │                          │ │
│ └──────────────────────────┘ │
│                              │
│ Message                      │
│ ┌──────────────────────────┐ │
│ │                          │ │
│ │                          │ │
│ └──────────────────────────┘ │
│                              │
│ [ Send Message ↗ ]           │
└──────────────────────────────┘
```

## 17.1 Catatan Contact Form

Jika tidak ada backend, jangan membuat form yang seolah-olah benar-benar mengirim data.

Alternatif:

```text
[ Email Us ]
[ WhatsApp ]
[ LinkedIn ]
[ Instagram ]
```

Jika ingin menggunakan form, gunakan layanan email/form pihak ketiga yang sesuai kebutuhan.

---

# 18. FOOTER

Footer harus minimal.

```text
────────────────────────────────────────────

TEAM NAME

Building, learning, and growing together.

[Instagram] [LinkedIn] [GitHub]

© 2026 Team Name
Built for iCraftDS Internship

────────────────────────────────────────────
```

Gunakan typography yang lebih kecil.

Jangan menambahkan terlalu banyak informasi.

---

# 19. RESPONSIVE DESIGN

Responsive adalah requirement wajib.

## 19.1 Desktop

```text
Navbar
Hero 2 columns
Team 3 columns
Project 2 columns
Experience 2 columns / timeline
Contact 2 columns
```

## 19.2 Tablet

```text
Hero 1-2 columns
Team 2 columns
Project 2 columns
Contact 1-2 columns
```

## 19.3 Mobile

```text
Navbar hamburger

Hero
  ↓
About
  ↓
Card
  ↓
Card
  ↓
Card
  ↓
Expertise
  ↓
Experience
  ↓
Projects
  ↓
Documents
  ↓
CTA
  ↓
Contact
  ↓
Footer
```

Mobile jangan hanya mengecilkan desktop.

Layout harus dirancang ulang agar nyaman disentuh dan dibaca.

---

# 20. SPACING SYSTEM

Gunakan spacing yang konsisten.

Rekomendasi:

```text
Section Padding:
Desktop: 96px top/bottom
Mobile: 64px top/bottom

Container:
max-width: 1200px

Horizontal Padding:
Desktop: 32px
Mobile: 20px

Card Gap:
24px

Element Gap:
16px
```

Jangan setiap section menggunakan jarak yang berbeda tanpa alasan.

---

# 21. BORDER RADIUS

Gunakan hierarchy.

```text
Button:
12px

Small Card:
16px

Large Card:
20-24px

Hero Container:
24-32px
```

Hindari membuat semua elemen `rounded-full`.

---

# 22. BUTTON SYSTEM

## Primary Button

```text
Background:
#7C5CFC

Text:
#FFFFFF

Radius:
12px

Padding:
12px 20px
```

Hover:

```text
Primary → #6847F5
```

## Secondary Button

```text
Background:
transparent

Border:
rgba(255,255,255,0.1)

Text:
#FFFFFF
```

Hover:

```text
Background → Surface
Border → Accent
```

---

# 23. ICON SYSTEM

Gunakan satu icon library agar konsisten.

Rekomendasi:

**Lucide Icons**

Jangan mencampurkan banyak icon library dalam satu website.

Hindari kombinasi seperti:

```text
Font Awesome
Bootstrap Icons
Material Icons
Lucide
```

dalam satu interface.

Satu sistem icon lebih konsisten dan mudah dipelihara.

---

# 24. ANIMATION SYSTEM

Animation harus subtle.

## 24.1 On Load

Hero:

```text
opacity: 0 → 1
translateY: 20px → 0
```

## 24.2 Hover

Card:

```text
translateY(-4px)
```

## 24.3 Scroll Reveal

Section dapat muncul secara perlahan ketika masuk viewport.

Durasi:

```text
300-500ms
```

Hindari:

- Text berputar
- Card terbang
- Parallax berlebihan
- Cursor custom yang tidak diperlukan
- Loading screen terlalu lama
- Animasi pada setiap elemen

Prinsip:

> Modern bukan berarti banyak animasi.

---

# 25. STRUKTUR FINAL HALAMAN

Urutan final:

```text
01  NAVBAR
        ↓
02  HERO
        ↓
03  ABOUT TEAM
        ↓
04  TEAM MEMBERS
        ↓
05  EXPERTISE / SKILLS
        ↓
06  SELECTED PROJECTS
        ↓
07  EXPERIENCE
        ↓
08  EDUCATION
        ↓
09  DOCUMENTS
        ↓
10  CTA
        ↓
11  CONTACT
        ↓
12  FOOTER
```

Navigation:

```text
Home
About
Team
Projects
Experience
Contact
```

---

# 26. ARSITEKTUR WEBSITE

Jangan menjadikan tiga halaman CV sebagai pengalaman utama.

Gunakan satu landing page tim sebagai halaman utama.

Struktur:

```text
TEAM WEBSITE
       │
       ├── Bhadriko Profile
       ├── Alfan Profile
       └── Iqbal Profile
```

Card anggota dapat membuka halaman detail masing-masing.

Contoh:

```text
Bhadriko
View Profile →
```

membuka:

```text
/members/bhadriko.html
```

Dengan demikian requirement terpenuhi dalam dua level:

```text
Landing Page Tim
        +
CV Individu
```

---

# 27. STRUKTUR FILE PROJECT

Rekomendasi:

```text
team-portfolio/
│
├── index.html
│
├── members/
│   ├── bhadriko.html
│   ├── alfan.html
│   └── iqbal.html
│
├── src/
│   └── input.css
│
├── dist/
│   └── output.css
│
├── assets/
│   ├── images/
│   │   ├── team/
│   │   ├── bhadriko/
│   │   ├── alfan/
│   │   └── iqbal/
│   │
│   ├── documents/
│   │   ├── bhadriko-cv.pdf
│   │   ├── alfan-cv.pdf
│   │   └── iqbal-cv.pdf
│   │
│   └── icons/
│
├── js/
│   └── main.js
│
├── package.json
└── README.md
```

---

# 28. TEKNOLOGI YANG DIGUNAKAN

## Frontend

```text
HTML5
Tailwind CSS v4
JavaScript
```

## Styling

```text
Tailwind CSS
```

## Icons

```text
Lucide Icons
```

## Version Control

```text
Git
GitHub
```

## Hosting

Bisa menggunakan layanan hosting statis yang mendukung project HTML/CSS/JS.

---

# 29. TAILWIND CSS INSTALLATION

Gunakan Tailwind secara lokal menggunakan CLI.

Jangan menjadikan CDN sebagai metode utama untuk project final.

## 29.1 Inisialisasi

```bash
npm init -y
```

Install Tailwind:

```bash
npm install tailwindcss @tailwindcss/cli
```

## 29.2 Input CSS

File:

```text
src/input.css
```

Isi:

```css
@import "tailwindcss";
```

## 29.3 Package Script

Tambahkan script:

```json
{
  "scripts": {
    "dev": "npx @tailwindcss/cli -i ./src/input.css -o ./dist/output.css --watch"
  }
}
```

## 29.4 Jalankan Development

```bash
npm run dev
```

## 29.5 Hubungkan ke HTML

```html
<link rel="stylesheet" href="./dist/output.css">
```

Untuk halaman dalam folder `members`, path harus disesuaikan:

```html
<link rel="stylesheet" href="../dist/output.css">
```

---

# 30. KENAPA HTML + TAILWIND?

Project ini tidak membutuhkan framework frontend berat.

Tidak ada kebutuhan wajib untuk:

- Authentication
- Database
- Dashboard
- State management kompleks
- API
- Realtime system
- CMS
- Routing kompleks

Karena itu:

> **HTML + Tailwind + JavaScript seperlunya adalah pilihan yang aman dan efisien.**

Keuntungan:

- Setup sederhana
- Mudah dipahami seluruh anggota tim
- Mudah dikerjakan bersama menggunakan Git
- Tidak membutuhkan React/Next.js
- Tetap menggunakan workflow modern
- Mudah di-hosting sebagai static website
- Risiko teknis lebih kecil menjelang deadline

---

# 31. KAPAN MENGGUNAKAN FRAMEWORK?

Framework seperti React atau Next.js baru layak dipilih jika:

- Semua anggota tim sudah nyaman menggunakannya
- Ada kebutuhan component system yang kompleks
- Ada interaksi/state yang cukup banyak
- Ingin sekalian belajar framework sebagai tujuan project

Jika kemampuan framework anggota belum merata dan deadline dekat, jangan menambah kompleksitas tanpa kebutuhan.

Prioritas:

```text
DESIGN BAGUS
      ↓
FUNCTIONAL
      ↓
RESPONSIVE
      ↓
CONTENT LENGKAP
      ↓
DEPLOYMENT
      ↓
POLISH
```

Bukan:

```text
FRAMEWORK CANGGIH
      ↓
SETUP RIBET
      ↓
DEBUGGING
      ↓
DESIGN TERBENGKALAI
```

---

# 32. KONTEN CV SETIAP ANGGOTA

Setiap anggota minimal memiliki:

## Data Diri

```text
Nama
Role
Email
Social Media
Lokasi umum jika diperlukan
```

Hindari menampilkan data pribadi yang tidak diperlukan.

## Pendidikan

```text
Institusi
Program Studi
Periode
Deskripsi singkat
```

## Organisasi

```text
Nama organisasi
Jabatan
Periode
Kontribusi
```

## Project

```text
Nama project
Role
Periode
Deskripsi
Tools
Output
```

## Skills

```text
Technical Skills
Professional Skills
Tools
```

## Documents

```text
CV
Certificate
Supporting Documents
```

---

# 33. STANDAR COPYWRITING

Gunakan bahasa profesional tetapi tetap natural.

Hindari:

```text
Kami adalah kelompok yang sangat solid
dan mempunyai banyak sekali pengalaman...
```

Lebih baik:

```text
We are a team of three individuals with different
strengths, working together to learn, build, and
create meaningful digital experiences.
```

Gunakan kalimat pendek.

Jangan membuat website penuh paragraf.

---

# 34. FOTO DAN ASSET

Gunakan foto dengan style yang konsisten.

Idealnya:

- Background serupa
- Lighting serupa
- Rasio foto serupa
- Crop serupa
- Resolusi cukup tinggi

Jangan menggunakan:

```text
Bhadriko → selfie
Alfan → foto formal
Iqbal → foto dari acara
```

jika ingin hasil visual yang konsisten.

Lebih baik ketiga anggota memiliki sesi foto yang sama atau setidaknya menggunakan treatment visual yang sama.

---

# 35. QUALITY CONTROL

Sebelum deployment, cek:

## Visual

- [ ] Semua font konsisten
- [ ] Semua warna konsisten
- [ ] Semua card memiliki radius konsisten
- [ ] Semua spacing konsisten
- [ ] Tidak ada section terlalu padat
- [ ] Foto anggota memiliki ukuran konsisten

## Content

- [ ] Nama tim sudah final
- [ ] Profil Bhadriko lengkap
- [ ] Profil Alfan lengkap
- [ ] Profil Iqbal lengkap
- [ ] Pendidikan tersedia
- [ ] Pengalaman tersedia
- [ ] Organisasi/proyek tersedia
- [ ] Skills tersedia
- [ ] CV tersedia
- [ ] Dokumen pendukung tersedia jika diperlukan

## Technical

- [ ] Semua link berfungsi
- [ ] Semua gambar tampil
- [ ] PDF dapat dibuka
- [ ] Tidak ada broken path
- [ ] Mobile responsive
- [ ] Tablet responsive
- [ ] Desktop responsive
- [ ] Tidak ada console error
- [ ] Git repository rapi
- [ ] Website sudah live

## Deployment

- [ ] URL publik dapat diakses
- [ ] HTTPS aktif
- [ ] Semua anggota dapat membuka website
- [ ] Link yang dikumpulkan adalah URL website live

---

# 36. RESPONSIBILITY PEMBAGIAN KERJA

Rekomendasi pembagian:

## Bhadriko

Fokus:

- Project structure
- Design system
- Landing page
- Navbar
- Hero
- About
- Integration
- Final quality control

## Alfan

Fokus:

- Profile page
- Education
- Experience
- Organization
- Skills
- CV section

## Iqbal

Fokus:

- Projects
- Documents
- Contact
- Footer
- Responsive refinement

Semua anggota tetap wajib memberikan konten CV masing-masing.

Pembagian ini bukan berarti anggota hanya boleh menyentuh bagian tersebut. Tujuannya agar ownership jelas.

---

# 37. GIT WORKFLOW

Gunakan repository bersama.

Branch utama:

```text
main
```

Branch pekerjaan:

```text
feature/landing-page
feature/bhadriko-profile
feature/alfan-profile
feature/iqbal-profile
feature/projects
feature/contact
```

Workflow:

```text
Create Branch
      ↓
Work
      ↓
Commit
      ↓
Push
      ↓
Pull Request
      ↓
Review
      ↓
Merge
```

Commit sebaiknya jelas.

Contoh:

```text
feat: add team hero section
feat: add bhadriko profile
style: improve team cards
fix: mobile navbar
fix: broken CV links
```

---

# 38. PRINCIPLE DESAIN UTAMA

Pegang prinsip berikut selama pengerjaan:

### 1. Less, but better

Lebih baik 5 elemen yang bagus daripada 15 elemen yang tidak perlu.

### 2. Consistency beats complexity

Konsistensi warna, spacing, typography, dan component lebih penting daripada efek visual rumit.

### 3. Content first

Jangan membuat desain bagus tetapi informasi CV tidak lengkap.

### 4. Mobile matters

Website harus nyaman dibuka lewat smartphone.

### 5. Don't fake functionality

Jangan membuat fitur seolah-olah bekerja jika sebenarnya tidak ada backend.

### 6. Don't over-engineer

Jangan menggunakan framework hanya karena terlihat lebih profesional.

### 7. Make it feel like a real portfolio

Hasil akhir harus terasa sebagai portfolio profesional yang kebetulan dibuat dalam program magang, bukan sekadar tugas yang harus dikumpulkan.

---

# 39. FINAL VISUAL FLOW

```text
┌──────────────────────────────────────────────┐
│                    NAVBAR                    │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                    HERO                      │
│                                              │
│        We Build. We Learn. We Create.       │
│                                              │
│              [Meet The Team]                 │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                 ABOUT TEAM                   │
│                                              │
│  Who We Are          Team Philosophy         │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                 MEET THE TEAM                │
│                                              │
│   [Bhadriko]     [Alfan]      [Iqbal]       │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                OUR EXPERTISE                 │
│                                              │
│  Technical • Professional • Tools            │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│              SELECTED PROJECTS               │
│                                              │
│       [Project]       [Project]              │
│       [Project]       [Project]              │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│            EXPERIENCE & EDUCATION            │
│                                              │
│                  Timeline                    │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                  DOCUMENTS                   │
│                                              │
│        [CV]       [Certificate]              │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                     CTA                      │
│                                              │
│        LET'S BUILD SOMETHING TOGETHER       │
│                                              │
│               [Get In Touch]                 │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                   CONTACT                    │
│                                              │
│  Contact Info           Contact Form         │
└──────────────────────────────────────────────┘
                      ↓
┌──────────────────────────────────────────────┐
│                   FOOTER                     │
│                                              │
│  Team Name • Social • © 2026                 │
└──────────────────────────────────────────────┘
```

---

# 40. TARGET AKHIR

Website final harus memenuhi empat hal utama:

```text
          PROFESSIONAL
               │
               ▼
        ┌──────────────┐
        │              │
        │ TEAM WEBSITE │
        │              │
        └──────────────┘
          ▲     ▲     ▲
          │     │     │
      CONTENT DESIGN TECHNICAL
          │     │     │
          ▼     ▼     ▼
        Lengkap Bagus  Solid
```

Output yang diharapkan:

1. Landing page tim yang profesional.
2. Profil tiga anggota yang jelas.
3. CV individu yang lengkap.
4. Portfolio/project yang relevan.
5. Dokumen pendukung yang dapat diakses.
6. Responsive pada desktop, tablet, dan mobile.
7. Website menggunakan coding, bukan website builder.
8. Website live dan dapat diakses publik.
9. Repository Git rapi.
10. Seluruh anggota mengumpulkan URL website yang sama melalui portal iCraftDS.

---

# 41. URUTAN PENGERJAAN YANG DIREKOMENDASIKAN

Jangan langsung mengerjakan animasi atau detail kecil.

Urutan:

```text
01. Tentukan nama tim
        ↓
02. Tentukan identitas visual
        ↓
03. Kumpulkan seluruh data CV
        ↓
04. Kumpulkan foto & dokumen
        ↓
05. Setup Git + Tailwind
        ↓
06. Buat global layout
        ↓
07. Buat Navbar
        ↓
08. Buat Hero
        ↓
09. Buat About
        ↓
10. Buat Team Cards
        ↓
11. Buat Profile/CV
        ↓
12. Buat Projects
        ↓
13. Buat Documents
        ↓
14. Buat CTA
        ↓
15. Buat Contact
        ↓
16. Buat Footer
        ↓
17. Responsive
        ↓
18. Animation
        ↓
19. Quality Control
        ↓
20. Deploy
        ↓
21. Test URL
        ↓
22. Submit
```

Prioritas utama:

> **Content → Structure → Design → Responsive → Interaction → Polish**

Jangan dibalik.
