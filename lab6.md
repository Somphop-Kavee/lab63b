# การทดลองที่ 6 เรื่อง การเขียนโปรแกรมสร้างไวไฟแอคเซสพอยต์(Wifi AP)

## วัตถุประสงค์
1.เพื่อให้เข้าใจการเขียนโปรแกรมเพื่อสร้างไวไฟแอคเซสพอยต์


## อุปกรณ์ที่ใช้
1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
2. สาย USB
3. อุปกรณ์ต่อ USB
4. คอมพิวเตอร์


## ศึกษาข้อมูลเบื้องต้น
1. 06 run wifi AP https://youtu.be/T26DVHePlTs

## วิธีการทำการทดลอง
1. เสียบไมโครคอนโทรลเลอร์เข้ากับ serial port

![image](https://user-images.githubusercontent.com/80879728/112317179-60d2fb00-8cde-11eb-9495-d016f02b734a.png)

2. พิมพ์ vi src/main.cpp เพื่อดู sourecode ของ 06_Wifi-AP-Web-Server

![image](https://user-images.githubusercontent.com/80879728/112317507-b60f0c80-8cde-11eb-927a-932f94b07e3c.png)

![image](https://user-images.githubusercontent.com/80879728/112317651-d939bc00-8cde-11eb-984e-7b2c2994ace7.png)

![image](https://user-images.githubusercontent.com/80879728/112318432-9b896300-8cdf-11eb-807c-dfeab6b99186.png)

![image](https://user-images.githubusercontent.com/80879728/112318458-a217da80-8cdf-11eb-8f9b-11e56ec1c9a9.png)

3. พิมพ์ pio run -t upload และ กดปุ่มสีดำและสีแดง

![image](https://user-images.githubusercontent.com/80879728/112319256-76492480-8ce0-11eb-9140-ef29301f1863.png)

![image](https://user-images.githubusercontent.com/80879728/112319284-7cd79c00-8ce0-11eb-883e-894383869ed3.png)

![image](https://user-images.githubusercontent.com/80879728/112319482-b27c8500-8ce0-11eb-8755-8b7b09d56663.png)

![image](https://user-images.githubusercontent.com/80879728/112319493-b6100c00-8ce0-11eb-8c0a-8cc13e953312.png)

4. พิมพ์ pio device monitor

![image](https://user-images.githubusercontent.com/80879728/112319815-038c7900-8ce1-11eb-81aa-c79207892a3d.png)

## การบันทึกผลการทดลอง
ขึ้น WIFI ชื่อ HI_BMFWIFI_2.4G ในโทรศัพท์

## อภิปรายผลการทดลอง
WIFI ชื่อ HI_BMFWIFI_2.4G ถูกสร้างมาจากบอร์ดไมโครคอนโทรลเลอร์ ESP-01

## คำถามหลังการทดลอง
Access point สร้างได้จากอะไร
### คำตอบ
เครือข่าย LAN
