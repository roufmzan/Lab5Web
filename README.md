# Nama : Felix Amon Sitinjak
# NIM : 312410063
# Kelas : TI.24.A1

**Hasil Output**

<img width="959" height="503" alt="image" src="https://github.com/user-attachments/assets/1ce91ee7-8624-45e7-8797-8bf114fd8d00" />

**Code**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
<html>
<head>
    <title>alert box</title>
</head>
<body>
    <script language="javascript">
    <!--
        window.alert("ini merupakan pesan untuk anda");
    //-->
    </script>
</body>
</html>
<html>
<head>
    <title>skrip javascript</title>
</head>
<body>
    percobaan memakai javascript:<br>
    <script language="javascript">
    <!--
        document.write("selamat mencoba javascript<br>");
        document.write("semoga sukses!");
    //-->
    </script>
</body>
</html>
<html>
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language="javascript">
    <!--
        var nama = prompt("siapa nama anda?", "masukkan nama anda");
        document.write("hai, " + nama);
    //-->
    </script>
</body>
</html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function pesan() {
            alert("memanggil javascript lewat body onload");
        }
    </script>
</head>
<body onload="pesan()">
</body>
</html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test(val1, val2) {
            document.write("<br>perkalian : val1 * val2 = " + (val1 * val2) + "<br>");
            document.write("pembagian : val1 / val2 = " + (val1 / val2) + "<br>");
            document.write("penjumlahan : val1 + val2 = " + (val1 + val2) + "<br>");
            document.write("pengurangan : val1 - val2 = " + (val1 - val2) + "<br>");
            document.write("modulus : val1 % val2 = " + (val1 % val2) + "<br>");
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick="test(9,4)">
</body>
</html>
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language="javascript">
    <!--
        var nilai = prompt("nilai (0-100): ", 0);
        var hasil = "";
        if (nilai >= 60)
            hasil = "lulus";
        else
            hasil = "tidak lulus";
        document.write("hasil: " + hasil);
    //-->
    </script>
</body>
</html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test() {
            var val1 = window.prompt("input nilai (1-5):");
            switch (val1) {
                case "1":
                    document.write("bilangan satu");
                    break;
                case "2":
                    document.write("bilangan dua");
                    break;
                case "3":
                    document.write("bilangan tiga");
                    break;
                case "4":
                    document.write("bilangan empat");
                    break;
                case "5":
                    document.write("bilangan lima");
                    break;
                default:
                    document.write("bilangan lainnya");
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick="test()">
</body>
</html>
<html>
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test() {
            var val1 = document.kirim.T1.value;
            if (val1 % 2 == 0)
                document.kirim.T2.value = "bilangan genap";
            else
                document.kirim.T2.value = "bilangan ganjil";
        }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick="test()"></p>
    </form>
</body>
</html>
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language="javascript">
    <!--
        function ubahWarnaLB(warna) {
            document.bgColor = warna;
        }
        function ubahWarnaLD(warna) {
            document.fgColor = warna;
        }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onClick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onClick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onClick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onClick="ubahWarnaLD('BLUE')">
    </form>

    <script language="javascript">
    <!--
        document.write("Dimodifikasi terakhir pada " + document.lastModified);
    //-->
    </script>
</body>
</html>
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
            total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0) {
                    total -= parseInt(harga);
                }
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500</label><hr />
    <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
</body>
</html>
```

**Penjelasan**
# Praktikum Lab 5 - Pengenalan JavaScript

# Deskripsi
File ini berisi kumpulan contoh dasar penggunaan **JavaScript** di dalam halaman HTML.  
Tujuannya adalah untuk memahami cara kerja **JavaScript** dalam:
- Menampilkan output ke halaman (`document.write`)
- Menampilkan pesan ke pengguna (`alert`, `prompt`)
- Melakukan operasi aritmatika
- Struktur kontrol (`if-else`, `switch`)
- Manipulasi objek `document`
- Interaksi dengan elemen HTML melalui `onclick`
- Menghitung total harga menggunakan `checkbox`

---

# Isi File
### `lab5_javascript.html`
Berisi beberapa contoh script JavaScript dalam satu file:
1. **Hello World**
   - Menampilkan teks menggunakan `document.write()` dan `console.log()`.
2. **Alert Box**
   - Menampilkan pesan peringatan dengan `window.alert()`.
3. **Prompt Input**
   - Mengambil input nama dari pengguna dan menampilkannya di halaman.
4. **Operasi Aritmatika**
   - Menghitung hasil penjumlahan, pengurangan, perkalian, pembagian, dan modulus.
5. **Percabangan `if-else`**
   - Menentukan kelulusan berdasarkan nilai.
6. **Percabangan `switch-case`**
   - Menentukan teks berdasarkan angka input pengguna.
7. **Pengecekan Bilangan Ganjil/Genap**
   - Mengambil input angka dan menampilkan apakah genap atau ganjil.
8. **Manipulasi Warna Latar & Teks**
   - Mengubah warna latar belakang dan warna teks halaman.
9. **Daftar Menu Makanan**
   - Menghitung total harga berdasarkan checkbox yang dipilih.
