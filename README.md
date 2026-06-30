# Impact Map — 30th Anniversary, Faculty of Environmental Management (PSU)

แผนที่ผลกระทบงานวิจัยแบบ Interactive · ครบรอบ 30 ปี คณะการจัดการสิ่งแวดล้อม มหาวิทยาลัยสงขลานครินทร์
Interactive research-impact map — *From Knowledge to Sustainability / จากความรู้ สู่ความยั่งยืน*

เครือข่ายความร่วมมือทั่วโลก · พื้นที่ศึกษา · ไทม์ไลน์ 30 ปี · สาขางานวิจัย · SDGs · ผลงานเด่น
จากผลงานตีพิมพ์ใน Scopus 989 ชิ้น (1997–2026)

---

## 📁 ไฟล์ในชุดนี้ / Files (อัปโหลด "ทั้งหมด" ขึ้น repo)

```
index.html          ← หน้าเว็บหลัก
support.js          ← ตัวรันระบบ (จำเป็น)
impact-data.js      ← ข้อมูลที่ประมวลผลแล้ว
study-sites.json    ← ข้อมูลพื้นที่ศึกษา
assets/
  logo-en-white.png
  logo-th-white.png
```

> ⚠️ ต้องอัปโหลด **ทุกไฟล์พร้อมโฟลเดอร์ `assets/`** ให้อยู่ระดับเดียวกัน — ถ้าขาด `support.js` / `impact-data.js` / `study-sites.json` แผนที่และข้อมูลจะไม่แสดง

---

## 🚀 Deploy บน GitHub Pages

1. สร้าง repository ใหม่ (หรือใช้ repo เดิม `Envi-Interactive-Impact-Map`)
2. อัปโหลด **ทุกไฟล์ด้านบน** เข้า repo (ลากวางผ่าน *Add file → Upload files* — ลากทั้งโฟลเดอร์ได้)
   - ตรวจให้แน่ใจว่ามี `support.js`, `impact-data.js`, `study-sites.json` และโฟลเดอร์ `assets/` ครบ
3. ไปที่ **Settings → Pages**
4. *Build and deployment → Source* เลือก **Deploy from a branch**
5. เลือก branch **`main`** โฟลเดอร์ **`/ (root)`** แล้ว **Save**
6. รอ 1–2 นาที เว็บจะออนไลน์ที่ `https://<username>.github.io/<repo>/`

> Netlify / Vercel / Cloudflare Pages: ลากโฟลเดอร์นี้ทั้งโฟลเดอร์วางได้ทันที

---

## 🩹 ถ้าแผนที่ไม่แสดง (Troubleshooting)

- **ขาดไฟล์** — สาเหตุที่พบบ่อยที่สุดคืออัปโหลด `index.html` ไฟล์เดียว ต้องอัป `support.js` + `impact-data.js` + `study-sites.json` + `assets/` ด้วย
- **ต้องออนไลน์** — แผนที่ใช้ไลบรารี d3 / TopoJSON / world-atlas จาก CDN (jsdelivr) จึงต้องมีอินเทอร์เน็ต (GitHub Pages ออนไลน์อยู่แล้ว)
- **อย่าเปิดแบบ `file://`** — เบราว์เซอร์จะบล็อกการโหลดข้อมูล ให้เปิดผ่าน GitHub Pages หรือเซิร์ฟเวอร์ (เช่น `python -m http.server` ในโฟลเดอร์นี้)
- เปิด **Console (F12)** ดู error ได้ ถ้ามีบรรทัด `init` แสดงว่าโหลดไลบรารี/ข้อมูลไม่สำเร็จ

---

## 📊 ที่มาข้อมูล / Data source

Scopus · ปรับปรุงข้อมูล 30 มิ.ย. 2569 (30 June 2026) · ครอบคลุมผลงานถึงปี 2026
ประเทศ/สถาบันสกัดจาก affiliation · พื้นที่ศึกษาสกัดจากชื่อเรื่อง+บทคัดย่อ (~69%) · SDG ประเมินจากคำสำคัญ

ระบบไทย/อังกฤษสลับได้ที่ปุ่มมุมขวาบน · รองรับมือถือ (responsive)
