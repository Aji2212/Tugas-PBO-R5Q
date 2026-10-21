# Praktikum 3 - Access Modifier Protected pada Java

Aplikasi CRUD (Create, Read, Update, Delete) data mahasiswa menggunakan `ArrayList`, pewarisan (`extends`), access modifier `protected`, dan Java Swing.

## Struktur folder

```text
Praktikum3-CRUD-Mahasiswa/
├── src/
│   ├── induk/Mahasiswa.java
│   ├── anak/MahasiswaApp.java
│   └── gui/MahasiswaGUI.java
└── README.md
```

## Menjalankan aplikasi

Pastikan JDK sudah terpasang. Buka terminal di folder project.

Kompilasi semua file:

```bash
javac -d out src/induk/Mahasiswa.java src/anak/MahasiswaApp.java src/gui/MahasiswaGUI.java
```

Jalankan versi console:

```bash
java -cp out anak.MahasiswaApp
```

Jalankan versi GUI:

```bash
java -cp out gui.MahasiswaGUI
```

## Konsep yang dipraktikkan

- `private`: menyembunyikan `namaApp`, yang dibaca melalui getter `getNamaApp()`.
- `protected`: memberi akses kepada class turunan terhadap data dan method CRUD.
- `extends`: `MahasiswaApp` dan `MahasiswaGUI` mewarisi `Mahasiswa`.
- `ArrayList`: menyimpan daftar nama mahasiswa.
- Swing: `JFrame`, `JTextField`, `JButton`, dan `JTable` untuk antarmuka grafis.
- Komposisi: `JFrame` menjadi field pada `MahasiswaGUI`, bukan superclass-nya.
