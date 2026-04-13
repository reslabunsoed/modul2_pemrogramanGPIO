# Modul 2: Pemrograman GPIO

## 🎯 Tujuan Praktikum

Berikut ini adalah tujuan praktikum pada Modul Praktikum 2:
- Membuat program dengan teknik loop dalam arduino untuk control input dan output pin arduino
- Merangkai rangkaian input dan output dengan arduino.
- Mengendalikan LED dalam Seven Segment dan penggunaan Push Button

## 📄 Dasar Teori

GPIO (General Purpose Input/Output) adalah salah satu fitur penting dalam pengembangan proyek elektronik dan pemrograman mikrokontroler. Pada Arduino, fungsi GPIO memungkinkan pengguna untuk melakukan interaksi langsung dengan lingkungan sekitar, seperti membaca data dari sensor, mengoperasikan motor maupun menyalakan LED. GPIO adalah pin pada mikrokontroler atau komputer papan tunggal (seperti Raspberry Pi) yang dapat dikonfigurasi sebagai input atau output sesuai kebutuhan pengguna. Pin-pin ini tidak memiliki fungsi khusus bawaan, sehingga disebut "general purpose" (serbaguna).

Pada mikrokontroler Arduino berbasis ATmega, setiap pin secara default berada dalam mode input setelah sistem dinyalakan. Oleh karena itu, tidak selalu diperlukan pemanggilan fungsi pinMode() untuk menetapkannya sebagai input.

Pada tahap ini, kita mulai menyalakan LED menggunakan program dengan memberikan logika HIGH (5V) pada `pin 11`. Selanjutnya, program tersebut akan diubah sehingga LED tidak hanya menyala terus, tetapi juga dapat berkedip. Untuk itu, kita perlu memahami konsep keluaran digital pada Arduino.

Arduino Uno memiliki 20 pin GPIO yang dapat digunakan untuk menerima atau mengirim sinyal digital, yaitu HIGH dan LOW. Sinyal ini dikendalikan melalui fungsi `digitalRead()` untuk membaca dan `digitalWrite()` untuk menulis nilai digital.

Walaupun pin digital lain juga bisa digunakan, Pin 11 dipilih agar konsisten dengan pelajaran selanjutnya, sehingga proses belajar menjadi lebih sederhana dan tidak membingungkan

<img width="2615" height="1338" alt="ArduinoUno_DigitalIOPins" src="https://github.com/user-attachments/assets/b460b772-82aa-4df9-8a62-fa67c5d66a80" />

Anda dapat mengendalikan salah satu dari 20 pin digital I/O tersebut dengan menggunakan tiga fungsi berikut:

- `pinMode(int pin, int mode)`. Fungsi ini digunakan untuk mengatur sebuah pin agar berfungsi sebagai INPUT atau OUTPUT. Dalam kasus ini, kita memilih OUTPUT karena kita ingin mengirimkan sinyal untuk menyalakan LED.
- `digitalRead(int pin)`. Fungsi ini digunakan untuk membaca sinyal digital dari pin tertentu, yaitu HIGH atau LOW. Fungsi digitalRead akan dibahas lebih lanjut pada seri pelajaran pengantar input.
- `digitalWrite(int pin, int value)`. Fungsi ini digunakan untuk mengirimkan sinyal digital ke pin tertentu, yaitu HIGH atau LOW. Pada pelajaran ini, kita akan menggunakan fungsi `digitalWrite`.

<h2>Bagaimana kita menghitung 20 pin I/O digital?</h2>

Pada Arduino Uno dan Leonardo, tulisan dan label pada papan sering membuat kita mengira hanya ada 14 pin digital. Padahal, jika dilihat secara keseluruhan, terdapat 20 pin digital I/O yang bisa digunakan. Untuk memastikan hal ini, kita dapat melihat diagram pinout resmi Arduino Uno yang menunjukkan semua pin yang tersedia.

<img width="2621" height="1418" alt="ArduinoUno_OfficialPinOutDiagram" src="https://github.com/user-attachments/assets/bd663b67-2c34-41ea-a147-6d8df3e1695d" />

Untuk lebih jelasnya, berikut pin I/O digtial dan analog

<img width="2607" height="1419" alt="ArduinoUno_OfficialPinOutDiagram_DigitalIOPinsMarked" src="https://github.com/user-attachments/assets/9df3cb76-7db3-499b-802b-98996772aa8c" />

<h2></h2>

<br>

![banner](https://github.com/user-attachments/assets/f1f03032-41c0-4121-94e3-df1d513b42e5)
