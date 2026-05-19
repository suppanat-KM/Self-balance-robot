# Self-balance-robot
C++ & IOT

## 🔧 Features

- ควบคุมสมดุลด้วย MPU6050 และอัลกอริธึม PID
- ควบคุมทิศทางด้วยรีโมตอินฟราเรด (IR Remote)
- รองรับการปรับค่า PID แบบง่ายในโค้ด
- ใช้งานร่วมกับ Arduino Uno

## 🧰 Hardware Requirements

- Arduino Uno
- MPU6050
- Motor Driver L298N
- DC Motors x2
- ล้อ (Wheels)
- แบตเตอรี่ 7.4V หรือ 12V
- รีโมต IR และตัวรับ IR
- model robot ตามใจเรา หรือ ดูจาก `img/model.jpg`

## 🚀 Getting Started

1. ต่ออุปกรณ์ตามวงจรใน `img/robot circuit.png`
2. เปิด `main.ino` ใน Arduino IDE
3. อัปโหลด Library ที่เกียวข้อง
4. ปรับค่าพินตามที่เชื่อมต่อในโค้ด
5. ปรับค่า PID , offset , setpoint ให้เข้ากับหุ่นยนต์ของตัวเอง
6. อัปโหลดโค้ดไปยัง Arduino Uno
7. ทดสอบการทรงตัวบนพื้นเรียบ และใช้รีโมตควบคุม

## ⚙️ PID Tuning

ค่าเริ่มต้นในโค้ด:

```cpp
double Kp = 40;
double Ki = 280;
double Kd = 0.3;
