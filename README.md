# TP4DPBO2025C1
Tugas Praktikum 4 Dasar Pemrograman Berbasis Objek (DPBO)

# Janji
Saya Faisal Nur Qolbi dengan NIM 2311399 mengerjakan Tugas Praktikum 4 dalam mata kuliah Desain dan Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

# Desain Program
Program kali ini dibuat dengan GUI Java Swing (dengan event handling juga) dengan menggunakan IntelliJ IDEA, dimana ada 2 class yaitu `Menu` dan `Mahasiswa` berikut detailnya:

## Class
1. **Mahasiswa** - Model data yang berisi informasi mahasiswa
2. **Menu** - GUI untuk mengelola data mahasiswa (extends JFrame dari Form Java Swing GUI)

## Atribut
### Class Mahasiswa
- nim (String)
- nama (String)
- jenisKelamin (String)
- nilai (String) - A, B, C, D, atau E

### Class Menu
- Komponen GUI (JTextField, JRadioButton, JComboBox, JTable, dll)
- ArrayList<Mahasiswa> untuk menyimpan data
- selectedIndex (int) - untuk melacak baris yang dipilih di tabel

## Method Utama
### Class Menu
- DefaultTableModel() - mengatur model tabel
- insertData() - menambah data mahasiswa
- updateData() - mengubah data mahasiswa
- deleteData() - menghapus data mahasiswa
- clearForm() - mengosongkan form input
- populateList() - mengisi data awal mahasiswa
- getSelectedNilai() - mendapatkan nilai dari radio button yang dipilih
- setSelectedNilaiRadioButton() - mengatur radio button berdasarkan nilai

# Alur Program
1. Program dimulai, method populateList() dipanggil untuk mengisi data dummy
2. setTable() dipanggil untuk menampilkan data di tabel
3. User dapat:
   - Menambah data: isi form → klik `Add` → insertData() → refresh tabel
   - Mengubah data: pilih/klik data dari tabel → data muncul di form → ubah → klik `Update` → updateData() → refresh tabel
   - Menghapus data: pilih/klik data dari tabel → klik `Delete` → konfirmasi → deleteData() → refresh tabel
   - Membatalkan input: klik `Cancel` → clearForm()
4. Setiap operasi CRUD diakhiri dengan refresh tabel dan feedback ke user untuk memperbarui tabel data

# Dokumentasi
https://github.com/user-attachments/assets/79c7cf23-c4a5-4e23-bb09-48548f7a5131
