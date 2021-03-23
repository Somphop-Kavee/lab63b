# การทดลองที่ 1 เรื่อง การเขียนโปรแกรมเพื่อรันบนไมโครคอนโทรเลอร์ 

## วัตถุประสงค์
1.เพื่อให้เข้าใจการเขียนโปรแกรมบนไมโครคอนโทรลเลอร์

## อุปกรณ์ที่ใช้
 1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
 2. สาย USB
 3. อุปกร์ต่อ USB
 4. คอมพิวเตอร์

## ศึกษาข้อมูลเบื้องต้น
1. 01 run example 1 https://www.youtube.com/watch?v=NLIUsWLEpmg&ab_channel=TANI-IOT

## วิธีการทำการทดลอง
1. เสียบไมโครคอนโทรลเลอร์เข้ากับ serial port

![image](https://user-images.githubusercontent.com/80879728/112182393-d3d16880-8c2f-11eb-84e7-47d7d29f53b1.png)

2. เรียกโปรแกรม PATTANI ขึ้นมาจากโฟลเดอร์

![image](https://user-images.githubusercontent.com/80879728/112184017-64f50f00-8c31-11eb-9d27-cfae1f124be3.png)

3. พิมพ์ vi platformio.ini เพื่อแสดงข้อมูลของบอร์ด ESP-01

![image](https://user-images.githubusercontent.com/80879728/112184871-3a578600-8c32-11eb-9d69-585b5fd7a566.png)

4. พิมพ์ pio run -t upload และกดปุ่มสีดำและปุ่มสีแดงเพื่ออัปโหลดโปรกรมเข้าไปในบอร์ด ESP-01

![image](https://user-images.githubusercontent.com/80879728/112185932-409a3200-8c33-11eb-99f8-371f3840e361.png)

![image](https://user-images.githubusercontent.com/80879728/112185987-4abc3080-8c33-11eb-8bdb-892acbc14266.png)

5. พิมพ์ pio device monitor เพื่อแสดงผลลัพธ์

![image](https://user-images.githubusercontent.com/80879728/112186803-1432e580-8c34-11eb-89e7-64f498e878b6.png)


## การบันทึกผลการทดลอง
ชื่อบอร์ดคือ esp01
framework arduino
เลขเพิ่มขึ้นทีละ1

## อภิปรายผลการทดลอง
การเขียนโปรแกรมมีความง่าย

## คำถามหลังการทดลอง
ให้เลือกบอร์ดไมโครคอนโทรลเลอร์มา 1 บอร์ด จาก platformio
