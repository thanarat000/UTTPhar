# UTTPhar · บัญชียา รพ.อุตรดิตถ์

เว็บแอพค้นหาบัญชียาของโรงพยาบาลอุตรดิตถ์ (static site ไม่ต้อง build)

- `index.html` หน้าแอพ
- `data.json` ข้อมูลยา (แปลงจากไฟล์ บช ยา 16112569.xlsx)

## Deploy บน Vercel
1. Import repository นี้ใน Vercel
2. Framework Preset: **Other**, Build Command: เว้นว่าง, Output Directory: เว้นว่าง (ใช้ root)
3. กด Deploy

## อัปเดตข้อมูลยา
แทนที่ `data.json` ด้วยไฟล์ใหม่ แล้ว commit/push Vercel จะ deploy ใหม่ให้อัตโนมัติ

## Google Apps Script
โฟลเดอร์ `apps-script/` มี `Code.gs`, `Index.html`, `Data.html` สำหรับวางในโปรเจกต์ Apps Script แล้ว Deploy เป็น Web app

## ความหมายสีตัวอักษร (ตาม HOSxP)
ม่วง = OCPA/ยามูลค่าสูง · น้ำเงิน = High alert drugs · เขียว = staff สั่งใช้ได้ · ฟ้าพาสเทล = บัญชี จ2 · ส้ม = ชำระเงินเองทุกสิทธิ · แดง = NED เฉพาะเบิกได้ · ชมพู = Restrict drugs (ATB)
