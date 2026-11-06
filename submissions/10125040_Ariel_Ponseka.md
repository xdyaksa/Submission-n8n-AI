# Submission n8n Study Jam - GDGoC Universitas Widyatama

## 👤 Informasi Peserta
- **Nama Lengkap**: Ariel Ponseka
- **NIM**: 10125040
- **Program Studi**: Teknik Informatika
- **Username GitHub**: [@imrealll](https://github.com/imrealll)
- **URL Repositori Tugas**: [https://github.com/imrealll/GDGoC-n8n-StudyJam](https://github.com/imrealll/GDGoC-n8n-StudyJam)

---

## 📊 Matriks Progres Tugas (P1 - P5)

| Pertemuan | Topik Tugas | Tautan File Workflow (.json) | Bukti Eksekusi (Screenshot) | Status |
| :---: | :--- | :---: | :---: | :---: |
| **P1** | Pengenalan n8n & Workflow Automation Dasar | [P1_Ariel_Ponseka.json](https://github.com/imrealll/GDGoC-n8n-StudyJam/blob/main/Pertemuan-1/P1_Ariel_Ponseka.json) | [P1_Ariel_Ponseka.png](https://github.com/imrealll/GDGoC-n8n-StudyJam/blob/main/Pertemuan-1/P1_Ariel_Ponseka.png) | Selesai |
| **P2** | Webhook Triggers & Data Transformation | - | - | Belum Selesai |
| **P3** | Advanced API Integration & Error Handling | - | - | Belum Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | - | - | Belum Selesai |
| **P5** | Capstone Final Project: Smart Autonomous AI | - | - | Belum Selesai |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
- **Tujuan Workflow**: Membangun alur kerja otomasi n8n berbasis Webhook untuk menerima permintaan HTTP POST, memproses data payload (berupa Nama dan Pesan) secara otomatis menggunakan node Edit Fields, serta mengembalikan pesan balasan kepada client pengirim.
- **Node Kunci yang Digunakan**: Webhook, Edit Fields (Set), Respond to Webhook.
- **Logika Alur Kerja**: 
  1. *Workflow* dipicu (*trigger*) ketika node **Webhook** menerima permintaan HTTP POST pada endpoint path `P1-test` yang memuat parameter data `Nama` dan `Pesan`.
  2. Data payload tersebut diteruskan ke node **Edit Fields** untuk diolah, yaitu menetapkan nilai status `SUCCESS EUY!` dan merangkai balasan dinamis `Terima kasih {{ $json.body.Nama }} , {{ $json.body.Pesan }}`.
  3. Node **Respond to Webhook** mengirimkan hasil olahan data tersebut kembali secara instan sebagai HTTP response kepada pemanggil webhook dengan status sukses.

---

## 🌟 Refleksi & Kesan Belajar
Mengikuti Pertemuan 1 n8n Study Jam bersama GDGoC Universitas Widyatama memberikan pemahaman yang sangat jelas mengenai konsep otomasi visual berbasis flow node. Memahami cara mengintegrasikan Webhook, melakukan manipulasi data sederhana dengan Edit Fields, hingga mengembalikan respons langsung memberikan gambaran nyata betapa cepatnya membangun backend/alur kerja otomatis tanpa perlu menulis kode boilerplate yang rumit. Saya sangat bersemangat untuk melanjutkan ke modul pertemuan selanjutnya, terutama integrasi API lanjutan dan AI Agent.
