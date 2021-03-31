
# วัตถุประสงค์
1.เพื่อให้เข้าใจการเขียนโปรแกรมบนไมโครคอนโทรลเลอร์

# อุปกรณ์ที่ใช้
1. บอร์ดไมโครคอนโทรลเลอร์ ESP-01
2. สาย USB
3. อุปกรณ์ต่อ USB
4. คอมพิวเตอร์

# ศึกษาข้อมูลเบื้องต้น
06 platformio https://youtu.be/APdBR37Ukxg

# วิธีการทำการทดลอง
 #include <Arduino.h>
 
 #include <ESP8266WiFi.h>

 int cnt = 0;

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



# คำถามหลังการทดลอง


คำตอบ
