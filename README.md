# 🔐 SmoFi – Smart Door Lock & Smoke Detector System

**SmoFi** adalah proyek IoT mini yang mengintegrasikan sistem smart door lock dan deteksi asap (smoke detector) dengan dukungan web dashboard berbasis Laravel. Sistem ini dirancang untuk meningkatkan keamanan ruangan dengan kontrol jarak jauh dan notifikasi saat terdeteksi asap.

---

## 🚀 Fitur Utama

- 🔥 **Deteksi Asap Otomatis**  
  Sensor mendeteksi keberadaan asap dan mengirimkan log ke server.

- 🔐 **Kontrol Smart Lock via Web**  
  Admin dapat membuka pintu secara remote melalui dashboard web.

- 📊 **Monitoring Log**  
  Riwayat aktivitas pintu dan level asap tercatat dan ditampilkan di web.

- 👤 **Manajemen Akses Admin**  
  Hanya user dengan peran admin yang dapat membuka pintu.

---

## 🛠️ Teknologi yang Digunakan

| Komponen       | Teknologi               |
|----------------|--------------------------|
| Backend        | Laravel (PHP)            |
| Frontend       | Blade Template + Bootstrap |
| Database       | MySQL                    |
| IoT Device     | ESP32, MQ-2 / MQ-135, Solenoid Lock |
| Komunikasi     | MQTT                     |

---

## 🔌 IoT Device Setup

- ESP32 membaca sensor asap (MQ-2 / MQ-135)
- ESP32 mengirim data ke broker MQTT
- Server Laravel menerima data dari MQTT (gunakan bridge atau microservice jika diperlukan)

---

