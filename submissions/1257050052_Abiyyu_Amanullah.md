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
| **P2** | Webhook Triggers & Data Transformation | [P2_Abiyyu_Amanullah.json](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-02/P2_Abiyyu_Amanullah.json) | [P2_Abiyyu_Amanullah.png](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-02/P2_Abiyyu_Amanullah.png)| Selesai |
| **P3** | Advanced API Integration & Error Handling | [P3_1257050052_Abiyyu_Amanullah.json](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-03/P3_1257050052_Abiyyu_Amanullah.json) | [P3_Abiyyu_Amanullah_Bukti_Positif.png](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-03/P3_Abiyyu_Amanullah_Bukti_Positif.png) & [P3_Abiyyu_Amanullah_Bukti_Negatif.png](https://github.com/abiyyumnllh/GDGoC-n8n-StudyJam/blob/main/Pertemuan-03/P3_Abiyyu_Amanullah_Bukti_Negatif.png) | Selesai |
| **P4** | AI Agent & LLM Chain Automation di n8n | - | - | Belum Selesai |
| **P5** | Capstone Final Project: Smart Autonomous AI | - | - | Belum Selesai |

---

## 💡 Ringkasan & Solusi Otomasi (Workflow Highlights)
Seiring berjalannya Study Jam dari Pertemuan 1 hingga Pertemuan 3, alur kerja otomasi berbasis **Webhook** yang saya bangun berkembang secara bertahap dari sekadar pertukaran data sederhana menjadi sistem pemrosesan berbasis AI dengan percabangan logika:

- **Pertemuan 1 (Dasar Webhook & HTTP Response):** Membangun fondasi alur kerja *request-response* secara *real-time* menggunakan **Webhook Node**, **Edit Fields (Set)**, dan **Respond to Webhook**. Data JSON (`Nama` dan `Pesan`) yang dikirim melalui metode `POST` dari Hoppscotch diolah menggunakan ekspresi dinamis sebelum dikembalikan sebagai respons sukses.
- **Pertemuan 2 (Integrasi AI Persona Generator):** Mengembangkan alur kerja sebelumnya dengan menyisipkan node **Google Gemini** di antara proses *input* dan *output* untuk menghasilkan respons berbasis AI sesuai persona tertentu dari payload yang diterima.
- **Pertemuan 3 (Logika Flow Control & Klasifikasi Sentimen):** Membangun sistem balasan otomatis ulasan pelanggan kafe menggunakan **Switch Node** untuk mengatur percabangan logika. Payload masuk dari **Input Webhook** dan **Format Input** dinilai terlebih dahulu oleh node **Reviewer (Gemini)** ke dalam empat kategori (`POSITIF`, `NETRAL`, `NEGATIF`, dan `SPAM`), lalu diarahkan ke jalur penanganan masing-masing—mulai dari pembuatan kode voucher acak untuk ulasan positif, balasan empatik untuk keluhan, hingga penolakan otomatis untuk pesan spam sebelum dikirim kembali melalui node **Respond**.

---

## 🌟 Refleksi & Kesan Belajar
Pengalaman belajar di n8n Study Jam GDGoC Universitas Widyatama ini sangat seru dan membuka wawasan, terutama karena sebelumnya saya belum pernah menggunakan n8n. Mulai dari Pertemuan 1 yang mengenalkan konsep dasar alur data antar-node dan pengujian API lewat Hoppscotch, berlanjut ke integrasi kecerdasan buatan di Pertemuan 2, hingga akhirnya memahami cara kerja *flow control* menggunakan node `Switch` di Pertemuan 3.

Tantangan paling berkesan muncul saat menguji alur bercabang dan mengelola konfigurasi model serta kuota API Gemini agar setiap jalur dapat dieksekusi dengan lancar. Melalui rangkaian praktik langsung ini, saya jadi jauh lebih paham bagaimana merancang alur otomasi *backend* yang terstruktur, efisien, dan siap dikembangkan untuk kebutuhan proyek nyata.
