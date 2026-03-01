# 📱 ScorePro PWA — วิธีติดตั้งบนมือถือ

## ไฟล์ที่ได้รับ (ต้องอยู่ในโฟลเดอร์เดียวกันทั้งหมด)
```
📁 ScorePro/
  ├── คะแนน.html       ← ตัวแอป
  ├── manifest.json    ← ข้อมูลแอป
  ├── sw.js            ← ระบบ offline
  ├── icon-192.png     ← ไอคอนแอป
  └── icon-512.png     ← ไอคอนแอป (ใหญ่)
```

---

## 🚀 วิธีใช้งาน — เลือกทำแบบใดแบบหนึ่ง

### ตัวเลือก A: อัปโหลดขึ้น GitHub Pages (ฟรี 100%)
1. สมัคร [github.com](https://github.com) (ฟรี)
2. สร้าง Repository ใหม่
3. อัปโหลดไฟล์ทั้งหมดขึ้นไป
4. ไปที่ Settings → Pages → เลือก Branch: main
5. ได้ลิงก์เช่น `https://ชื่อ.github.io/scorepro/คะแนน.html`
6. เปิดลิงก์บนมือถือ → ติดตั้งได้เลย

### ตัวเลือก B: ใช้ Netlify Drop (ง่ายที่สุด)
1. ไปที่ [app.netlify.com/drop](https://app.netlify.com/drop)
2. ลากโฟลเดอร์ทั้งหมดใส่
3. ได้ลิงก์ทันที → เปิดบนมือถือ → ติดตั้งได้เลย

### ตัวเลือก C: รันบนคอมตัวเอง (ต้องรัน server)
```bash
# ต้องมี Python ในคอม
cd โฟลเดอร์ที่วางไฟล์
python3 -m http.server 8080
# เปิด http://localhost:8080/คะแนน.html
```

---

## 📲 วิธีติดตั้งบนมือถือ

### Android (Chrome)
1. เปิดลิงก์ใน Chrome
2. กด **⋮** (เมนู 3 จุด) มุมขวาบน
3. เลือก **"Add to Home screen"** หรือ **"ติดตั้งแอป"**
4. กด ติดตั้ง ✅

### iPhone/iPad (Safari)
1. เปิดลิงก์ใน **Safari** (ต้องใช้ Safari เท่านั้น)
2. กดปุ่ม **แชร์** (กล่องมีลูกศรชี้ขึ้น) ด้านล่าง
3. เลือก **"Add to Home Screen"**
4. กด เพิ่ม ✅

### Mac (Chrome หรือ Safari)
1. เปิดลิงก์
2. Chrome: กดไอคอน ⊕ ใน address bar → Install
3. Safari: File → Add to Dock

---

## ✨ ฟีเจอร์ PWA
- 📴 ใช้งาน **offline** ได้ (หลังจากเปิดครั้งแรก)
- 🏠 มีไอคอนบน Home Screen เหมือนแอปจริง
- 💾 ข้อมูลเซฟใน localStorage อัตโนมัติ
- 🖥️ ไม่มี address bar — หน้าจอเต็ม
