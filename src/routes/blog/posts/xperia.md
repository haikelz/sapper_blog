---
author: Haikel
title: Oprek Xperia Miro
date: 08-20-2021
description: Mencoba mengoprek hp lama saya
---

Mencoba mengoprek hp lama saya

<!-- more -->

## Table of Contents
<!-- vim-markdown-toc GFM -->

* [A. Pendahuluan](#a-pendahuluan)
* [B. Proses](#b-proses)
* [C. Penutup](#c-penutup)

<!-- vim-markdown-toc -->

# A. Pendahuluan

Seperti yang kita tau, Xperia Miro ini adalah salah satu produk yang dirilis oleh Sony sekitar tahun 2012. Di tahun 2021 ini, hp ini bisa dikatakan sudah ketinggalan jaman. Beberapa orang menjadikannya koleksi. Tapi apakah kita bisa menjadikan hp ini lebih enak dipakai? Walau paling hanya sekedar untuk dengar musik? Tentu saja bisa, salah satunya dengan cara oprek. Dan kali ini, saya akan membagikan bagaimana caranya.

# B. Proses

**DISCLAIMER!** Saya tidak bertanggung jawab apabila muncul masalah di hp kalian, karena saya juga melakukan ini dengan resiko. So, lakukan dengan bijak dan penuh kesadaran oke.

![](https://i.ibb.co/XWNX6jd/sony2.jpg)

1. **Pertama-tama,** kita perlu untuk UBL. Untuk caranya, bisa dilihat [disini](https://developer.sony.com/develop/open-devices/get-started/unlock-bootloader/how-to-unlock-bootloader/). Prosesnya sama seperti hp Sony lain. Menurut saya sendiri, UBL hp Sony ini justru lebih mudah ketimbang hp lain karena hanya berbekal IMEI, dan Unlock Code nya saja.

2. **Kalo sudah UBL, maka kita akan mencoba root.** Untuk proses ini silahkan download kingroot atau pakai saja superuser bawaan(biasanya sudah disediakan di firmware 11.0.A.5.5, saran saya coba cek dulu versi firmwarenya).

3. **Pasang TWRP.** Untuk link download TWRP, ada [disini](https://forum.xda-developers.com/attachments/twrp_miro-zip.1702672/).  Cara pasangnya:

   - Ekstrak ZIP nya
   - Sambungkan hp kalian ke PC/Laptop, dan hidupkan mode debugging USB.
   - Pilih install.bat dalam folder TWRP tadi, atau install.sh untuk linux(saran saya pakai windows aja karena kita akan memakai Flashtool). Tunggu hingga prosesnya selesai.
   - Untuk mengecek apakah TWRP sudah benar-benar terpasang, silahkan kalian matikan hp nya, dan hidupkan lagi sambil menekan tombol volume bawah(-) berkali-kali sampai muncul tulisan TWRP.

4. **Custom kernel, dan ROM**
   Link download ROM Gimlo, kernel vengeance, dan flashtool ada [disini](https://www.mediafire.com/folder/eoelo8ibguw1y/Documents)

# C. Penutup

Okeh mungkin sampai disini saja. Maaf saya tidak bisa menjelaskan cara pasang cusrom dan kernelnya karena saya gak sempat foto prosesnya.
Kalian bisa eksplorasi sendiri. Sebenarnya sama aja sih seperti kebanyakan hp. Untuk cusrom tinggal install via TWRP, ganti kernel via flashtool dengan keadaan hp dalam mode fastboot.

Terima Kasih :)


