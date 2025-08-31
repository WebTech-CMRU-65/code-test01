### 1. Downloads The AI Code Editor

 Click เพื่อดาวน์โหลด -> [https://cursor.com/downloads](https://cursor.com/downloads)

---

### 2. Check the environment Flutter

> [!WARNING]
> ถ้าเวอร์ชันต่ำกว่า 3.35.1 ควรอัพเกรดก่อนสร้าง Project Flutter

เช็คเวอร์ชัน Flutter 
```bash
$ flutter --version
```
อัพเกรด Flutter
```bash
$ flutter upgrade
```
สร้าง Project Flutter
```bash
$ flutter create <my_app>
```

---

### 3. Create Project Firebase

- Click เพื่อเข้าสู่หน้าเว็บไซต์ -> [https://firebase.google.com](https://firebase.google.com)
- Click ```Go To Console```
- Click ```Create a new Firebase project```
- Enter your project name and Click ```Continue``` x2
- choose or create a Google Analytics account and Click ```Create project``` and Click ```Continue```
---
### 4. Register App Android
> [!NOTE]
> Path Folder // ```android > app > build.gradle.kts```

- Click Icon -> ```android```
- 1 กรอก ```Android package name``` ->  กรอก ```App nickname``` -> เว้นว่าง -> ```Debug...```
- 2 ดาวน์โหลดไฟล์ ```google-services.json```
- 3 เลือก ```Kotlin DSL (build.gradle.kts)``` Click ```Next```
- 4 Click ```Continue to console```
---
### 5. edit environment variables

- Search For Windows -> ```Edit the system environment variables``` 🔍
- Click ```Environment Variables```
- เลือก ```Path``` ในช่อง User variables for ```<name PC>``` Click ```Edit...```
- Click ```New``` วาง Path นี้
```bash
C:\Users\<name PC>\AppData\Local\Pub\Cache\bin
```
> [!WARNING]
> อย่าลืมเปลี่ยนชื่อ <name PC > ให้ตรงกับ PC ของคุณ
- Click ```OK > OK > Apply > OK```

- เปิด ```Command Prompt```
ป้อนคำสั่ง install Firebase
```bash
$ npm install -g firebase-tools
```
ป้อนคำสั่ง Login Firebase
```bash
$ npm install -g firebase-tools
```
> [!WARNING]
> ถ้าเจอ Error ให้ใช้คำสั่งนี้ -> ```$ Set-ExecutionPolicy RemoteSigned```<br>
> เช็คว่า Firebase ติดตั้งในเครื่องหรือยัง -> ```$ firebase --version``` ถ้าติดตั้งแล้วจะแสดงเวอร์ชัน Ex. 14.15.1

