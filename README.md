# GomuluSistemProje
Remote Control project by an Android app for raspberry pi 4 model
(Android mobil uygulama tabanlı uzaktan kontrol projesi)
<img align="right" src="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/smart%20tech.jpg">
Projenin adım adım yapılışını [Sunum](https://drive.google.com/file/d/1E2f2XrrP8_0pYNAL4NVeHentCClqI8yb/view?usp=sharing) 'inde, 
sadece uygulama videosunu [Video Link](https://drive.google.com/file/d/1-JU1hBfqBnj6zNEEH2qz8ftxPbXCcGVn/view?usp=sharing) 'inde bulabilirsiniz.

## Project Requirements -(Proje Gereksinimleri)
  ### Hardware(Donanım)
     1-Raspberry Pi 4B
     2-Android Phone(Android Telefon) 
     3-Breadboard(Devre Tahtası)
     4-Resistor(Direnç)
     5-Led
     6-Powerbank(Taşınabilir güç ünitesi)
     7-Connection cables(Bağlantı için gerekli kablolar)
  ### Software(Yazılım) 
     1.Diet Pi OS (Diet Pi İşletim Sistemi)
     2.Blynk App
     
 ## Benefits and Target-(Projenin Faydaları ve Hedefi)
    1. Improving Energy Efficiency(Enerji verimliliğini arttırmak)
    2. Ensuring Accessibility(Erişilebilirliği ve mobiliteyi sağlamak)
    3. Make savings for money and energy (Enerji ve para tasarrrufu)
## Raspberry Pi 4B
1.5 GHz 4 Cores ARM Cortex-A72 CPU
2GB LPDDR4 RAM SKU | 
VideoCore VI Graphics
4kp60 HEVC video
Gigabit Ethernet
2 × USB 3.0 ve 2 × USB 2.0 Ports
2 × mikro HDMI (1 × 4K@60Hz & 2 × 4K@30Hz) 
<img align=src="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/raspberry%20pi%204B.jpg">

## Diet Pi OS
You can download from this link to install your raspberry(Diet Pi işletim sistemini bu linkten indirebilirsiniz)[Link](https://dietpi.com/downloads/images/DietPi_RPi-ARMv6-Buster.7z)
<img align=src="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/diet%20pi.PNG">
## Blynk App
You can download from this link to install your raspberry(Blynk uygulamasını bu linkten indirebilirsiniz)[Link](https://play.google.com/store/apps/details?id=cc.blynk&hl=en)
<img align=src="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Blynk%20Server.png">

## How is it work? (Nasıl Çalışır?)
1.Blynk application receives inputs from the user(Blynk uygulaması kullanıcıdan gelen inputları alır)
2.Received inputs are sent to Blynk servers(Alınan inputlar Blynk serverlarına gönderilir)
3.Raspberry Pi interprets the inputs that it receives from the Blynk server and transmits it to gpio pins(Rasberry Pi ,Blynk server'ından aldığı inputları yorumlar ve gpio çılışlarına iletir)
4.Gpio transmits the incoming information to the circuit board and the led lights up(Gpio gelen bilgileri devre tahtasına iletir ve led şık yanar)
<img align=src="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/how%20is%20it%20work..PNG">

## Codes (Kodlar)

1.Use below codes to update Diot OS version(Diet OS güncellemek için aşağıdaki kod yazılır)
### curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -

2.Install or update codes for Blynk app libraries (Blynk uygulamasının kütüphanelerinin indirilmesi ve kurulumu)
### sudo apt-get update && sudo apt-get upgrade
### sudo apt-get install build-essential nodejs -y
### sudo npm install blynk-library -g
### sudo npm install onoff -g

3.Install Blynk app from Play Market to android device(Play Market’ten Blynk uygulaması kumanda edecek telefona yüklenir)
<img align=src="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Play%20store.png">

4.Login to BLynk app(Uygulama üzerinde kullanıcı adı /şifre ile kayıt olunur)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Blynk%20Login.jpg">

5.Get token from Blynk app to connect raspberry pi (Uygulamanın,kayıt olunan mail hesabına Rasberry Pi ile eşleşme yapılması için token gönderimi)
### blynk-client YourAuthToken
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Connecting%20%20app%20to%20raspberry%20pi.jpg">

6.The token that prvided by Blynk (Blynk uygulamasından gelen mail ve token)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Blynk%20Authentication%20Code.jpg">

7.Pairing android device with raspberry pi (Rasberry Pi üzerinde eşlemenin tamamlanması)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/connected.png">

8.Open project on Blynk (Blynk uygulamasından yeni proje seçimi)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Blynk%20New%20Project.jpg">

9.Choose embedded model (Blynk uygulamasından donanım modeli ve versiyonunun seçilmesi)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Blynk%20choosing%20embedded%20model.jpg">

10.Choose output gpio(Donanım üzerinde led devresine bağlı portların seçilmesi)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/Blynk%20choosing%20gpio.jpg">

12.Finalize design and test your circuit (Uygulama arayüz tasarımının tamamlanması ve test işlemi)
<img align="https://github.com/fthkok/GomuluSistemProje/blob/master/Pictures/bread%20board.png">




