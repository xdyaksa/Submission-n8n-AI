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
| **P2** | Webhook Triggers & Data Transformation | - | - | Belum Selesai |
| **P3** | Advanced API Integration & Error Handling | - | - | Belum Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | - | - | Belum Selesai |
| **P5** | Capstone Final Project: Smart Autonomous AI | - | - | Belum Selesai |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
Tuliskan penjelasan singkat mengenai alur kerja yang telah kamu bangun:
- **Tujuan Workflow**: Membangun alur kerja otomasi n8n berbasis Webhook untuk menerima HTTP request (POST), memproses data JSON, serta mengembalikan respons secara real-time ke client pengirim.
- **Node Kunci yang Digunakan**: Webhook Node, Edit Fields (Set) Node, dan Respond to Webhook Node.
- **Logika Alur Kerja**:
  1. **Webhook Node** menerima data JSON (`Nama` dan `Pesan`) yang dikirim melalui metode POST dari Hoppscotch.
  2. Data diproses pada **Edit Fields Node** menggunakan ekspresi dinamis `{{ $json.body.Nama }}` dan `{{ $json.body.Pesan }}` untuk menyusun teks balasan.
  3. **Respond to Webhook Node** mengembalikan pesan balasan tersebut ke Hoppscotch sebagai respons HTTP sukses.

---

## 🌟 Refleksi & Kesan Belajar
Pengalaman belajar di Pertemuan 1 n8n Study Jam GDGoC Universitas Widyatama sangat seru dan bermanfaat, apalagi bagi saya yang masih baru dengan hal seperti n8n.
