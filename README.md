NAMA    : ALYA SEFHIA EKA PUTRI

KELAS   : TI.22.B1

NIM     : 312210108

# Contoh dan Penjelasan Modul Praktikum Pertemuan ke-13

1. Berikut adalah fungsi yang mengubah suhu dari derajat derajat Kelvin menjadi derajat Fahrenheit. Karena nol derajat derajat Kelvin sedingin yang didapat, fungsi tersebut ditebus jika melihat suhu negatif.

    ![1](https://user-images.githubusercontent.com/115520278/208279478-5fcea52a-dc83-416b-9c5d-02b1bbb46776.png)

   Ketika kode di atas dijalankan, muncul Exception yang bernama Traceback...
   ```AssertionError``` artinya terjadi error pada pernyataan assert.
   
2. Contoh ini untuk membuka file, menulis konten di file dan keluar dengan lancar karena tidak ada masalah sama sekali.

    ![2](https://user-images.githubusercontent.com/115520278/208279755-3508a445-99ba-4c90-9210-f990de60450e.png)

- Hasilnya :

      Written content in the file successfully
      
  Hasilnya seperti ini karena else akan dijalankan ketika try adalah True
  
3. Contoh ini mencoba membuka file di mana Anda tidak memiliki izin menulis, sehingga menimbulkan pengecualian.

   ![3](https://user-images.githubusercontent.com/115520278/208279835-94ce0f41-17c8-48be-930c-773e961f91b7.png)

- Mengapa hasilnya error?

  r adalah read - Membuka file untuk membaca, akan error jika file tidak ada. Disini ingin membaca file bukan menulis maka dibawahnya ```fh = open("testfile", "r")``` tambahkan ```print(fh.readline())``` dan fh.write dihapus. Setelah dijalankan, try dan else ditampilkan.
  
4. Contoh keempat

    ![4](https://user-images.githubusercontent.com/115520278/208279919-90b020d0-6dc6-4395-ad50-ec915a4156fd.png)

   Hasil diatas bukan error, karena finally dijalankan ketika try dan except dijalankan. Dan berhasil dibuat filenya setelah dijalankan.
   
5. Contoh single exception

    ![5](https://user-images.githubusercontent.com/115520278/208279963-61d5c290-b856-4af4-91d9-805f0d518525.png)
    
- Hasilnya :

      The argument does not contain numbers 
      invalid literal for int() with base 10: 'xyz'
      
   ketika dijalankan, maka muncul error. Hapus ```#!/usr/bin/python``` dan di ```except ValueError, Argument:``` ganti koma dengan as seperti ```except ValueError as Argument:```agar tidak error. Jika dijalankan akan muncul error lagi. Kenapa? karena parameter def temp_convert harus mengandung angka.
      
6. Contoh dan penjelasan keenam

    ![6](https://user-images.githubusercontent.com/115520278/208279989-e78135d9-6624-48e4-9752-58254c03219d.png)
    
    Jika dijalankan muncul SyntaxError artinya ada kesalahan sintaks. Pada raise ```"Invalid level!", level``` ganti tanda koma dengan tanda plus. Cetak def dengan angka yang lebih besar dari 1.
    
Selesai

