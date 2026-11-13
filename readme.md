# 🧊 Fridge Expiry Manager

แดชบอร์ดบอกว่าของในตู้เย็นชิ้นไหนใกล้หมดอายุ เพื่อให้กินทันก่อนต้องทิ้ง
A small web dashboard that shows which food and medicine in your fridge is about to expire, so you use it before you have to throw it away.

**Live demo:** https://YOUR-USERNAME.github.io/YOUR-REPO/  <!-- แก้เป็นลิงก์ GitHub Pages ของคุณ / replace with your GitHub Pages link -->

## ปัญหาที่แก้ / The problem

คนที่อยู่หอพักคนเดียวหรืออยู่กับครอบครัวมักซื้อของสด นม หรือยามาเก็บไว้แล้วลืมกิน จนหมดอายุและต้องทิ้ง
ทำให้เสียเงิน เกิดขยะอาหาร และถ้าเป็นยา อาจเผลอกินยาที่หมดอายุแล้วได้

People who live alone (for example in a dorm) or with family buy fresh food, milk and medicine, forget about it, and end up throwing it away.
That wastes money, creates food waste, and for medicine it can be unsafe to take something that has expired.

## ใครใช้ / Who it is for

นักศึกษาที่อยู่หอ ครอบครัว และทุกคนที่ใช้ตู้เย็นร่วมกัน
Students in dorms, families, and anyone who shares a fridge.

## ทำอะไรได้บ้าง / Features

- เพิ่มของ: ชื่อ หมวดหมู่ (นม ผัก เนื้อสัตว์ ยา ฯลฯ) และวันหมดอายุ / Add items with a name, category and expiry date
- เรียงอัตโนมัติ ของที่ใกล้หมดอายุที่สุดอยู่บนสุด / Always sorted by days left, soonest first
- สีแจ้งเตือน / Colour alerts
  - 🔴 แดง: หมดอายุแล้วหรือเหลือน้อยกว่า 3 วัน / expired or under 3 days left
  - 🟡 เหลือง: เหลือ 3–7 วัน / 3 to 7 days left
  - 🟢 เขียว: เหลือมากกว่า 7 วัน / more than 7 days left
- ปุ่ม "กินแล้ว" และ "ทิ้งแล้ว" ลบรายการและนับสถิติว่าช่วยลดขยะอาหารได้เท่าไร / "Eaten" and "Thrown away" buttons remove an item and keep a count
- อิโมจิตามหมวดหมู่ / An emoji for each category
- เมนูแนะนำจากของที่ใกล้หมดอายุ เช่น ไข่ + ขนมปัง → เฟรนช์โทสต์ (ใช้กฎง่าย ๆ ไม่ใช้ AI) / Simple rule-based meal ideas, no AI involved
- เตือนเมื่อยาหมดอายุ / Warning for expired medicine
- สลับภาษาไทย/อังกฤษได้ / Thai and English interface
- โหมดมืดและใช้บนมือถือได้ / Dark mode and mobile friendly

## วิธีรัน / How to run

ไม่ต้องติดตั้งอะไร / No installation needed.

1. ดาวน์โหลด `index.html` จาก repository นี้ / Download `index.html` from this repository
2. ดับเบิลคลิกเพื่อเปิดในเบราว์เซอร์ (Chrome, Edge, Safari ฯลฯ) / Double-click it to open in a browser
3. ครั้งแรกจะมีข้อมูลตัวอย่างให้ลอง กดปุ่ม "ล้างตัวอย่าง" แล้วเพิ่มของจริงของคุณ / The first visit shows sample data. Click "Clear samples" and add your own items

ข้อมูลถูกเก็บในเบราว์เซอร์ของคุณ (localStorage) ไม่ถูกส่งไปที่ไหน
Your data is saved in your own browser (localStorage) and is never sent anywhere.

## เทคโนโลยี / Tech

HTML, CSS and JavaScript in a single file (`index.html`). No libraries, no build step.
