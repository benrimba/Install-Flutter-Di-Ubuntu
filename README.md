# InstallAndroidStudiodanFlutter
Setelah menginstall Git, download Flutter SDK pada website resminya https://flutter.dev/docs/get-started/install/linux.

Ekstrak file yang sudah didownload, misal file yang didownload tadi berada di folder Downloads ingin diekstrak ke directory Home, buka terminal (CTRL+ALT+T) dan jalankan perintah.
	
```py 
cd ~/Downloads
```
```py	
tar xf flutter_linux_1.17.5-stable.tar.xz --directory /home/$USER/
```
Tambahkan flutter ke dalam path. Buka file .bashrc.
```py	
nano ~/.bashrc
```
Lalu tambahkan baris berikut paling bawah.
```py	
export PATH="$PATH:/home/$USER/flutter/bin"
```
Atau bisa juga dengan cara membuka file .bashrc pada File Manager dan tekan CTRL+H lalu buka .bashrc dengan text editor dan tambahkan kode path tadi pada baris paling bawah.

Reload konfiguasi atau restart terminal.
```py	
source ~/.bashrc
```
Verifikasi penginstallan flutter dengan menjalankan.
```py	
flutter doctor
```
Jika penginstallan berhasil akan tampil seperti ini.
```py
Doctor summary (to see all details, run flutter doctor -v):
[✓] Flutter (Channel stable, v1.17.5+hotfix.9, on Linux, locale en_US.UTF-8)
[✗] Android toolchain – develop for Android devices
✗ ANDROID_HOME = /home/atm/Android/Sdk
but Android SDK not found at this location.
[!] Android Studio (not installed)
[!] Connected device
! No devices available! Doctor found issues in 3 categories.
```
