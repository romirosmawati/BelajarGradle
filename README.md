# BelajarGradle
Pekerjaan rumah 16 | Module 18 Membuat Project Gradle dengan kriteria sebagai berikut:
1. buat tugas Gradle sederhana untuk menerima parameter CLI dan mencetaknya dengan pesan ucapan
2. Proyek skrip Gradle harus dibuat di repositori yang berbeda dan push ke GitHub. Detail:
- Proyek Gradle baru ada atas perintah "gradle init --type java-library" dengan struktur direktori dan file nama "build.gradle" root.
- Menjalankan perintah berikut: "./gradlew greetingTask -Pname=YourName" pada Terminal.
- Menambahkan dependensi bawaan Gradle.
- Melakukan tambahkan dependencies dan code ke file "build.gradle" seperti dibawah ini
task greetingTask() {
 doLast {
String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User' println "Hello, $nama! Welcome to Gradle World!"
}

}
- Untuk menjalankan tugas dengan menjalankan perintah berikut: "./gradlew greetingTask -Pname=YourName"
- Dependencies yang digubakan dalam project ini yaitu JUnit 5.10.0 dan JUnit Jupiter
- run Project pada terminal dengan cara : "./gradlew greetingTask -Pname=RomiR"
- Hasil capture project dapat dilihat pada link berikut
