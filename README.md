# BELUM (KHUSUS HP)

# Peringtan

Segala resiko diluar tanggung jawab saya

## Bahan

[Termux](https://play.google.com/store/apps/details?id=com.termux&hl=id)

[Code Editor](https://play.google.com/store/apps/details?id=com.rhmsoft.code&hl=id&gl=US)

[Kiwi Browser](https://play.google.com/store/apps/details?id=com.kiwibrowser.browser&hl=id)

[Blumtod](https://github.com/akasakaid/blumtod/tree/main) (download nanti)

## Tutorial

### Download semua bahannya untuk Handphone

### Cek repo termux dengan cara

masukan command 

```
termux-change-repo
```
Klik OK > OK Saja
Setelah itu masukan command

```
apt-get upgrade
apt-get update
```

### Install Python

```
pkg install python
```

### Install github

```
pkg install github
```

### Membuat Folder Baru Di Internal Memory HP

caranya ya tinggal ke file manajer bikin folder baru aja
contoh disini saya bikin folder namanya "belum"

### Masuk ke folder yang sudah dibikin tadi di internal hp

```
cd /storage/emulated/0/belum
```

### Copy github blumtod

```
git clone https://github.com/akasakaid/blumtod.git
```

setelah itu dicek terlebih dahulu apa sudah ada foldernya dengan ketik command

```
dir
```

jika sudah muncul lanjut ke next step

### Open folder yg sudah didownload melalui termux

```
cd blumtod
```

catatan untuk hp : jika termux sudah dikeluarkan dan ingin masuk folder langsung maka perintahnya

```
cd /storage/emulated/0/belum/blumtod
```

### Install Requirements

```
python -m pip install -r requirements.txt
```

### Edit config.json

Edit config.json dengan app code editor agar mudah
Buka code editor yang sudah diinstall dan open cari file config.json di folder blumtod

• Edit  *config.json* file

```env
    "interval": 3,                # Berfungsi untuk nilai jeda antara akun
    "auto_complete_task": false,  # Berfungsi untuk menyelesaikan task
                                    true = On / false = Off
    "auto_play_game": false,      # Berfungsi untuk auto play game tiket
                                    true = On / false = Off
    "game_point":                 # Mengatur hasil score tiap sekali permainan
        "low": 240,
        "high": 250
```

### Edit data.txt

Edit data.txt dengan app code editor agar mudah
Buka code editor yang sudah diinstall dan open cari file data.txt di folder blumtod

• Edit  *data.txt* file

```env
   diisikan dengan query telegram bot blum bisa multi akun
  contoh :
  query= .........
  query= .........
  user= .........
```

• Cara mendapatkan query

1. Buka kiwi browser
2. Download extension [Ignore X-Frame headers](https://chromewebstore.google.com/detail/ignore-x-frame-headers/gleekbfjekiniecknbkamfmkohkpodhe) dan [Violentmonkey](https://chromewebstore.google.com/detail/violentmonkey/jinjaccalgkegednnccohejagnlnfdag)
3. Buka web Telegram dan login
4. Buka Blum App sampai muncul Blum nya
5. Buka "Developer tools" dengan mode "desktop site" di bagian opsi titik 3 kanan atas
6. Pilih tab "Application" di pada devtools
7. Pilih "Session Storage" di sebelah kiri
8. Pilih "telegram.blum.codes"
9. Dan cari "tgWebAppData" di sebelah kanan dan ada tulisan "query_id......" dan klik
10. Lihat paling bawah ada tulisan warna merah dan tulisan "query_id..."
11. Tekan dan tahan sampai muncul opsi
12. Pilih "Copy Value"
13. Paste ke "data.txt" di folder blumtod tadi


### Run Bot

```
python bot.py
```

### Credit & Thx

[Termux]
[Code Editor]
[Kiwi Browser]
[akasakaid](https://github.com/akasakaid)
