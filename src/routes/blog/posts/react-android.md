---
author: Haikel
date: 01-29-2022
description: Ngoding react di Android? Kenapa tidak?
title: Setup react di Android
---

Ngoding react di Android? Kenapa tidak?

<!-- more -->

Jadi, saya iseng pengen setup ngoding react di android. Mumpung di hpnya juga udah saya install termux, jadi saya coba dah tu. Eh berhasil rupanya:D, jadi saya dokumentasikan ke sini aja biar ga nyari kemana-mana lagi.

**Note: Tidak memerlukan root, jadi jangan khawatir.**

Tahapan:

- Install Termux. Sebagai informasi, Termux yang ada di PlayStore itu sudah ga update lagi. Jadi silahkan download di [f-droid](https://f-droid.org/en/packages/com.termux/). Biasanya kalo masih pake versi lama, bakal ada pemberitahuannya.
- Setelah menginstall Termux, kemudian install `nodejs` via termux dengan perintah `pkg install nodejs`.
- Siapkan text editor. Terserah mau pake apaan, tapi disini saya pake neovim dengan konfigurasi [nvchad](https://github.com/NvChad/NvChad).
- Sama seperti biasanya, untuk membuat `react-app`, kita bisa memasukkan perintah:

  ```shell
  npx create-react-app namaProject
  ```

  ![react](https://i.ibb.co/vqZ7wsJ/Screenshot-20220129-103808.png)

- Untuk preview di browser, tinggal ketik `npm run start` di direktori projectnya, nanti dia otomatis mengarahkan kita ke `localhost` untuk previewnya.

  ![localhost](https://i.ibb.co/4YTMHZw/Screenshot-20220120-213322.png)
  
- Selesai.
