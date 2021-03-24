# การทดลองที่ 3 เรื่อง การเขียนโปรแกรมเอ้าพุทสัญญาณดิจิทัล
## วัตถุประสงค์
1. เพื่อให้เข้าใจการเขียนโปรแกรมเอ้าพุทสัญญาณดิจิทัลโดยใช้หลอด LED เป็นตัวแสดงผล
2. เพื่อให้รู้จักการประยุกต์ใช้ relay กับ บอร์ดไมโครคอนโทรลเลอร์ ESP-01


## อุปกรณ์ที่ใช้
1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
2. สาย USB
3. อุปกรณ์ต่อ USB
4. คอมพิวเตอร์
5. adaptor
6. relay

## ศึกษาข้อมูลเบื้องต้น
1. 03 run example 3 https://youtu.be/CCnN1WJsXQY
2. 03 run example 3 https://youtu.be/CCnN1WJsXQY

## วิธีการทำการทดลอง
1. นำ adaptor เสียบกับ serial port และนำ ESP-01 เสียบกับ adaptor อีกที

![image](https://user-images.githubusercontent.com/80879728/112282713-ed1ef700-8cb9-11eb-88ed-0db68f506206.png)

2. พิมพ์คำสั่งเรียก 03_Ouput-Port จากโฟลเดอร์ 

![image](https://user-images.githubusercontent.com/80879728/112283352-a2ea4580-8cba-11eb-8913-67082cef806a.png)

![image](https://user-images.githubusercontent.com/80879728/112283384-ac73ad80-8cba-11eb-8965-e6baa18ce833.png)

3. พิมพ์ pio run -t upload และ กดปุ่มสีดำและสีแดง เพื่ออัพโหลดโปรแกรม

![image](https://user-images.githubusercontent.com/80879728/112283927-3cb1f280-8cbb-11eb-954f-2aba0b82a575.png)

![image](https://user-images.githubusercontent.com/80879728/112283959-43406a00-8cbb-11eb-9615-d003bcdb07a7.png)

![image](https://user-images.githubusercontent.com/80879728/112283975-489db480-8cbb-11eb-8f7e-8fed12fe8af0.png)

4.พิมพ์ piorun device monitor เพื่อดูผลการรันโปรแกรม

![image](https://user-images.githubusercontent.com/80879728/112284440-d4174580-8cbb-11eb-846b-bbef5a2aa896.png)

![image](https://user-images.githubusercontent.com/80879728/112284455-d9749000-8cbb-11eb-9850-2751dadd495d.png)

![image](https://user-images.githubusercontent.com/80879728/112284478-de394400-8cbb-11eb-8215-a1f6d2c902c7.png)

### run relay 
#### วิธีการทำทดลอง
1. นำบอร์ดไมโครคอนโทรลเอร์ ESP-01 ที่เขียนโปรแกรมไว้แล้ว มาต่อกับ relay

![image](https://user-images.githubusercontent.com/80879728/112285969-71bf4480-8cbd-11eb-8553-20951bc66bf0.png)

2. นำสายขั้วชาร์จของ relay มาต่อกับหัวของสาย USB คอมพิวเตอร์

![image](https://user-images.githubusercontent.com/80879728/112286491-f5793100-8cbd-11eb-8f6f-a6865937ccab.png)

![image](https://user-images.githubusercontent.com/80879728/112286525-fe6a0280-8cbd-11eb-8080-ba2c9ba8094b.png)


## การบันทึกผลการทดลอง
1. หลอดไฟ LED ตรง port0 ไฟติดถ้า count เป็นเลขคี่ ไฟดับเมื่อ count เป็นเลขคู่
2. เมื่อนำ ESP-01 ต่อกับ relay ทำให้เกิดเสียงสวิตช์เปิด-ปิด

## อภิปรายผลการทดลอง
1. หลอดไฟ LED ติด เพราะถ้าค่าสัญญาณเป็นเลขคี่ ให้เป็นสัญญาณดิจิตอล1ซึ่งหมายถึง ON  และ หลอดไฟLEDดับ เพราะถ้าค่าสัญญาณเป็นเลขคู่ ให้เป็นสัญญาณดิจิตอล0ซึ่งหมายถึง OFF
2. เสียงสวิตช์เปิด-ปิด เป็นเสียงของหน้าสัมผัสแม่เหล็กของ relay
## คำถามหลังการทดลอง
relay ทำหน้าที่คล้ายอุปกรณ์ไฟฟ้าใด
### คำตอบ
สวิตช์ไฟฟ้า
