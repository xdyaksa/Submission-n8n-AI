# Submission n8n Study Jam - GDGoC Universitas Widyatama

## 👤 Informasi Peserta
- **Nama Lengkap**: Abiyyu Amanullah
- **NIM**: 1257050052
- **Program Studi**: Teknik Informatika
- **Username GitHub**: [@abiyyumnllh](https://github.com/abiyyumnllh)
- **URL Repositori Tugas**: [https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam)

---

## 📊 Matriks Progres Tugas (P1 - P5)

| Pertemuan | Topik Tugas | Tautan File Workflow (.json) | Bukti Eksekusi (Screenshot) | Status |
| :---: | :--- | :---: | :---: | :---: |
| **P1** | Pengenalan n8n & Workflow Automation Dasar | [P1_Abiyyu_Amanullah.json](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-01/P1_Abiyyu_Amanullah.json) | [P1_Abiyyu_Amanullah.png](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-01/P1_Abiyyu_Amanullah.png) | Selesai |
| **P2** | Webhook Triggers & Data Transformation | [P2_Abiyyu_Amanullah.json](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-02/P2_Abiyyu_Amanullah.json) | [P2_Abiyyu_Amanullah.png](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-02/P2_Abiyyu_Amanullah.png) | Selesai |
| **P3** | Advanced API Integration & Error Handling | - | - | Belum Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | - | - | Belum Selesai |
| **P5** | Capstone Final Project: Smart Autonomous AI | - | - | Belum Selesai |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)

### Pertemuan 1: Pengenalan n8n & Workflow Automation Dasar
- **Tujuan Workflow**: Membangun alur kerja otomasi n8n berbasis Webhook untuk menerima HTTP request (POST), memproses data JSON, serta mengembalikan respons secara real-time ke client pengirim.
- **Node Kunci yang Digunakan**: Webhook Node, Edit Fields (Set) Node, dan Respond to Webhook Node.
- **Logika Alur Kerja**:
  1. **Webhook Node** menerima data JSON (`Nama` dan `Pesan`) yang dikirim melalui metode POST dari Hoppscotch.
  2. Data diproses pada **Edit Fields Node** menggunakan ekspresi dinamis `{{ $json.body.Nama }}` dan `{{ $json.body.Pesan }}` untuk menyusun teks balasan.
  3. **Respond to Webhook Node** mengembalikan pesan balasan tersebut ke Hoppscotch sebagai respons HTTP sukses.

### Pertemuan 2: Webhook Triggers & Data Transformation (AI Persona Generator)
- **Tujuan Workflow**: Menyambungkan input data dari Webhook ke model AI Gemini supaya workflow bisa membalas request dari Hoppscotch secara otomatis dengan komentar yang sesuai input.
- **Node Kunci yang Digunakan**: Webhook, Edit Fields, Google Gemini (`Message a model`), dan Respond to Webhook.
- **Alur Kerja**:
  1. **Webhook** menangkap data JSON berisi `Nama` dan `Hobi` yang dikirim lewat metode POST di Hoppscotch.
  2. **Edit Fields** menggabungkan data tersebut memakai ekspresi `{{ $json.body.Nama }}` dan `{{ $json.body.Hobi }}` menjadi satu kalimat *prompt* utuh.
  3. **Message a model (Gemini 3 Flash Preview)** membaca *prompt* tadi dan membuatkan komentar sesuai instruksi.
  4. **Respond to Webhook** meneruskan hasil teks dari `{{ $json.content.parts[0].text }}` kembali sebagai balasan di Hoppscotch.

---

## 🌟 Refleksi & Kesan Belajar
- **Pertemuan 1**: Pengalaman belajar di Pertemuan 1 n8n Study Jam GDGoC Universitas Widyatama sangat seru dan bermanfaat, apalagi bagi saya yang baru tahu mengenai n8n.
- **Pertemuan 2**: Materi pertemuan kedua ini bikin makin kebayang gimana caranya ngolah data JSON dari request luar lalu langsung disambungin ke AI. Bagian paling terpakai saat belajar pakai ekspresi dinamis di Edit Fields sama ngatur *Retry On Fail* biar aman kalau kena limit API.
