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

- Click Icon -> ```android``` หน้า project overview ของ Firebase
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
> เช็คว่า Firebase ติดตั้งในเครื่องหรือยัง -> ```$ firebase --version``` <br>
> ถ้าติดตั้งแล้วจะแสดงเวอร์ชัน Ex. 14.15.1

---

### 6. FlutterFire CLI.

> [!WARNING]
> เช็คว่า FlutterFire ติดตั้งในเครื่องหรือยัง -> ```$ flutterfire --version``` <br>
> ถ้าติดตั้งแล้วจะแสดงเวอร์ชัน Ex. 1.3.1

-  Click Icon -> ```Flutter``` หน้า project overview ของ Firebase
-  1 Click ```Next```
-  2 Run คำสั่ง Flutterfire CLI ตามที่แสดงหน้าเว็บไซต์
  
From any directory, run this command:
```bash
$ dart pub global activate flutterfire_cli
```
Then, at the root of your Flutter project directory, run this command:
```bash
$ flutterfire configure --project= <Project Name>
```
- Click ```Next```
- Click ```Continue to console```

ป้อนคำสั่ง ติดตั้ง firebase_core ใน project
```bash
$ flutter pub add firebase_core
```
---
### 7. วิธีติดตั้ง Git + ใช้งาน GitHub (ฉบับสั้น)

ดาวน์โหลด Git 👉 [https://git-scm.com/downloads](https://git-scm.com/downloads)
 → ติดตั้งแบบ CLI -> เข้าหน้าเว็บแล้วเลือกระบบปฏิบัติการตามที่ท่านใช้งานอยู่
 ```bash
$ winget install --id Git.Git -e --source winget
```
แบบ Next → Next → Finish ไปเรื่อย ๆ

เช็คเวอร์ชัน

 ```bash
$ git --version
```

ตั้งชื่อและอีเมล (ต้องตรงกับ GitHub)
 ```bash
$ git config --global user.name "ชื่อคุณ"
```
 ```bash
$ git config --global user.email "อีเมลที่ใช้ใน GitHub"
```

สร้างโฟลเดอร์โปรเจค แล้วเชื่อมกับ GitHub

 ```bash
$ git init
```
 ```bash
$ git add .
```
 ```bash
$ git commit -m "first commit"
```
 ```bash
$ git branch -M main
```
 ```bash
$ git remote add origin https://github.com/username/repo.git
```
 ```bash
$ git push -u origin main
```
