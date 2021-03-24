# การทดลองที่ 2 เรื่อง การเขียนโปรแกรมค้นหาไวไฟ

## วัตถุประสงค์
1.เพื่อให้เข้าใจการเขียนโปรแกรมเพื่อค้นหาไวไฟ


## อุปกรณ์ที่ใช้
1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
2. สาย USB
3. อุปกรณ์ต่อ USB
4. คอมพิวเตอร์

## ศึกษาข้อมูลเบื้องต้น
1. 02 run example 2 https://youtu.be/yBjab0UNuB8

## วิธีการทำการทดลอง
1. เสียบ esp-01 เข้ากับ serial port

![image](https://user-images.githubusercontent.com/80879728/112277153-0ae95d80-8cb4-11eb-986d-ef3a2f49ee89.png)

2. พิมพ์ vi src/main.cpp

![image](https://user-images.githubusercontent.com/80879728/112277837-beeae880-8cb4-11eb-8b47-ca6f9bb4053b.png)

![image](https://user-images.githubusercontent.com/80879728/112277869-cad6aa80-8cb4-11eb-8677-449cedf54b1a.png)

![image](https://user-images.githubusercontent.com/80879728/112278091-083b3800-8cb5-11eb-8aee-956315402655.png)

3. พิมพ์ pio run -t upload เพื่ออัพโหลดโปรแกรมเข้าสู่ไมโครคอนโทรลเลอร์ และ กดปุ่มสีดำและสีแดง

![image](https://user-images.githubusercontent.com/80879728/112278858-da0a2800-8cb5-11eb-8dc1-8b536978dcc3.png)

![image](https://user-images.githubusercontent.com/80879728/112278884-df677280-8cb5-11eb-9f90-a9d92a2d2cb9.png)

![image](https://user-images.githubusercontent.com/80879728/112278953-f1e1ac00-8cb5-11eb-9a77-5dbec37fff5e.png)

4. พิมพ์ pio device monitor เพื่อค้นหาไวไฟ

![image](https://user-images.githubusercontent.com/80879728/112279245-4b49db00-8cb6-11eb-96fa-d0326e3a4575.png)



## การบันทึกผลการทดลอง
เจอ WIFI หลยอัน เช่น
1. MASTER BEDROOM 2.GHz (-86)
2. HI_BMFWIFI_2.4G (-53)

## อภิปรายผลการทดลอง
สามารถเจอ WIFI ได้หลายอันขึ้นอยู่กับว่าบริเวณรอบรอบมีสัญญาณ WIFI มากขนาดไหน

## คำถามหลังการทดลอง
สัญญาณ WIFI ที่สแกนเจอจะมากหรือน้อยขึ้นอยู่กับสิ่งใด
### คำตอบ
ความแรงของสัญญาณ WIFI
