# Modul 10 (Timer)

![img.png](img.png)

Dari gambar di atas, terlihat bahwa pesan Nobel's Computer: outside spawn adalah pesan pertama yang dicetak, kemudian diikuti oleh pesan Nobel's Computer: howdy! dan setelah 2 detik, muncul pesan Nobel's Computer: done!. Hal ini terjadi karena pesan howdy! dan done! merupakan future yang hanya akan dijalankan saat executor dieksekusi. Sementara itu, perintah print untuk pesan outside spawn berada tepat setelah pemanggilan spawner.spawn(...) dan sebelum executor.run(), sehingga perintah tersebut dieksekusi terlebih dahulu dibandingkan dengan print untuk howdy! dan done!.