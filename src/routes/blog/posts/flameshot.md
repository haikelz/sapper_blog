---
author: Haikel
date: 12-31-2021
description: Flameshot bisa dijadikan pilihan selain scrot
title: Menggunakan Flameshot Untuk Screenshot
---

Jika bosan dengan scrot, bisa mencoba flameshot

<!-- more -->

## Table of Contents

<!-- vim-markdown-toc GFM -->

* [A. Pendahuluan](#a-pendahuluan)
* [B. Proses](#b-proses)
* [C. Kustomisasi](#c-kustomisasi)
* [D. Shortcut Keyboard](#d-shortcut-keyboard)
* [E. Referensi](#e-referensi)

<!-- vim-markdown-toc -->

# A. Pendahuluan

Jadi selama ini saya menggunakan scrot untuk screenshot. Memang simple, tapi jika ingin menghiasnya, saya mesti bolak balik ke [Screely](https://screely.com). Nah kebetulan saya ketemu tulisannya Om [Bandithijo](https://bandithijo.github.io) tentang bagaimana mengambil screenshot dan menghiasnya langsung tanpa bolak-balik ke Screely.

Aslinya, scriptnya pake Ruby, cuma saya ngambil yang udah diporting ke Bash oleh [Om Berrabe](https://github.com/berabee). Terima kasih Om Bandithijo dan Om Berrabe udah berbagi tips dan triknya.

# B. Proses

- Pertama-tama, install flameshotnya terlebih dahulu, sesuaikan dengan distro yang dipakai.

  ```bash
  sudo pacman -S flameshot
  ```

- Setelah terinstall, ada dua opsi dalam scriptnya, yakni memakai script original yang berbahasa ruby dari Om Bandithijo, atau yang sudah diporting ke bash. Disini saya pilih yang bash aja.

  ```bash
  wget https://raw.githubusercontent.com/berrabe/awesome-flameshot/master/awesome-flameshot
  ```

- Jangan lupa buat scriptnya jadi executable dengan:

  ```bash
  chmod +x awesome-flameshot
  ```

- Jika ingin menjalankannya, cukup dengan `./awesome-flameshot`

# C. Kustomisasi

Untuk mengganti icon, font, dan letak directory penyimpanan screenshot, tinggal kalian edit aja scriptnya.

![Flameshot](https://i.ibb.co/yW6fbG6/flameshot.png)

Ada 4 hal penting yang saya ubah:

- No.1 Menunjukkan tempat menyimpan screenshot. Nah nanti hasil screenshotnya akan ada dua, yakni hasil aslinya dan hasil yang telah diedit.
- No.2 Adalah warna backgroundnya. Defaultnya warna putih, ganti sesuai keinginan.
- No.3 Menunjukkan nama user, tanggal, dan waktu. Disini saya cuma ganti icon untuk usernya aja.
- No.4 Adalah jenis font yang dipakai.

Untuk bagian yang lain, saya belum ngulik lagi hehe. Soalnya mengubah 4 hal tadi udah dirasa cukup bagi saya.

# D. Shortcut Keyboard

Daripada ribet mesti buka terminal buat jalaninnya, saya menambahkan shortcut keyboard ke `sxhkdrc`. Disini saya pake bspwm.

![sxhkdrc](https://i.ibb.co/wc6BVG2/sxhkdrc-edited.png)

# E. Referensi

- [Om Bandithijo](https://bandithijo.github.io/blog/memodifikasi-screenshot-dari-flameshot-dengan-imagemagick)
- [Om Berrabe](https://github.com/berrabe/awesome-flameshot)
- [Website Flameshot](https://flameshot.org/)
