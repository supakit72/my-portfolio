# 🏢 SmartDorm (ระบบจัดการหอพักอัจฉริยะ)

โปรเจกต์เว็บแอปพลิเคชันสำหรับจัดการหอพัก สร้างขึ้นเพื่อช่วยเจ้าของหอพักในการบริหารจัดการห้องพัก ผู้เช่า และการออกบิลค่าเช่าได้อย่างเป็นระบบและแม่นยำ ลดการใช้กระดาษ (Paperless) และเพิ่มความสะดวกในการติดตามสถานะต่างๆ ผ่านแดชบอร์ดส่วนกลาง

🔗 **Live Demo:** [https://smart-dorm-five.vercel.app](https://smart-dorm-five.vercel.app)
📸 **ตัวอย่างหน้าจอระบบ (Screenshots):Screenshot 2026-08-13 212101.png**


---

## ✨ คุณสมบัติหลักของระบบ (Key Features)

*   📊 **Dashboard Analytics:** สรุปภาพรวมหอพัก อัตราการเข้าพัก และยอดบิลค้างชำระรายเดือน
*   🚪 **Room & Tenant Management:** ระบบจัดการข้อมูลห้องพัก ประเภทห้อง และประวัติผู้เช่าแบบครบวงจร
*   🧾 **Billing System:** ระบบออกบิล จัดการจดมิเตอร์ (ค่าไฟ/ค่าน้ำ) และรายการบิลเพิ่มเติม (Presets)
*   📱 **Responsive Design:** รองรับการใช้งานทั้งบนคอมพิวเตอร์และโทรศัพท์มือถือ (พร้อมระบบ Collapsible Sidebar ที่ปรับรูปแบบตามขนาดหน้าจอ)
*   🔐 **Secure Authentication:** ระบบเข้าสู่ระบบที่ปลอดภัยสำหรับผู้ดูแลระบบ (Admin)

---

## 🛠 เทคโนโลยีที่ใช้ (Tech Stack)

*   **Frontend:** Next.js (App Router), React, TypeScript, Tailwind CSS
*   **Backend:** Next.js Server Actions (จัดโครงสร้างแยกโฟลเดอร์ไว้ที่ `src/backend` อย่างชัดเจน)
*   **Database:** Supabase (PostgreSQL) สำหรับจัดการฐานข้อมูลและระบบ Authentication
*   **Icons/Assets:** Inline SVG (ไม่พึ่งพา Icon Library ภายนอกเพื่อเพิ่มความเร็วในการโหลดหน้าเว็บ)
*   **Deployment:** Vercel (Auto-deploy) & GitHub

---

## 🚀 ขั้นตอนการติดตั้งและการรันระบบ (Getting Started)

**1. Clone Repository**
```bash
git clone [https://github.com/supakit72/smart-dorm.git](https://github.com/supakit72/smart-dorm.git) 
cd smart-dorm

2. Install Dependencies

Bash
npm install
3. Environment Setup
สร้างไฟล์ .env.local ที่ root directory และตั้งค่าตัวแปรสำหรับเชื่อมต่อ Supabase:

ข้อมูลโค้ด
NEXT_PUBLIC_SUPABASE_URL=your-supabase-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-supabase-anon-key
4. Run Application

Bash
npm run dev 
เปิดเบราว์เซอร์และเข้าไปที่ http://localhost:3000

💡 สิ่งที่ได้เรียนรู้และกระบวนการคิด (Key Learnings)
การออกแบบสถาปัตยกรรมโค้ด (Code Architecture): ได้เรียนรู้การจัดระเบียบโปรเจกต์ Full-stack โดยแยกส่วน Frontend (src/app, src/components) และ Backend (src/backend) ออกจากกันอย่างชัดเจนภายในโปรเจกต์ Next.js เดียว เพื่อให้ง่ายต่อการดูแลรักษา

การจัดการฐานข้อมูลด้วย BaaS: การประยุกต์ใช้ Supabase ในการออกแบบโครงสร้างฐานข้อมูล (Relational Database) และจัดการระบบยืนยันตัวตนได้อย่างมีประสิทธิภาพ

การปรับปรุง UI/UX & Performance: การใช้ Tailwind CSS ในการทำ Responsive Design แก้ไขปัญหาเมนูนำทางในโหมด Mobile และการฝัง Inline SVG แทนการโหลด Library ภายนอกเพื่อรีดประสิทธิภาพของเว็บไซต์ให้โหลดเร็วที่สุด

👤 ผู้พัฒนา (Author)
ศุภกิตติ์ (Supakit)

🎓 โครงงานนวัตกรรมธุรกิจดิจิทัล

🐙 GitHub Profile: @supakit72