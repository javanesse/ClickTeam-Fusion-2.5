# ClickTeam Fusion 2.5

# Alternatif dari
https://steamcommunity.com/sharedfiles/filedetails/?id=914599868

# Cara Export APK menggunakan ClickTeam Fusion
1. install clickteam
2. install JDK (saat ini yang terbaru adalah java SE Development Kit 12.0.1) 64Bit
3. Buat aplikasi test dalam bentuk OUYA aplication
4. save aplikasi
5. Build/export aplikasi menjadi APK
6. jika di minta  select directory of Java SDK, lokasikan, biasanya di (C:\Program Files\Java\jdk-12.0.1)
7. maka akan mendapati errorlog, dimana akan kelihatan error apa saja saat build
```
> Failed to install the following Android SDK packages as some licences have not been accepted.
     platforms;android-26 Android SDK Platform 26
     build-tools;28.0.3 Android SDK Build-Tools 28.0.3
  To build this project, accept the SDK license agreements and install the missing components using the Android Studio SDK Manager.
  Alternatively, to transfer the license agreements from one workstation to another, see http://d.android.com/r/studio-ui/export-licenses.html
```

8. download dan install Android SDK lama (google Drive) pilih everyone, saat choose users (C:\Program Files (x86)\Android\android-sdk), buka dan jalankan
9. kemudian lihat error di atas, di tambah dengan sedikit tambahan untuk driver usb misalnya, maka pilih saat install
	- Tools - Android SDK Tools
	- Tools - Android SDK Build-Tools 28.0.3
	- Android 8.0.0 (API 26) - SDK Platform
	- Android 8.0.0 (API 26) - Sources for Android SDK
	- Extras - Google Play Services
	- Extras - Google USB Driver
10. install(download) sampai selesai
11. di aplikasi clickteam, buka tools, preferences, general
 pada exporter android, lokasikan instalasi android sdk yang baru saja di install (C:\Program Files (x86)\Android\android-sdk)
12. restart komputer
13. coba build kembali
