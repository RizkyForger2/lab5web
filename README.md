Membuat Dokumen HTML dengan nama file

      <!DOCTYPE html>
      <html lang="en">
      <head>
          <title>Mengenal JavaScript</title>
      </head>
      <body>
          <h1>Pengenalan JavaScript</h1>
          <h3>Contoh dokument.write dan console.log</h3>
          <script>
              document.write("Hello Word");
              console.log("Hello Word");
          </script>    
      </body>
      </html>
  
![Screenshot 2024-11-04 120850](https://github.com/user-attachments/assets/20f68830-d0c3-47f7-8917-cd9b4381ac2d)

Kode JavaScript ini menggunakan document.write untuk menampilkan "Hello World" langsung di halaman web, sementara console.log mencetak teks tersebut di konsol browser. document.write berguna untuk menampilkan konten di halaman, sedangkan console.log bermanfaat untuk debugging tanpa memengaruhi tampilan halaman.

2. Pemakaian Alert sebagai property window.

  <!DOCTYPE html>
  <html lang="en">
  <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>alert box</title>
   </head>
   <body>
       <script language = "Javascript">
           window.alert("ini merupakan pesan untuk anda");
       </script>
   </body>
   </html>

   ![Screenshot 2024-11-04 121020](https://github.com/user-attachments/assets/99552bcc-0456-4c82-9b95-7a3c4173d8ec)

Kode JavaScript ini memakai window.alert untuk menampilkan kotak pesan (alert box) yang berisi teks "ini merupakan pesan untuk anda" begitu halaman dimuat. Pengguna harus menutup kotak pesan ini agar dapat melanjutkan interaksi dengan halaman.

3. Pemakaian method dalam objek

                 <!DOCTYPE html>
                 <html lang="en">
                 <head>
                     <meta charset="UTF-8">
                     <meta name="viewport" content="width=device-width, initial-scale=1.0">
                     <title>Skrip JavaScript</title>
                 </head>
                 <body>
                     percobaan memakai JavaScript:<br>
                     <script language = "javascript">
                         document.write("Selamat mencoba Javascript<br>");
                         document.write("Semoga sukses!");
                     </script>
                     
                 </body>
                 </html>

     ![Screenshot 2024-11-04 121106](https://github.com/user-attachments/assets/51218854-a2a1-4de3-8181-5c91635c7a2e)

Kode JavaScript ini menampilkan teks "selamat mencoba javascript" diikuti dengan pindah baris (<br>), lalu menampilkan "semoga sukses!" di halaman web. document.write digunakan untuk langsung menuliskan teks ke halaman saat kode dijalankan.

Pemakaian Prompt

                <!DOCTYPE html>
                <html lang="en">
                <head>
                    <meta charset="UTF-8">
                    <meta name="viewport" content="width=device-width, initial-scale=1.0">
                    <title>Pemasukan data</title>
                </head>
                <script language = "javascript">
                    var nama = prompt("Siapa nama anda?","Masukkan nama anda");
                    document.write("hai, "+ nama);
                </script>
                <body>
                    
                </body>
                </html>
    

![Screenshot 2024-11-04 121306](https://github.com/user-attachments/assets/a6e3df63-8be4-46b6-82f9-3a144a4b0947)

    Setelah perintah tadi lalu muncul seperti gambar diatas, lalu ketik "Nama Muhammad Rizky" lalu akan muncul seperti gambar dibawah ini

  ![Screenshot 2024-11-04 121343](https://github.com/user-attachments/assets/e5855c72-d730-4f1e-befc-a4825365152d)

  nah "Muhammad Rizky" akan muncul seperti yang diatas

5. Pembuatan fungsi dan cara pemanggilannya

              <!DOCTYPE html>
              <html lang="en">
              <head>
                  <title>Contoh program javascript </title>
                  <script language = "javascript">
                      function pesan(){
                          alert("Memanggil javascript lewat body onload")
                      }
                  </script>
              </head>
              <body onload=pesan()>
              </body>
              </html>

  ![Screenshot 2024-11-04 121422](https://github.com/user-attachments/assets/d219ac21-6a1d-4f35-96ae-c54dac825f74)

 Kode ini memunculkan kotak pesan (alert box) dengan teks "memanggil javascript lewat body onload" ketika halaman selesai dimuat. Atribut onload="pesan()" di dalam tag <body> secara otomatis memanggil fungsi pesan() saat halaman selesai dimuat, sehingga pesan ditampilkan sebagai pop-up.

6. Dasar Pemrograman Di Javascript
   
      Operasi Dasar Aritmatika
      <html>
      <head>
          <title>contoh program javascript</title>
          <script language="javascript">
              function test (val1, val2)
              {
                  document.write("<br>"+"perkalian : val1*val2"+"<br>")
                  document.write(val1*val2)
                  document.write("<br>"+"pembagian : val1/val2 "+"<br>")
                  document.write(val1/val2)
                  document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
                  document.write(val1+val2)
                  document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
                  document.write(val1-val2)
                  document.write("<br>"+"mmodulus : val1%val2 "+"<br>")
                  ocument.write(val1%val2)
              }
          </script>
      </head>
      <body>
          <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
      </body>
      </html>

    ![Screenshot 2024-11-04 121529](https://github.com/user-attachments/assets/2e7a4985-131b-4b89-bcf6-a35274141661)
   ![Screenshot 2024-11-04 121542](https://github.com/user-attachments/assets/18b115a2-0669-4ddc-ae09-bf490add12ec)

Kode ini mendefinisikan fungsi test(val1, val2) yang menjalankan operasi aritmatika (perkalian, pembagian, penjumlahan, pengurangan, dan modulus) pada dua angka yang diberikan. Ketika tombol "arithmetic" diklik, fungsi dipanggil dengan nilai 9 dan 4. Hasil dari setiap operasi ditampilkan di halaman melalui document.write, menghasilkan output berikut:

Perkalian: 36
Pembagian: 2.25
Penjumlahan: 13
Pengurangan: 5
Modulus: 1

7. Seleksi kondisi (if..else)

  <html>
  <head>
      <title>contoh if-else</title>
      <script language="javascript">
          var nilai = prompt("nilai (0-100): ", 0);
          var hasil = " ";
          if (nilai >= 60)
          hasil = "lulus";
          else
          hasil = "tidak lulus";
          document.write("hasil: " + hasil);
      </script>
  </head>
  <body>
  </html>

  ![Screenshot 2024-11-04 121732](https://github.com/user-attachments/assets/1c7490cc-5016-44b8-b92f-db6204e8766f)

  setelah mengikuti perintah tersebut akan muncul gambar seperti ini, lalu saya akan mengisi dengan angka 75
  
  ![Screenshot 2024-11-04 121841](https://github.com/user-attachments/assets/29206cdd-327a-4203-845b-3ac5a4c0522d)

dan hasilnya lulus.

8. Penggunaan operator switch untuk seleksi kondisi

    <html>
    <head>
        <title>contoh if-else</title>
        <script language="javascript">
                function test() {
                    let val = window.prompt("Input nilai (1-5):")
                    switch (val) {
                        case "1":
                            document.write("Bilangan satu")
                            break
                        case "2":
                            document.write("Bilangan dua")
                            break
                        case "3":
                            document.write("Bilangan tiga")
                            break
                        case "4":
                            document.write("Bilangan empat")
                            break
                        case "5":
                            document.write("Bilangan lima")
                            break
                        default:
                            document.write("Bilangan lainnya")
               }
        }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="switch" onclick=test()>
    </body>
    </html>

![Screenshot 2024-11-04 121938](https://github.com/user-attachments/assets/1173bfbc-d737-4d97-9f86-3c0afc6cb249)
![Screenshot 2024-11-04 124318](https://github.com/user-attachments/assets/ba9eb36b-43b1-4e60-ba0d-1b0e30c7578c)

Ketika angka 4 dimasukkan sebagai output dari perintah tersebut, hasil yang ditampilkan adalah

![Screenshot 2024-11-04 122020](https://github.com/user-attachments/assets/bcc46cd5-3606-467f-ab64-366e352678d2)

"bilangan 4"

9. Form Input

    <html>
    <head>
        <title>Contoh if-else</title>
        <script language="javascript">
        function test() {
            var val1 = document.kirim.T1.value; // Ganti 'ver' dengan 'var'
            if (val1 % 2 == 0)
                document.kirim.T2.value = "bilangan genap";
            else
                document.kirim.T2.value = "bilangan ganjil";
        }
        </script>
    </head>
    <body>
        <form method="POST" name="kirim">
            <p>BIL <input type="text" name="T1" size="20"> <!-- Ganti T2 dengan T1 -->
            MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
            <p><input type="button" value="TEBAK" name="B1" onclick="test()"></p> <!-- Tambahkan tanda kutip -->
        </form>
    </body>
    </html>

    ![Screenshot 2024-11-04 122200](https://github.com/user-attachments/assets/3feea3f4-e18d-4c5d-8b14-afb642f67e38)

   Kode ini memeriksa apakah nilai yang dimasukkan pada kotak input pertama (T1) merupakan bilangan genap atau ganjil. Saat tombol "TEBAK" ditekan, hasilnya akan ditampilkan di kotak input kedua (T2) dengan keterangan "bilangan genap" atau "bilangan ganjil".

10. from button

  <html>
  <head>
      <title>objek document</title>
  </head>
  <body>
      <script language="javascript">
          function ubahWarnaLB(warna) {
              document.bgColor = warna;
          }
          function ubahWarnaLD(warna) {
              document.fgColor = warna;
          }
          </script>
          <h1>tes</h1>
          <form>
              <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
              <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
              <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
              <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
          </form>
          <script language = "javascript">
              document.write("Dimodifikasi terakhir pada " +
              document.lastModified);
          </script>
  </body>
  </html>

![Screenshot 2024-11-04 122319](https://github.com/user-attachments/assets/f5be29dc-7c28-4dd0-aba8-767e283b312a)
![Screenshot 2024-11-04 122326](https://github.com/user-attachments/assets/d46773d9-5808-4677-b825-3659cf77ae8f)
![Screenshot 2024-11-04 122348](https://github.com/user-attachments/assets/4e45fd26-66f0-4a40-ac87-9d1675d0eef7)
![Screenshot 2024-11-04 122356](https://github.com/user-attachments/assets/ec57a604-07dc-42ae-8acb-671589eb25ad)
![Screenshot 2024-11-04 122404](https://github.com/user-attachments/assets/ca796c6d-cf6d-4c95-b2ff-e643651072bb)

Kode ini menyediakan tombol untuk mengganti warna latar belakang dan warna teks pada halaman. Fungsi ubahWarnaLB digunakan untuk mengubah warna latar belakang (bgColor), sedangkan fungsi ubahWarnaLD digunakan untuk mengubah warna teks (fgColor). Tombol yang tersedia memungkinkan pengguna untuk memilih warna latar belakang hijau atau putih serta warna teks kuning atau biru. Di bagian bawah halaman, document.write menampilkan informasi tentang terakhir kali halaman dimodifikasi menggunakan document.lastModified.

11. HTML DOM

  <!--
  File: daftar_menu.html
  -->
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
                  if (total > 0)
                      total -= parseInt(harga);
              }
  
              document.getElementById('total').value = total;
          }
      </script>
  </head>
  <body>
      <h1>Daftar Menu Makanan</h1>
      <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"> Ayam Goreng Rp. 5.000</label><br />
      <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);"> Tempe Goreng Rp. 500</label><br />
      <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);"> Telur Dadar Rp. 2.500</label><hr />
      <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
  </body>
  </html>

  ![Screenshot 2024-11-04 122456](https://github.com/user-attachments/assets/445e729f-9fec-425c-84fe-ebfb43cec88f)

  Kode ini menampilkan daftar menu makanan dengan checkbox untuk memilih item dan menghitung total harga. Fungsi hitung akan menambah atau mengurangi harga dari item yang dipilih atau dibatalkan, kemudian memperbarui nilai total di kotak input total. Setiap checkbox memiliki nilai harga sesuai dengan itemnya, dan saat dipilih, total harga akan diperbarui secara langsung di halaman.

Pertanyaan dan Tugas

1. Buat script untuk melakukan validasi pada isian form.

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Validasi Form</title>
        <script>
            function validateForm() {
                // Mengambil nilai dari input
                var name = document.forms["myForm"]["name"].value;
                var email = document.forms["myForm"]["email"].value;
                var phone = document.forms["myForm"]["phone"].value;
    
            // Validasi Nama
            if (name === "") {
                alert("Nama harus diisi.");
                return false;
            }
    
            // Validasi Email
            var emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/; // Regex untuk validasi email
            if (email === "") {
                alert("Email harus diisi.");
                return false;
            } else if (!emailPattern.test(email)) {
                alert("Email tidak valid.");
                return false;
            }
    
            // Validasi Nomor Telepon
            var phonePattern = /^[0-9]+$/; // Regex untuk validasi nomor telepon
            if (phone === "") {
                alert("Nomor telepon harus diisi.");
                return false;
            } else if (!phonePattern.test(phone)) {
                alert("Nomor telepon hanya boleh berupa angka.");
                return false;
            }
    
            // Jika semua validasi berhasil
            alert("Form berhasil dikirim!");
            return true; // Mengizinkan form untuk disubmit
        }
    </script>
    </head>
    <body>
        <h1>Formulir Pendaftaran Lomba Informatika 2024 </h1>
        <form name="myForm" onsubmit="return validateForm()">
            <label for="name">Nama:</label><br>
            <input type="text" name="name"><br><br>
            
        <label for="email">Email:</label><br>
        <input type="text" name="email"><br><br>
        
        <label for="phone">Nomor Telepon:</label><br>
        <input type="text" name="phone"><br><br>
        
        <input type="submit" value="Kirim">
    </form>
    </body>
    </html>

   ![Screenshot 2024-11-04 122618](https://github.com/user-attachments/assets/e60acb6f-7df8-4ada-9341-90ae752d4617)
   ![Screenshot 2024-11-04 122634](https://github.com/user-attachments/assets/a3d6f685-183a-4ca3-a735-7b405ba00247)

   Fungsi validateForm(): Fungsi ini dijalankan saat form disubmit. Ia mengambil nilai dari input dan melakukan validasi. Validasi Nama: Memastikan bahwa kolom nama tidak kosong. Validasi Email: Memastikan kolom email tidak kosong dan memenuhi pola email yang benar menggunakan regular expression (regex). Validasi Nomor Telepon: Memastikan kolom nomor telepon tidak kosong dan hanya berisi angka. Menggunakan alert: Jika ada kesalahan dalam input, pengguna akan diberi tahu melalui pesan alert. Mengizinkan atau Mencegah Pengiriman Form: Jika semua validasi berhasil, form akan disubmit; jika tidak, pengiriman akan dibatalkan.
