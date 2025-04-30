
# WhatsApp Bot di Termux menggunakan Baileys

Bot WhatsApp ini dibuat menggunakan **Baileys** (pustaka untuk Node.js) dan dapat dijalankan langsung di **Termux** di perangkat Android. Dengan bot ini, kamu dapat mengirim pesan otomatis melalui WhatsApp menggunakan koneksi WhatsApp Web.

---

## Langkah-Langkah

### 1. Install Node.js dan Git

Pastikan kamu telah menginstal **Node.js** dan **Git** di Termux:

```bash
pkg update && pkg upgrade
pkg install nodejs git
```

### 2. Clone Repositori Bot WhatsApp

Clone repositori **Baileys** untuk mulai membuat bot WhatsApp:

```bash
git clone https://github.com/adiwajshing/Baileys
cd Baileys
npm install
```

Atau kamu bisa memilih untuk menggunakan **bot siap pakai**:

```bash
git clone https://github.com/DGXeon/CheemsBot-MD3
cd CheemsBot-MD3
npm install
```

### 3. Jalankan Bot

Setelah menginstal semua dependencies, jalankan bot dengan perintah:

```bash
node .
```

Saat pertama kali menjalankan bot, kamu akan diminta untuk memindai **QR Code** menggunakan aplikasi WhatsApp di ponsel kamu untuk autentikasi.

---

## Catatan Penting

- **Jangan logout dari WhatsApp Web** setelah kamu memindai QR Code, karena koneksi bot dapat terputus.
- Bot ini hanya bisa berjalan selama **Termux** tetap aktif. Kamu bisa menggunakan tool seperti `tmux` untuk membuat bot tetap berjalan di background.
- Pastikan koneksi internet kamu stabil agar bot dapat tetap terhubung ke WhatsApp.

---

## Custom Fitur Bot

Jika kamu ingin **menyesuaikan** bot atau menambahkan fitur tertentu (seperti auto-reply, integrasi API, atau lainnya), kamu bisa melakukan modifikasi di dalam file `index.js` atau file utama bot sesuai kebutuhan.

---

### Menjalankan Bot secara Otomatis

Jika kamu ingin bot berjalan terus menerus tanpa harus menjaga Termux tetap terbuka, kamu bisa menggunakan **tmux** atau **screen** untuk menjalankannya di background:

```bash
pkg install tmux
tmux
node .
```

---

Selamat menggunakan bot WhatsApp kamu di Termux! 🚀
