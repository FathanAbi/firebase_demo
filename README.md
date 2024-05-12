# Firebase-Flutter tutrorial

## 1. install firebase
bisa menggunakan npm, yarn, atau exe file

contoh menggunaka npm:
``` shell
npm install -g firebase-tools
```

![ss terminal](<Screenshot 2024-05-11 105919.png>)

## 2. login firebase
pastikan telah membuat akun di website firebase login. kemudian jalankan firebase login pada terminal.

``` shell
firebase login
```

![ss terminal](<Screenshot 2024-05-11 110008.png>)

## 3. tambahkan pub ke environment variable
![alt text](<Screenshot 2024-05-11 110511.png>)

## 4. Install flutterfire
```shell
dart pub global activate flutterfire_cli
```

![alt text](<Screenshot 2024-05-11 110405.png>)

## 5. buat project baru di flutter
buat project baru di flutter seperti biasa
![alt text](<Screenshot 2024-05-11 110955.png>)

## 6. buat project baru di website firebase
![alt text](<Screenshot 2024-05-11 112638.png>)

## 7. add firebase_core
```shell
flutter pub add firebase_core
```
![alt text](<Screenshot 2024-05-11 112331.png>)

## 8. konfigurasi flutterfire
```shell
flutterfire configure
```
![alt text](<Screenshot 2024-05-11 112834.png>)

pilih project yang baru dibuat

## 9. edit main.dart
![alt text](<Screenshot 2024-05-11 113716.png>)

## 10. pada android/app/build.graddle
tambahakan
``` gradle
android {
    defaultConfig {
        ...
        multiDexEnabled true
    }
}

dependencies {
    implementation 'androidx.multidex:multidex:2.0.1'
}
```

## 11. konfigrasi firestore database
pada website project firebase pergi ke build lalu ke firestore database. kemudian buat database. pada tab rules ubah read and write ,emjadi true

![alt text](<Screenshot 2024-05-12 125413.png>)

kemudian add cloud_firestore
```shell
flutter pub add cloud_firestore
```
