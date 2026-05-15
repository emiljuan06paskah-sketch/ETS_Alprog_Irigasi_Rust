# Sistem Monitoring dan Kontrol Irigasi Otomatis Berbasis Rust 🌾

Repository ini berisi *source code* dan dokumentasi untuk Project Evaluasi Tengah Semester (ETS) mata kuliah Algoritma dan Pemrograman. 

**Disusun Oleh:**
- Arina Sofa'il Assoriyyah (NRP: 2042251022)
- Emil Juan Paskah Purba (NRP: 2042251039)
- **Program Studi:** D4 Teknologi Rekayasa Instrumentasi, ITS

---

## 📝 Deskripsi Project
Sistem ini adalah purwarupa perangkat lunak (*software*) sistem kontrol irigasi otomatis berbasis *closed-loop control system*. Program ini disimulasikan sebagai aplikasi berbasis terminal (*console application*) yang dikembangkan menggunakan bahasa pemrograman **Rust**. 

Sistem ini membaca input multi-variabel, yaitu level air (cm) dan kelembapan tanah (%) dari tiga titik sensor yang berbeda di lahan persawahan. Program menerapkan **Pemrograman Berbasis Objek (OOP)** dan komputasi numerik (*Spatial Average*) untuk bertindak sebagai *controller* cerdas yang mengevaluasi data sensor dan mengendalikan aktuator (pompa irigasi) secara berjenjang.

## 🚀 Cara Menjalankan Program
Untuk menjalankan program simulasi ini di komputer/laptop Anda, ikuti langkah-langkah berikut:

1. **Persiapan:** Pastikan Anda sudah menginstal bahasa pemrograman Rust dan Cargo di sistem Anda (dapat diunduh di [rust-lang.org](https://www.rust-lang.org/)).
2. **Clone Repository:**
   ```bash
   git clone [https://github.com/emiljuan06paskah-sketch/ETS_Alprog_Irigasi_Rust.git](https://github.com/emiljuan06paskah-sketch/ETS_Alprog_Irigasi_Rust.git)<img width="1287" height="463" alt="Skenario 3" src="https://github.com/user-attachments/assets/676d9a04-c7ca-4b1a-ba34-c3cb55c33a3b" />
## 1. Skenario Genangan Ideal (Air >= 3 cm)
Sistem mendeteksi genangan air memadai, sehingga pompa dimatikan untuk menghemat energi.
<img width="1293" height="469" alt="Skenario 1" src="https://github.com/user-attachments/assets/22867a37-21df-4f2e-a675-012c4056332f" />
2. Skenario Air Surut, Tanah Basah
Sistem mendeteksi air surut (< 3 cm), namun residu kelembapan tanah masih baik (>= 65%). Pompa diset ke mode siaga.
<img width="1287" height="476" alt="Skenario 2" src="https://github.com/user-attachments/assets/a9970093-371d-4248-8d9c-eb270cebafc1" />
3. Skenario Kekeringan Ekstrem
Sistem mendeteksi level air habis (< 1 cm) dan tanah sangat kering (< 65%). Alarm aktif dan pompa dinyalakan maksimal.
<img width="1287" height="463" alt="Skenario 3" src="https://github.com/user-attachments/assets/0fea2cc9-7eff-47be-bc2d-5b6512cf5394" />
