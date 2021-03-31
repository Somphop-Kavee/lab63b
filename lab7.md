# การทดลองที่ 7 การแก้ไขคำสั่งการหน่วงเวลา
## วัตถุประสงค์
1.เพื่อให้เข้าใจการเขียนโปรแกรมบนไมโครคอนโทรลเลอร์ในการแก้ไขคำสั่งการหน่วงเวลา

## อุปกรณ์ที่ใช้
1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
2. สาย USB
3. อุปกรณ์ต่อ USB
4. คอมพิวเตอร์

## ศึกษาข้อมูลเบื้องต้น
1. 03 run example 3 https://youtu.be/CCnN1WJsXQY
2. https://www.myarduino.net/article/134/%E0%B8%AA%E0%B8%AD%E0%B8%99%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99-arduino-%E0%B8%84%E0%B8%B3%E0%B8%AA%E0%B8%B1%E0%B9%88%E0%B8%87%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%AB%E0%B8%99%E0%B9%88%E0%B8%A7%E0%B8%87%E0%B9%80%E0%B8%A7%E0%B8%A5%E0%B8%B2

## วิธีการทำการทดลอง
 #include <Arduino.h>
 
 #include <ESP8266WiFi.h>

 int cnt = 1;

 void setup()
 
 {
 
        Serial.begin(115200);
	
	pinMode(0, OUTPUT);
	
	Serial.println("\n\n\n");
	
}

void loop()

{
	cnt++;
	
	if(cnt % 2) {
	
		Serial.println("========== ON ===========");
		
		digitalWrite(0, HIGH);
		
	} else {
	
		Serial.println("========== OFF ===========");
		
		digitalWrite(0, LOW);
		
	}
	
	delay(1000);
}


# การบันทึกผลการทดลอง
เวลาหน่วงมีมากขึ้น



# คำถามหลังการทดลอง
delay คืออะไีร

### คำตอบ
คำสั่งหน่วงเวลา
