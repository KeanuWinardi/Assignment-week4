1. membuat sebuah folder kosong dengan **namamu sendiri**. **mkdir keanu**
2. membuat sebuah file di dalam folder tersebut dengan nama `README.md`, isi file tersebut dengan kalimat<br>`"Halo perkenalkan aku halaman utama"`. **echo "Halo perkenalkan aku halaman utama" > README.md**
3. **inisialisasi** folder tersebut dengan Git, kemudian simpan perubahan menggunakan `commit` dengan pesan<br>`"First commit"`. **git add README.md** 
**git commit -m "First commit"** 
4. Ganti teks sebelumnya dengan `"Hello world". **echo "Hello world" > README.md**
5. Tampilkan isi teks tersebut pada command line menggunakan command `cat`. **cat README.md**
6. Ternyata kamu tidak ingin perubahan tersebut, dan ingin kembali ke perubahan seperti commit yang terakhir. Lakukan teknik git backtracking untuk mengembalikan ke perubahan commit yang terakhir. **git checkout README.md**
7. buat `branch` baru dengan nama `cv`, hal ini berguna agar histori kita tidak tercampur. **git branch cv**
8. pindah `branch` ke dalam `cv`, kemudian buat file dengan nama `cv.txt` dan isi file tersebut dengan kalimat:<br>`"Ini adalah file CV"`.
9. kemudian simpan perubahan menggunakan `commit` dengan pesan<br>`"Initial CV"`. **git add cv.txt**
 **git commit -m "Initial CV"**
10. tambahkan **3 perusahaan** yang akan kamu lamar, dan setiap menuliskan 1 nama perusahaan kamu harus melakukan dokumentasi dan menyimpan perubahan menggunakan `commit`.
**echo "" > PT.TELKOM.txt**
**git add PT.TELKOM.txt**
**git commit -m "perusahaan pertama"**
**echo "" > PT.PERTAMINA.txt**
**git add PT.PERTAMINA.txt**
**git commit -m "perusahaan kedua"**
**echo "" > PT.FREEPORT.txt**
**git add PT.FREEPORT.txt**
**git commit -m "perusahaan ketiga"**
11. kembali ke `branch master`. **git checkout main**
12. ubah file `README.md` menjadi
    ```
    Halo perkenalkan aku halaman utama

    Ini adalah update pertama pada branch master
    ```
    jangan lupa untuk menyimpan perubahan menggunakan `commit` dengan pesan<br>`"update master pertama"`. **echo 'Halo perkenalkan aku halaman utama ' ''  'Ini adalah update pertama pada branch master ' > README.md**
    **git commit -m "update master pertama"**

13. gabungkan branch `cv` ke dalam branch `master` menggunakan perintah `git merge`. **git merge cv**
14. unggah Git Repository project tersebut tersebut ke dalam GitHub. **git push origin main**
