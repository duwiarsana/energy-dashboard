# Energy Meter Dashboard

Sebuah dashboard untuk memantau konsumsi energi listrik secara real-time menggunakan MQTT.

## Fitur
- Menampilkan data real-time: Tegangan, Arus, Daya, Energi, Power Factor, dan Biaya
- Tampilan responsif yang mendukung perangkat mobile
- Koneksi MQTT untuk pembaruan data otomatis
- Antarmuka pengguna yang modern dan mudah dibaca

## Teknologi
- HTML, CSS, JavaScript
- MQTT.js untuk koneksi ke broker MQTT
- Google Fonts untuk tipografi

## Instalasi
1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/Energy-Dashboard.git
   cd Energy-Dashboard
   ```

2. Buka `index.html` di browser web Anda

## Konfigurasi
Edit variabel berikut di file `index.html` sesuai kebutuhan:
```javascript
const brokerUrl = 'ws://broker.emqx.io:8083/mqtt';
const tarifPerKwh = 1500; // Sesuaikan dengan tarif listrik per kWh
```

> **Catatan**: Koneksi MQTT tidak menggunakan username/password. Jika broker Anda membutuhkan autentikasi, aktifkan baris `mqtt_username` dan `mqtt_password` di `index.html`.

## Topik MQTT
Dashboard ini berlangganan ke topik-topik berikut:
- `alat1/tegangan`
- `alat1/arus`
- `alat1/daya`
- `alat1/kwh`
- `alat1/pf`

## Kontribusi
Silakan buat pull request untuk berkontribusi pada proyek ini.

## Lisensi
MIT
