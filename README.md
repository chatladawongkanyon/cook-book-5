## ควบคุม LED ให้ติดเรียงกัน4ดวง
1.เปิด VS Code และใช้คำสั่ง Create ESP-IDF Project เพื่อสร้างโปรเจกต์ใหม่ เลือกบอร์ด ESP32 และตั้งชื่อโปรเจกต์

![Screenshot 2024-11-09 005837](https://github.com/user-attachments/assets/b1c8bda1-8e53-4fbd-b4a7-42b92703d02b)

2.การตั้งค่า GPIO สำหรับ LED
LED 4 ดวงถูกเชื่อมต่อกับ GPIO 12, 13, 14, 15:
ไปที่ไฟล์ main/main.c
เขียนโค้ดเพื่อกำหนด GPIO สำหรับ LED และตั้งค่าการควบคุมไฟ LED

![Screenshot 2024-11-09 025404](https://github.com/user-attachments/assets/140a2897-e714-4097-8206-98a13273518d)

![Screenshot 2024-11-09 025428](https://github.com/user-attachments/assets/97cd93ea-90f2-44a3-bd16-28a8fdf08f0a)

 3.คอมไพล์และอัปโหลดโค้ดไปยัง ESP32
Build, Flash and Monitor เพื่อคอมไพล์และอัปโหลดโค้ดไปยัง ESP32
ถ้าเชื่อมต่อบอร์ดสำเร็จ จะเห็นข้อความใน Serial Monitor และ LED ทั้ง 4 ดวงจะติดเรียงกันตามลำดับในลูป (สลับการเปิดปิด LED ทีละดวง)
