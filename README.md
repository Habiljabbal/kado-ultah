# 🎁 Interactive Birthday Card Web App

Sebuah web aplikasi statis (Single Page Application) interaktif dan estetik bertema pastel pink yang dirancang khusus sebagai hadiah ulang tahun digital. Proyek ini mengandalkan manipulasi DOM JavaScript murni dan animasi CSS untuk memberikan pengalaman membuka hadiah digital yang personal dan langsung terintegrasi ke WhatsApp.

---

## 🚀 Fitur Utama

1. **Simulasi Pembukaan Amplop Interaktif (Page 1)**
   - Transisi interaktif dari bentuk amplop surat fisik menggunakan manipulasi properti CSS (`transform`, `rotateX`, dan `z-index`) saat diklik.
   - Efek animasi partikel hati berguguran (*falling hearts animation*) yang diinjeksi secara dinamis ke DOM menggunakan JavaScript.

2. **Surat Ucapan & Desain Estetik (Page 2)**
   - Transisi halaman yang halus memanfaatkan utility classes dari Tailwind CSS.
   - Desain responsif (*Mobile-first*) yang diselaraskan dengan kombinasi Google Fonts romantis (*Sacramento, Caveat, Quicksand*).

3. **Interaktif Gift Picker (Pemilih Kado)**
   - Komponen kartu pilihan kado yang responsif terhadap klik user. Status visual kartu akan berubah secara dinamis untuk menandakan kado yang dipilih.

4. **WhatsApp Gateway Integration**
   - Menyusun teks balasan dari *textarea* dan kado yang dipilih menjadi format `URI Component`, lalu meneruskannya langsung ke API WhatsApp tujuan tanpa memerlukan backend.

---

## 🛠️ Tech Stack

- **UI & Styling:** Tailwind CSS (via CDN)
- **Icons:** FontAwesome v6.5.1
- **Fonts:** Google Fonts API
- **Logic:** Vanilla JavaScript (ES6+)

---

## ⚙️ Cara Konfigurasi Nomor WhatsApp

Buka file `index.html` dan sesuaikan variabel nomor tujuan pada tag `<script>` sebelum dideploy:

```javascript
// Gunakan kode negara (misal: 62 untuk Indonesia)
const MY_WHATSAPP_NUMBER = "628xxx";
