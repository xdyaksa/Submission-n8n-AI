# Submission n8n Study Jam - GDGoC Universitas Widyatama

## 👤 Informasi Peserta
- **Nama Lengkap**: Sulthan Faruq Hasan
- **NIM**: 10125009
- **Program Studi**: Teknik Informatika
- **Username GitHub**: [@sfhfrq](https://github.com/sfhfrq)
- **URL Repositori Tugas**: [https://github.com/sfhfrq/GDGoC-n8n-StudyJam](https://github.com/sfhfrq/GDGoC-n8n-StudyJam)

---

## 📊 Matriks Progres Tugas (P1 - P5)

| Pertemuan | Topik Tugas | Tautan File Workflow (.json) | Bukti Eksekusi (Screenshot) | Status |
| :---: | :--- | :---: | :---: | :---: |
| **P1** | Pengenalan n8n & Workflow Automation Dasar | [P1_Sulthan_Faruq_Hasan.json](https://github.com/sfhfrq/GDGoC-n8n-StudyJam/blob/main/Pertemuan-1/P1_Sulthan_Faruq_Hasan.json) | [P1_Sulthan_Faruq_Hasan.png](https://github.com/sfhfrq/GDGoC-n8n-StudyJam/blob/main/Pertemuan-1/P1_Sulthan_Faruq_Hasan.png) | Selesai |
| **P2** | Webhook Triggers & Data Transformation | - | - | Belum Selesai |
| **P3** | Advanced API Integration & Error Handling | - | - | Belum Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | - | - | Belum Selesai |
| **P5** | Capstone Final Project: Smart Autonomous AI | - | - | Belum Selesai |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
- **Tujuan Workflow**: Menerima data input (`nama` dan `pesan`) melalui HTTP POST Webhook pada n8n, memformat pesan balasan secara dinamis menggunakan ekspresi n8n, dan mengembalikan respons JSON otomatis kepada pengirim request.
- **Node Kunci yang Digunakan**: `Webhook` (HTTP Method: POST, Path: `p1`), `Edit Fields` (`n8n-nodes-base.set`), dan `Respond to Webhook` (`n8n-nodes-base.respondToWebhook`).
- **Logika Alur Kerja**:
  1. Node **Webhook** menerima request `POST` pada path `/p1` dengan mode respons `responseNode`.
  2. Data payload (`$json.body.nama` dan `$json.body.pesan`) diteruskan ke node **Edit Fields** untuk membentuk objek respons dengan field `status: "sukses"` dan `messege: "TerimaKasih {{ $json.body.nama }} Pesan Kamu {{ $json.body.pesan }}"`.
  3. Node **Respond to Webhook** mengirimkan output JSON yang telah diformat kembali ke pemanggil webhook.

---

## 📝 Refleksi & Kesan Belajar
Melalui Pertemuan 1 n8n AI & Automation Study Jam bersama GDGoC Universitas Widyatama, saya mempelajari konsep dasar workflow automation menggunakan n8n, mulai dari cara membuat endpoint penerima data dengan node Webhook, memetakan dan memanipulasi variabel JSON secara dinamis di node Edit Fields, hingga mengembalikan hasil eksekusi secara langsung melalui Respond to Webhook.
