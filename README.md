# Sistem Monitoring dan Kontrol Irigasi Otomatis Berbasis Rust 

Repository ini berisi *source code* dan dokumentasi untuk Project Evaluasi Tengah Semester (ETS) mata kuliah Algoritma dan Pemrograman. 

**Disusun Oleh:**
- Arina Sofa'il Assoriyyah (NRP: 2042251022)
- Emil Juan Paskah Purba (NRP: 2042251039)
- **Program Studi:** D4 Teknologi Rekayasa Instrumentasi, ITS

---

##  Deskripsi Project
Sistem ini adalah purwarupa perangkat lunak (*software*) sistem kontrol irigasi otomatis berbasis *closed-loop control system*. Program ini disimulasikan sebagai aplikasi berbasis terminal (*console application*) yang dikembangkan menggunakan bahasa pemrograman **Rust**. 

Sistem ini membaca input multi-variabel, yaitu level air (cm) dan kelembapan tanah (%) dari tiga titik sensor yang berbeda di lahan persawahan. Program menerapkan **Pemrograman Berbasis Objek (OOP)** dan komputasi numerik (*Spatial Average*) untuk bertindak sebagai *controller* cerdas yang mengevaluasi data sensor dan mengendalikan aktuator (pompa irigasi) secara berjenjang.

## 🚀 Cara Menjalankan Program
Untuk menjalankan program simulasi ini di komputer/laptop Anda, ikuti langkah-langkah berikut:

1. **Persiapan:** Pastikan Anda sudah menginstal bahasa pemrograman Rust dan Cargo di sistem Anda (dapat diunduh di [rust-lang.org](https://www.rust-lang.org/)).
2. **Clone Repository:**
   ```bash
   git clone [https://github.com/emiljuan06paskah-sketch/ETS_Alprog_Irigasi_Rust.git](https://github.com/emiljuan06paskah-sketch/ETS_Alprog_Irigasi_Rust.git)
