# wiw — Vercel-ready static website

โปรเจกต์เว็บไซต์แบบ Static HTML พร้อมนำเข้า Vercel ผ่าน GitHub

## ไฟล์
- `index.html` — หน้าเว็บไซต์หลัก
- `vercel.json` — ตั้งค่า Vercel ให้ใช้ไฟล์ในโฟลเดอร์หลัก โดยไม่ต้องมีขั้นตอน build

## วิธีนำขึ้น Vercel สำหรับมือใหม่
1. แตกไฟล์ ZIP นี้ในคอมพิวเตอร์
2. เข้า GitHub และสร้าง Repository ใหม่ เช่น `wiw`
3. ใน Repository เลือก **Add file → Upload files** แล้วอัปโหลด `index.html`, `vercel.json` และ `README.md` จากโฟลเดอร์ที่แตกไฟล์ (อย่าอัปโหลด ZIP)
4. กด **Commit changes**
5. เข้า Vercel แล้วเลือก **Add New → Project**
6. เชื่อมต่อ GitHub หากระบบถามสิทธิ์ แล้วเลือก Repository `wiw` กด **Import**
7. ตรวจว่า Root Directory เป็นโฟลเดอร์ที่มี `index.html` และ `vercel.json` อยู่ โดยทั่วไปคือ `./`
8. กด **Deploy** และรอจนสถานะเป็น Ready
9. เปิด URL ที่ Vercel แสดงให้

## หมายเหตุ
- เป็น Static HTML ไม่ต้องใช้ Build Command หรือ Install Command
- ข้อมูลที่เก็บใน `localStorage` อยู่ในเบราว์เซอร์ของผู้ใช้แต่ละคน ไม่ซิงก์ระหว่างผู้ใช้โดยอัตโนมัติ
- รูปภาพที่เก็บไว้ในเบราว์เซอร์จะไม่ถูกอัปโหลดไปยังเซิร์ฟเวอร์กลางโดยอัตโนมัติ
