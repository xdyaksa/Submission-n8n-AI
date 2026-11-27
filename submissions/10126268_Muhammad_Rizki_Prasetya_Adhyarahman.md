# Submission n8n Study Jam - GDGoC Universitas Widyatama

## 👤 Informasi Peserta
- **Nama Lengkap**: Muhammad Rizki Prasetya Adhyarahman
- **NIM**: 10126268
- **Program Studi**: Teknik Informatika
- **Username GitHub**: mykito09 https://github.com/mykito09
- **URL Repositori Tugas**: https://github.com/mykito09/GDGoC-n8n-StudyJam

---

## 📊 Matriks Progres Tugas (P1 - P5)

| Pertemuan | Topik Tugas | Tautan File Workflow (.json) | Bukti Eksekusi (Screenshot) | Status |
| :---: | :--- | :---: | :---: | :---: |
| **P1** | Pengenalan n8n & Workflow Automation Dasar | [P1_MuhammadRizkiPrasetyaAdhyarahman.json](https://github.com/mykito09/GDGoC-n8n-StudyJam/blob/main/P1_MuhammadRizkiPrasetyaAdhyarahman.json) | [P1_MuhammadRizkiPrasetyaAdhyarahman.png](https://github.com/mykito09/GDGoC-n8n-StudyJam/blob/main/P1_MuhammadRizkiPrasetyaAdhyarahman.png) | Selesai |
| **P2** | Webhook Triggers & Data Transformation | [P2_MuhammadRizkiPrasetyaAdhyarahman.json](https://github.com/mykito09/GDGoC-n8n-StudyJam/blob/main/P2_MuhammadRizkiPrasetyaAdhyarahman.json) | [P2_MuhammadRizkiPrasetyaAdhyarahman_CanvasWorkflow.png](https://github.com/mykito09/GDGoC-n8n-StudyJam/blob/main/P2_MuhammadRizkiPrasetyaAdhyarahman_CanvasWorkflow.png) | Selesai |
| **P3** | Advanced API Integration & Error Handling | [P3_MuhammadRizkiPrasetyaAdhyarahman.json](https://github.com/mykito09/GDGoC-n8n-StudyJam/blob/main/P3_MuhammadRizkiPrasetyaAdhyarahman.json) | [P3_MuhammadRizkiPrasetyaAdhyarahman_Workflow.png](https://github.com/mykito09/GDGoC-n8n-StudyJam/blob/main/P3_MuhammadRizkiPrasetyaAdhyarahman_Workflow.png) | Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | [P4_Nama.json](https://github.com/username-anda/GDGoC-n8n-StudyJam/blob/main/Pertemuan-04/P4_Nama.json) | [P4_Nama.png](https://github.com/username-anda/GDGoC-n8n-StudyJam/blob/main/Pertemuan-04/P4_Nama.png) | Selesai |
| **P5** | Capstone Final Project: Smart Autonomous AI | [P5_Nama.json](https://github.com/username-anda/GDGoC-n8n-StudyJam/blob/main/Pertemuan-05/P5_Nama.json) | [P5_Nama.png](https://github.com/username-anda/GDGoC-n8n-StudyJam/blob/main/Pertemuan-05/P5_Nama.png) | Selesai |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
Tuliskan penjelasan singkat mengenai alur kerja yang telah kamu bangun:
- **Tujuan Workflow**: • Mengotomatiskan proses analisis sentimen dan pembuatan balasan ulasan (review) pelanggan secara instan. Otomasi ini membantu memisahkan ulasan positif, netral, negatif, maupun spam secara cepat di latar belakang, memberikan apresiasi berupa kode voucher khusus untuk pelanggan yang puas, serta menangani keluhan dengan respons empatik tanpa perlu membalasnya secara manual satu per satu.
- **Node Kunci yang Digunakan**: • Webhook (Input Webhook), Edit Fields / Set (Format Input, Kode Voucher, Format Positif, Format Netral, Format Negatif, Format Spam), Google Gemini (AI Reviewer, AI Reply Positif, AI Reply Netral, AI Reply Negatif), Switch (Switch), dan Respond to Webhook (Respond).
- **Logika Alur Kerja**: • Data nama dan ulasan pelanggan masuk melalui Input Webhook (metode POST), lalu distrukturkan oleh Format Input. Data ulasan kemudian dikirim ke AI Reviewer untuk diklasifikasikan sentimennya menjadi empat kategori (POSITIF, NETRAL, NEGATIF, atau SPAM). Node Switch membagi alur berdasarkan hasil klasifikasi tersebut: ulasan POSITIF akan diberi Kode Voucher sebelum dibuatkan balasan apresiasi oleh AI; ulasan NETRAL dan NEGATIF diarahkan ke masing-masing node AI untuk dibuatkan balasan yang sesuai konteks; sedangkan SPAM langsung diformat sebagai ulasan yang diabaikan. Terakhir, seluruh output yang sudah diformat dikembalikan ke sistem pengirim melalui node Respond.

---

## 🌟 Refleksi & Kesan Belajar
Pada pengerjaan kali ini, saya semakin memahami cara mengintegrasikan kecerdasan buatan (Google Gemini) dengan logika percabangan (Switch) di n8n untuk membangun sistem respons otomatis yang dinamis. Tantangan yang sempat ditemui adalah menyesuaikan ekspresi data antar-node, mengelola masa aktif lingkungan kerja n8n, serta menangani kendala high demand (503 Service Unavailable) pada model AI tertentu, namun alur logika keseluruhan sudah dapat disusun dan dipahami dengan baik.
