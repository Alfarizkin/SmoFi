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

📸 Screenshot Tampilan Website

1. 📝 Register Page  
   ![register_page](https://github.com/user-attachments/assets/37318707-661d-4019-85ca-d5d7c2fd6313)

2. 🔐 Login Page  
   ![login_page](https://github.com/user-attachments/assets/8f1ce761-c42c-4706-9f85-553ab0e247fb)

3. 🚪 Door Lock / Unlock Control  
   ![door_lock_unlock_page](https://github.com/user-attachments/assets/9f05beb0-6f3a-4cfd-8497-9805854ed59f)

4. ✋ Enroll Fingerprint Page  
   ![enroll_fingerprint_page](https://github.com/user-attachments/assets/4c501d74-9dc5-4bff-93fb-2c6153f799c5)

5. 📑 Log Akses Pintu  
   ![log_access_page](https://github.com/user-attachments/assets/4decfef1-8bd5-4fb6-825f-462cca110433)

6. 🔥 Smoke Monitoring Page  
   ![smoke_monitoring_page](https://github.com/user-attachments/assets/feb39e3f-a5d1-4244-acd4-ef781d9baa86)

7. 👤 User List Page  
   ![user_list_page](https://github.com/user-attachments/assets/da83876c-03f1-4fa4-89c5-b80034f8db1c)

---

---

## Kontributor

| Nama                          | NIM         | Peran & Kontribusi                                                                 |
|-------------------------------|-------------|-------------------------------------------------------------------------------------|
| **Itsar Hevara**              | 2207421046  | Perancangan sistem secara keseluruhan dan integrasi modul                         |
| **Devina Anggraini**          | 2207421033  | Pengembangan antarmuka frontend (UI dashboard & halaman pengguna)                 |
| **Alfarizki Nurachman**       | 2207421041  | Pengembangan frontend log fingerprint, serta backend website termasuk integrasi WebSocket |
| **Abdurrahman Ammar Ihsan**   | 2207421047  | Implementasi IoT Smart Door Lock (ESP32 & Solenoid Lock)                          |
| **Izzaturrachmi**             | 2207421050  | Penanganan aspek keamanan sistem (akses admin, validasi, otorisasi)               |
| **Jonathan Victorian Wijaya** | 2207421051  | Implementasi IoT Smoke Detector (sensor MQ-2)                             |

