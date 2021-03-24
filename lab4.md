# การทดลองที่ 4 เรื่อง การเขียนโปรแกรมอินพุทสัญญาณดิจิทัล
## วัตถุประสงค์
1.เพื่อให้เข้าใจการเขียนโปรแกรมเพื่ออินพุทสัญญาณดิจิทัล

## อุปกรณ์ที่ใช้
1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
2. สาย USB
3. อุปกรณ์ต่อ USB
4. คอมพิวเตอร์
5. adaptor
6. เซ็นเซอร์แสง
7. ตัวต้านทาน
## ศึกษาข้อมูลเบื้องต้น
1. 04 run example 4 https://youtu.be/nFqoZT26U5k

## วิธีการทำการทดลอง
1. นำ adaptor เสียบกับ serial port และนำ ESP-01 เสียบกับ adaptor อีกที

![image](https://user-images.githubusercontent.com/80879728/112291138-6fabb480-8cc2-11eb-9377-8da7bddb7986.png)

2. พิมพ์ vi src/main.cpp เพื่อดู source code

![image](https://user-images.githubusercontent.com/80879728/112302654-e601e400-8ccd-11eb-8199-67d8dbca12a1.png)

![image](https://user-images.githubusercontent.com/80879728/112302708-f4500000-8ccd-11eb-8d20-2b9d5f393b87.png)

3. พิมพ์ pio run -t upload กดปุ่มสีดำและสีแดง

![image](https://user-images.githubusercontent.com/80879728/112303245-a687c780-8cce-11eb-9dd4-80475df8dd60.png)

![image](https://user-images.githubusercontent.com/80879728/112303266-abe51200-8cce-11eb-9a55-0e02c704b6d8.png)

![image](https://user-images.githubusercontent.com/80879728/112303285-b0a9c600-8cce-11eb-97c4-cb80bf99c0f4.png)

![image](https://user-images.githubusercontent.com/80879728/112303311-b7d0d400-8cce-11eb-920f-62458004b246.png)

4. พิมพ์ pio device monitor

![image](https://user-images.githubusercontent.com/80879728/112303576-041c1400-8ccf-11eb-8fc9-081e5bac4f59.png)

5. นำสายไฟเส้นสีขาว ไปจิ้มตรงช่องของสายไฟสีดำ

![image](https://user-images.githubusercontent.com/80879728/112304027-93292c00-8ccf-11eb-9837-50e7db354f2c.png)

6. กดปุ่มสีดำ

![image](https://user-images.githubusercontent.com/80879728/112304239-d6839a80-8ccf-11eb-93bd-b187ad5ef314.png)

![image](https://user-images.githubusercontent.com/80879728/112304274-e13e2f80-8ccf-11eb-8a7f-35f5beb4195f.png)

7. นำเซ็นเซอร์แสงพันกับตัวต้านทาน แล้วนำไปเสียบกับช่องสายไฟ และนะสายไฟสีขาวมาต่อกับช่องสายไฟ แล้วลองนำมือไปบังเซนเซอร์แสงและปล่อยสลับกันไป

![image](https://user-images.githubusercontent.com/80879728/112304961-b43e4c80-8cd0-11eb-9425-e2580bebc7ce.png)

![image](https://user-images.githubusercontent.com/80879728/112304977-b9030080-8cd0-11eb-8f70-ec9f4ed81945.png)


## การบันทึกผลการทดลอง
เมื่อนำมือไปบังเซนเซอร์แสง หลอดไฟLED จะติด ถ้านำเซนเซอร์แสงให้โดนแสงไฟจะดับ

## อภิปรายผลการทดลอง
หลอดไฟ LED ติด เพราะเมื่อนำมือไปบัง จะทำให้เซนเซอร์แสงมีความต้านทานน้อย  หลอดไฟ LED ดับ เพราะ เมื่อปล่อยมือ จะทำให้เซนเซอร์แสงมีความต้านทานมาก

## คำถามหลังการทดลอง
เซนเซอร์แสงมีกี่ประเภท อะไรบ้าง
### คำตอบ
2 ประเภท คือ 1.
