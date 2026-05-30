# Pintarnya.com - Telegram Q&A Chatbot 🤖💼

Repository ini berisi workflow otomatisasi (Tugas 5) untuk membangun asisten virtual (Chatbot) via Telegram. Chatbot ini dirancang khusus untuk menjawab pertanyaan seputar **Pintarnya.com**, platform lowongan kerja digital untuk pekerja kerah biru (*blue collar*) di Indonesia.

## 📋 Fitur Utama
- **Integrasi Telegram:** Berinteraksi langsung dengan pengguna melalui bot Telegram.
- **Q&A Otomatis:** Menjawab FAQ seputar cara daftar, melamar kerja, jenis pekerjaan, dan keamanan data di platform Pintarnya.
- **Fallback Web Search:** Terintegrasi dengan **SerpAPI**. Jika pertanyaan pengguna berada di luar cakupan FAQ, bot akan otomatis mencari informasi relevan melalui internet.
- **Tone & Persona:** Menjawab dengan ramah, ringkas, dan informatif menggunakan Bahasa Indonesia sesuai dengan standar *customer support* Pintarnya.

## 📂 File Workflow
Terdapat dua file workflow dalam repository ini:
1. `Tugas 5.json` - Workflow utama untuk chatbot Telegram.
2. `Tugas 5 copy.json` - Salinan/backup dari workflow utama.

## 🚀 Cara Menggunakan Workflow Ini
1. Unduh (download) file `.json` dari repository ini.
2. Buka platform [n8n](https://n8n.io/) Anda.
3. Pada halaman workflow, klik **Import from File** atau *copy-paste* isi file JSON langsung ke canvas n8n.
4. Pastikan Anda telah mengatur kredensial (*credentials*) berikut di n8n:
   - **Telegram Bot Token** (dapatkan dari BotFather di Telegram).
   - **API Key LLM** (misalnya OpenAI API Key untuk memproses System Prompt).
   - **SerpAPI Key** (untuk fitur pencarian web).
5. Aktifkan workflow dan tes chat melalui bot Telegram Anda.

## 🧠 System Prompt & Pengetahuan Dasar
Bot ini ditenagai oleh prompt sistem berikut untuk menjaga persona sebagai asisten virtual Pintarnya:

> Kamu adalah asisten virtual Pintarnya, platform lowongan kerja Indonesia yang terpercaya, terdaftar di KEMNAKER dan diawasi oleh KOMINFO. Pintarnya didirikan Mei 2022 oleh Nelly Nurmalasari, Ghirish Pakerdas, dan Herry Hendrowan untuk membantu 60 juta pekerja kerah biru di Indonesia. Jawab pertanyaan dengan ramah, ringkas, dan dalam Bahasa Indonesia. Jika pertanyaan di luar topik Pintarnya, arahkan pengguna kembali ke layanan kami. Jika pertanyaan tidak ada dalam FAQ, jawab dengan jujur bahwa kamu tidak memiliki informasi tersebut maka kamu silahkan gunakan tool Serpapi.

*Tugas ini dibuat untuk memenuhi requirement evaluasi pembuatan AI Chatbot terintegrasi.*
