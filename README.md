# Day 1 – Building with AI, Managing Change with GitHub

**Nama Lengkap:** Rizki Fauzan
**Kelompok:** Expedition 33

## Deskripsi Repository

Repository ini berisi dokumentasi kegiatan Day 1 workshop **"Building with AI, Managing Change with GitHub"** yang disampaikan oleh Nugi Farhan (Senior Product Designer). Isinya adalah rangkuman materi, pengetahuan baru yang saya dapat, dan pendapat pribadi saya tentang Day 1.

## Tujuan Repository

- Menyimpan dan mempublikasikan dokumentasi workshop secara daring melalui GitHub.
- Melatih pembuatan dan pengelolaan repository dengan visibilitas Public.
- Membiasakan diri mencatat materi dan kegiatan secara rapi dan terstruktur.
- Berlatih memakai `README.md` sebagai dokumentasi utama repository.

## Kegiatan Workshop yang Didokumentasikan

Day 1 membahas dua topik utama:

1. **Membuat dan mengembangkan** dengan bantuan AI (Prompt Engineering).
2. **Manajemen perubahan dan kolaborasi** dengan Git dan GitHub.

Dokumentasi lengkapnya ada di bagian berikut: rangkuman materi, poin penting, dan pendapat pribadi.

---

## 1. Rangkuman Materi

### A. Prompt Engineering

- **Prompt** adalah instruksi atau masukan yang diberikan kepada model AI untuk mendapatkan hasil tertentu. Bentuknya bisa berupa pertanyaan sederhana, kata kunci, instruksi yang rumit, atau potongan kode.
- **Prompt engineering** adalah cara merancang instruksi agar AI memberikan jawaban yang tepat, relevan, dan layak digunakan.
- **Konteks adalah kunci.** Prompt singkat seperti "Create student task planner" menghasilkan output yang umum. Prompt yang menjelaskan tujuan, kebutuhan, dan batasan menghasilkan output yang jauh lebih sesuai.
- **Struktur prompt yang baik** terdiri dari:
  - **Role**: peran yang diberikan kepada AI.
  - **Task**: tujuan yang ingin dicapai.
  - **Context**: kebutuhan (requirements) dan batasan (constraints).
  - **Format**: bentuk output yang diminta.
- **Taktik menulis prompt:** memakai kata kerja aksi, menentukan panjang dan format output, menentukan target audiens, menyertakan fakta dan data yang relevan, merujuk sumber atau dokumen tertentu, dan mendefinisikan istilah kunci.
- **Keuntungan prompt engineering:** meningkatkan performa model AI, mengurangi bias dan respons yang offensive, meningkatkan kontrol dan *predictability*, serta memberikan pengalaman penggunaan yang lebih baik.

### B. Git dan GitHub

- **Git** adalah *distributed version control system* (DVCS) yang melacak siapa, kapan, dan apa yang berubah pada suatu file. Git dibuat oleh Linus Torvalds pada 2005 dan bekerja secara lokal.
- **GitHub** adalah platform berbasis web untuk menyimpan repository Git secara online dan mendukung kolaborasi.
- **Git workflow** melewati tiga area:
  - **Working directory**: salinan satu versi proyek yang sedang dikerjakan.
  - **Staging area (index)**: tempat menampung perubahan yang akan masuk ke commit berikutnya.
  - **Git directory (repository)**: tempat Git menyimpan metadata dan object database proyek. Bagian inilah yang disalin saat melakukan `clone`.

**Perintah dasar Git dan GitHub**

| Perintah | Fungsi |
|---|---|
| `git init` | Memulai repository baru |
| `git clone "url"` | Menyalin repository dari GitHub |
| `git add .` / `git add -A` | Memindahkan file ke staging area |
| `git commit -m "message"` | Menyimpan perubahan ke repository |
| `git remote add <name> <url>` | Menghubungkan repository lokal ke remote |
| `git push origin main` | Mengirim branch saat ini ke remote |
| `git pull origin main` | Mengambil perubahan dari remote lalu menggabungkannya ke branch saat ini |

**Setup yang dibahas**

1. Install Git dan cek dengan `git --version`.
2. Atur identitas dengan `git config --global user.name` dan `git config --global user.email`, lalu cek dengan `git config --global --list`.
3. Install VS Code dan perintah `code` di PATH.
4. Buat SSH key dengan `ssh-keygen -t ed25519 -C "email@domain.com"`, daftarkan public key ke GitHub, lalu verifikasi koneksi dengan `ssh -T git@github.com`.

---

## 2. Poin Penting dan Pengetahuan Baru

- Prompt yang spesifik (Role, Task, Context, Format) menghasilkan output AI yang jauh lebih baik daripada prompt singkat tanpa konteks.
- Prompt yang baik juga bisa meminta AI memverifikasi hasilnya dan tidak langsung mengklaim bahwa hasilnya sudah benar.
- Git dan GitHub adalah dua hal yang berbeda: Git adalah alat version control lokal, GitHub adalah platform online untuk menyimpan repository dan berkolaborasi.
- Perubahan di Git tidak langsung masuk ke repository. Perubahan harus dipindahkan dulu ke staging area (`git add`), baru disimpan lewat `git commit`.
- Alur dasar mengirim pekerjaan ke GitHub: `git init` → `git add` → `git commit` → `git remote add` → `git push`.
- SSH key (Ed25519) membuat koneksi ke GitHub lebih aman dan praktis karena tidak perlu memasukkan kredensial berulang kali.

---

## 3. Pendapat Pribadi tentang Day 1 Proyek Workshop

Menurut saya, Day 1 memberi fondasi yang bagus karena menggabungkan dua hal yang saling melengkapi: cara berkomunikasi dengan AI lewat prompt yang jelas, dan cara mengelola hasil kerja lewat Git dan GitHub. Contoh perbandingan prompt tanpa konteks dan dengan konteks membuat saya mudah memahami kenapa detail dalam prompt sangat memengaruhi kualitas hasil AI.

Bagian Git dan GitHub juga berguna karena penjelasan tiga area (working directory, staging area, repository) membantu saya memahami apa yang sebenarnya terjadi saat menjalankan `git add` dan `git commit`. Bagian yang paling menantang adalah setup SSH key karena langkahnya banyak dan harus teliti, tetapi hasilnya terasa sepadan karena koneksi ke GitHub jadi lebih aman.

Ke depannya, saya ingin lebih sering berlatih membuat commit kecil yang rapi dan memakai prompt terstruktur setiap kali meminta bantuan AI. Repository ini adalah langkah pertama saya untuk membiasakan mendokumentasikan proses belajar di GitHub.
