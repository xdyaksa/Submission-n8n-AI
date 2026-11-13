# Submission n8n Study Jam - GDGoC Universitas Widyatama

## 👤 Informasi Peserta
- **Nama Lengkap**: Bagas Julian Hadgani Suty Prakoso
- **NIM**: 240611054
- **Program Studi**: Teknik Informatika
- **Username GitHub**: [@bagasjuliannn](https://github.com/bagasjuliannn)
- **URL Repositori Tugas**: [https://github.com/bagasjuliannn/GDGoC-n8n-StudyJam](https://github.com/bagasjuliannn/GDGoC-n8n-StudyJam)

---

## 📊 Matriks Progres Tugas (P1 - P5)

| Pertemuan | Topik Tugas | Tautan File Workflow (.json) | Bukti Eksekusi (Screenshot) | Status |
| :--- | :--- | :--- | :--- | :--- |
| **P1** | Pengenalan n8n & Workflow Automation Dasar | [P1_Bagas.json](https://github.com/bagasjuliannn/GDGoC-n8n-StudyJam/blob/main/P1_Bagas.json) | [P1_Bagas.png](https://github.com/bagasjuliannn/GDGoC-n8n-StudyJam/blob/main/P1_Bagas.png) | Selesai |
| **P2** | Webhook Triggers & Data Transformation | [P2_Bagas.json](https://github.com/bagasjuliannn/GDGoC-n8n-StudyJam/blob/main/P2_Bagas.json) | [P2_Bagas.png](https://github.com/bagasjuliannn/GDGoC-n8n-StudyJam/blob/main/P2_Bagas.png) | Selesai |
| **P3** | Advanced API Integration & Error Handling | - | - | Belum |
| **P4** | AI Agent & LLM Chain Automation di n8n | - | - | Belum |
| **P5** | Capstone Final Project: Smart Autonomous AI | - | - | Belum |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
- **Tujuan Workflow**: Menerima request POST dari Webhook, melakukan transformasi/pemetaan data masukan melalui Edit Fields, memproses prompt menggunakan AI Model (Gemini), dan mengembalikan respons teks secara otomatis ke client.
- **Node Kunci yang Digunakan**: Webhook, Edit Fields, Google Gemini (Message a model), Respond to Webhook.
- **Logika Alur Kerja**: Data JSON diterima via HTTP POST pada node Webhook, field data dipetakan pada node Edit Fields, diteruskan ke node Gemini AI untuk menghasilkan respons teks dinamis, lalu dikirimkan kembali ke pengirim melalui node Respond to Webhook.

---

## 🌟 Refleksi & Kesan Belajar
Sangat seru mengeksplorasi integrasi antara Webhook trigger, transformasi data JSON, dan pemrosesan prompt AI menggunakan node Gemini di n8n secara langsung.
