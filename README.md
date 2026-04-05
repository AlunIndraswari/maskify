# maskify

# Maskify 

**Maskify** adalah aplikasi web berbasis Flask yang dirancang untuk membantu pengguna melindungi informasi sensitif dalam teks. Aplikasi ini secara otomatis menyensor (masking) data pribadi dan kata-kata kasar untuk memastikan privasi dan kepatuhan konten sebelum dibagikan atau dipublikasikan.

## Fitur Utama

* **Penyensoran NIK (Nomor Induk Kependudukan):** Mendeteksi pola NIK Indonesia berdasarkan kode provinsi yang valid.
* **Masking Email:** Melindungi alamat email dari pengambilan data otomatis (*scrapping*).
* **Deteksi URL/Link:** Menyensor tautan situs web agar teks tetap bersih dan aman.
* **Filter Kata Kasar (Profanity Filter):** Menghapus kata-kata kasar atau umpatan dalam bahasa Indonesia dan Inggris menggunakan pencocokan pola Regex yang kuat.
* **Privacy-First:** Sistem tidak menyimpan data teks yang diinputkan oleh pengguna ke dalam database mana pun.

## Teknologi yang Digunakan

* **Back-End:** Python & Flask
* **Logic:** Regular Expressions (Re) untuk pengenalan pola data.
* **Front-End:** Jinja2 Template Engine (HTML/CSS).

## Instalasi & Cara Menjalankan

1.  **Clone repositori:**
    ```sh
    git clone [https://github.com/username/maskify.git](https://github.com/username/maskify.git)
    cd maskify
    ```

2.  **Instal Flask:**
    ```sh
    pip install flask
    ```

3.  **Jalankan aplikasi:**
    ```sh
    python app.py
    ```

4.  **Akses di browser:**
    Buka `http://127.0.0.1:5000`

## Cara Penggunaan

1.  Buka menu **Masking**.
2.  Masukkan teks yang mengandung informasi sensitif atau kata kasar.
3.  Pilih jenis data yang ingin disensor (NIK, Email, Link, atau Kata Kasar).
4.  Klik tombol proses, dan aplikasi akan menampilkan teks yang telah disensor dengan karakter `*`.
