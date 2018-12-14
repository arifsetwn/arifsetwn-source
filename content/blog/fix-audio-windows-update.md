---
title: "Suara hilang setelah Windows Update"
date: 2018-12-14T22:11:17+07:00
draft: false
---
> Suara hilang setelah update Windows Build 18298

Saya menggunakan Windows Insider Preview dimana jika ada update dari microsoft maka perangkat saya akan mendapat prioritas untuk menginstall update tersebut. Pagi tadi ada notif untuk melakukan restart karena ada update terbaru dari Windows. Ternyata, Setelah melakukan update dengan kode build 18928, audio devices menjadi tidak terdeteksi. Alhasil laptop saya menjadi bisu. Saya cek di `Device Manager` ada devices baru dengan nama `IDT High Definition Audio CODEC` yang memiliki tanda kuning alias sedang bermasalah.

![](https://9yvkyg.sn.files.1drv.com/y4mYx3P1vWwui5t2TVjS24fdxcwfMgEisHmNnc2U46UZiW7ajElC-pTFTGoW9--X9WzdgwhoTZKNFuglL5iMlmxog8Yy7BTlHzA77RBqZrXNwHQPsnRS5H5z-XTovVmHhnupjwPh4nMMWqvwwlQ86ZzHrAwJnGtfBPvSiW5a0SYnaKOvQO1SiZKyuXYriy0N2ikv6ptFsxklnEUXeouWbNRMg/idt.PNG)



Solusi dari permasalahan ini ternyata cukup mudah. Klik kanan device tersebut kemudian pilih `Update Driver Software`. Kemudian klik `Browse my computer for driver software`. Klik lagi pilihan `Let me pickup a list of device drivers on my computer`. Kemudian pilih  `High Definition Audio Device` (Jangan pilih `IDT High Definition Audio CODEC`).

Dan masalah terselesaikan :)
