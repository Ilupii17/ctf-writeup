## **Details**
- Author : aimardcr
- Deskripsi : You were just enjoying watching your favorite VTubers, while suddenly the FBI breached into your room because they have found out that you have an outstanding still in Open Source Intelligence. They need your help to recover an image that is taken by a threat actor who recently hacked their National Data Center, one of the FBI's intel managed to get a picture of the hacker by hacking into his/her phone but that's all they can get. Unfortunately the picture really didn't give much information as they thought. Can you analyze the image further? The intel said that the picture could be a clue where the hacker hides. Some might say it's full of paradise.
---

## How To Solve ?
Yang pertama kita di berikan sebuah file gambar seperti di bawah ini

![Preview](images/1.png)

gambarnya tidak menujukan petunjuk apapun

dikarenakan ini challenge osint maka langkah pertama yang kita harus cek yaitu `metadata` menggunakan tools `exiftools`
metadata ini biasa terekam jika file gambar ini masih asli dari foto (tanpa harus di kirim lewat manapun, proses pengiriman biasanya menghapus metadata)

![Preview](images/2.png)

sekarang kita cek hasil metadatanya sampai bawah hingga aku menemukan petunjuk baru di metadata tersebut

![Preview](images/3.png)

kita bisa mendapatkan gps latitude dan Longitude ketika foto tersebut di potret dalam keadaan gps on

maka kita bisa konversikan saja menggunakan chat gpt wkwk, untuk mendapatkan link gmaps nya

![Preview](images/4.png)

langsung saja cari di gmaps 

![Preview](images/5.png)

maka langsung saja tulis format flagnya seperti di deskripsi
`INTECHFEST{JimbaranBayBeachResort&Spa}`

![Preview](images/6.png)
