# FIRDHAN AGENT — AI + FULL WINDOWS ASSISTANT

**Firdhan Agent** adalah asisten desktop cerdas berbasis Python yang menggabungkan integrasi AI (OpenRouter) dengan kontrol sistem operasi Windows tingkat lanjut. Aplikasi ini menampilkan antarmuka Tkinter kustom bertema siber yang mendukung eksekusi perintah lokal, pemantauan kamera, dan penyematan jendela aplikasi eksternal (*window embedding*).

## 🚀 Fitur Utama

* **🤖 AI Assistant:** Antarmuka obrolan terintegrasi dengan OpenRouter untuk pemrosesan bahasa alami dan eksekusi aksi otomatis.
* **💻 System Terminal:** Terminal bawaan untuk mengeksekusi perintah Windows lokal (OSINT & eksekusi baris perintah) secara langsung tanpa membuka CMD terpisah.
* **🪟 Multi-Tasking Window Embedder:** Grid 2x2 interaktif yang menggunakan `ctypes` OS Windows untuk menarik dan menyematkan (*embed*) aplikasi Windows lain ke dalam antarmuka Firdhan Agent.
* **⚙️ Dynamic AI Configuration:** Panel khusus untuk menyesuaikan *Persona* (Prompt Injection) dan *System Prompt* secara *real-time* yang langsung tersimpan ke dalam konfigurasi.
* **📷 Camera Integration:** Pemrosesan umpan kamera perangkat secara langsung menggunakan OpenCV.
* **🎨 Custom UI/UX:** Tampilan mode gelap dengan animasi *glitch* logo, indikator status yang berdenyut (*pulse*), dan perutean input cerdas untuk mencegah hilangnya fokus pada jendela yang disematkan.

## 📋 Prasyarat Sistem

Aplikasi ini menggunakan manipulasi jendela tingkat OS (via `ctypes.windll.user32`), sehingga **diwajibkan berjalan di lingkungan OS Windows**.

Pastikan Python 3.8+ sudah terinstal, lalu instal dependensi berikut:

```bash
pip install opencv-python Pillow requests

(Catatan: Pustaka seperti tkinter, ctypes, threading, dan datetime merupakan bawaan standar Python).

🛠️ Konfigurasi
Sebelum menjalankan aplikasi, Anda perlu mengatur kredensial AI:

Buka file skrip utama.

Temukan variabel API_KEYS di bagian atas kode.

Masukkan OpenRouter API Key Anda yang valid.

💻 Penggunaan
Jalankan skrip utama melalui Command Prompt atau PowerShell:
python3 firdmultask.py

Navigasi Menu
◎ ASSISTANT: Mode utama untuk memberikan instruksi kepada AI atau menguji perintah dasar.

◎ SYSTEM: Ruang kerja khusus sistem operasi. Anda dapat mengetik search_apikeys untuk menjalankan pemindaian otomatis, atau menjalankan perintah Command Prompt biasa.

◎ MULTI TASKING: Klik "REFRESH APPS" untuk mendeteksi aplikasi Windows yang sedang berjalan, lalu sematkan hingga 4 aplikasi berbeda di dalam grid Firdhan Agent.

◎ AI CONFIG: Sesuaikan gaya bicara dan batasan sistem AI. Klik "SIMPAN KONFIGURASI" untuk menerapkan perubahan tanpa perlu restart aplikasi.

Author: Danar Firdhan Roichan
