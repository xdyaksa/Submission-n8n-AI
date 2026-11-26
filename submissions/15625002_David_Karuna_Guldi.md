# Submission n8n Study Jam - GDGoC Universitas Widyatama

## 👤 Informasi Peserta
- **Nama Lengkap**: David Karuna Guldi
- **NIM**: 15625002
- **Program Studi**: Teknik Robotika dan Kecerdasan Buatan
- **Username GitHub**: [@hirodav](https://github.com/hirodav)
- **URL Repositori Tugas**: [https://github.com/hirodav/GDGoC-n8n-StudyJam](https://github.com/hirodav/GDGoC-n8n-StudyJam)

---

## 📊 Matriks Progres Tugas (P1 - P5)

| Pertemuan | Topik Tugas | Tautan File Workflow (.json) | Bukti Eksekusi (Screenshot) | Status |
| :---: | :--- | :---: | :---: | :---: |
| **P1** | Pengenalan n8n & Workflow Automation Dasar | [P1_David_Karuna_Guldi.json](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-01/P1_David_Karuna_Guldi.json) | [P1_David_Karuna_Guldi.png](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-01/P1_David_Karuna_Guldi.png) | Selesai |
| **P2** | Webhook Triggers & Data Transformation | [P2_David_Karuna_Guldi.json](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-02/P2_David_Karuna_Guldi.json) | [P2_David_Karuna_Guldi.png](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-02/P2_David_Karuna_Guldi.png) | Selesai |
| **P3** | Advanced API Integration & Error Handling | [P3_David_Karuna_Guldi.json](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-03/P3_David_Karuna_Guldi.json) | [P3_David_Karuna_Guldi.png](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-03/P3_David_Karuna_Guldi.png) | Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | [P4_David_Karuna_Guldi.json](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-04/P4_David_Karuna_Guldi.json) | [P4_David_Karuna_Guldi.png](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-04/P4_David_Karuna_Guldi.png) | Belum |
| **P5** | Capstone Final Project: Smart Autonomous AI | [P5_David_Karuna_Guldi.json](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-05/P5_David_Karuna_Guldi.json) | [P5_David_Karuna_Guldi.png](https://github.com/hirodav/GDGoC-n8n-StudyJam/blob/main/Pertemuan-05/P5_David_Karuna_Guldi.png) | Belum |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
Tuliskan penjelasan singkat mengenai alur kerja yang telah kamu bangun:
- **Tujuan Workflow**:
  - **P1**: Webhook Aspirasi yang merapikan data pengirim dari Hoppscotch dan membalas otomatis.
  - **P2 (AI Persona Generator)**: Webhook menerima `Nama` dan `Hobi`, lalu Google Gemini membuat komentar singkat 1 paragraf dengan persona yang ramah.
  - **P3 (Smart Review Desk)**: Klasifikasi sentimen review kafe (`POSITIF`, `NETRAL`, `NEGATIF`, `SPAM`) + anti *prompt-injection*, percabangan Switch dengan *fallback*, generator kode voucher `KOPIPUAS-xxx`, dan normalisasi output JSON 6 field.
- **Node Kunci yang Digunakan**: Webhook, Edit Fields (Set), Google Gemini (`Message a model` + Retry On Fail), Switch (Rules + Fallback Extra Output), Respond to Webhook.
- **Logika Alur Kerja**: Data masuk via POST Webhook, dinormalisasi dengan Edit Fields, diproses oleh Google Gemini (klasifikasi & balasan personal pada P3, komentar persona pada P2), diarahkan sesuai kategori oleh Switch, lalu dikembalikan ke pemanggil via Respond to Webhook.

---

## 🌟 Refleksi & Kesan Belajar
- **P1**: Memahami konsep `Workflow = Trigger + Action` dan webhook sebagai pemicu real-time.
- **P2**: Belajar menghubungkan LLM (Google Gemini), mengatur system message/persona, serta mengaktifkan `Retry On Fail` untuk mengatasi limit sementara.
- **P3**: Mempelajari alur percabangan `Switch` + *fallback*, referensi node eksplisit `$('Format Input')` setelah node AI menimpa `$json`, dan normalisasi skema JSON akhir agar bisa disatukan ke satu `Respond to Webhook`.
