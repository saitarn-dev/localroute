# 🛺 LocalRoute (โลคอลรูท) — Thailand Local Transit & Tourist Safety Companion

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://saitarn-dev.github.io/localroute/)
[![Figma Ready](https://img.shields.io/badge/Figma-Design%20Tokens%20%26%20Flows-F24E1E?style=for-the-badge&logo=figma)](./design/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Mobile First](https://img.shields.io/badge/Design-Mobile%20First%20(390px)-8C82FC?style=for-the-badge)](index.html)

**LocalRoute** คือแอปพลิเคชันต้นแบบ (High-Fidelity Interactive Prototype) สำหรับช่วยเหลือนักท่องเที่ยวและผู้เดินทางคนเดียว (Solo Travelers) ในการเดินทางด้วยระบบขนส่งสาธารณะท้องถิ่นทั่วประเทศไทย เช่น รถสองแถวแดงเชียงใหม่, รถโพท้องภูเก็ต, รถสองแถวรอบเกาะสมุย, มอเตอร์ไซค์รับจ้าง และรถไฟฟ้า Airport Rail Link / BTS กรุงเทพฯ

---

## 🌟 ฟังก์ชันหลัก (Core Killer Features)

### 1. 🚊 ผังสถานีสไตล์ MRT/BTS (Station Schematic Tracker)
* จำลองเส้นทางและสถานี/ป้ายจุดจอดเสมือนจริงของขนส่งท้องถิ่น
* แสดงตำแหน่งรถสด พร้อมปุ่มจำลองการเดินทาง (`▶️ ขยับไปป้ายถัดไป`)
* คำนวณระยะทางและเวลาคงเหลืออัตโนมัติ

### 2. 🔔 ระบบปลุกเตือนก่อนถึงที่หมาย (500m Arrival Alert & Wake-Up)
* แจ้งเตือนด้วยเสียงกริ่งคู่ (Dual Web Audio Chime: 659Hz + 523Hz) และการสั่น
* แสดงหน้าต่างพร้อมปุ่มปิด `✕` และปุ่มเลื่อนเวลา `💤 เลื่อนเตือนอีก 2 นาที`
* ฟังก์ชันแตะเพื่อให้โทรศัพท์พูดภาษาไทยบอกคนขับ: *"จอดตรงนี้ด้วยครับ"*

### 3. 🛡️ แชร์พิกัดปลอดภัย & รายงานการโก่งราคา (Safe Ride & Scam Report)
* **Safe Ride Share:** กดแชร์พิกัด, ทะเบียนรถ, จุดหมาย และเวลาขึ้นรถเข้า LINE หรือ WhatsApp ได้ในคลิกเดียว
* **Community Scam Alert:** ระบบแจ้งเตือนโดนเรียกราคาเกินจริงจากชุมชน อัปเดตแถบแจ้งเตือนแบบเรียลไทม์

### 4. 📞 ระบบจำลองโทรฉุกเฉินเสมือนจริง (In-App Phone Call Simulator)
* รองรับสายด่วนสำคัญ: ตำรวจท่องเที่ยว (1155), กู้ชีพนเรนทร (1669), เหตุด่วนเหตุร้าย (191) และสหกรณ์เดินรถ
* หน้าจอจำลองการโทรระดับพรีเมียม มีเสียงสัญญาณต่อสาย (Dial Tone), ตัวนับเวลาคุยสาย และเสียงเจ้าหน้าที่ตอบรับอัตโนมัติ

### 5. 🛎️ บริการจองที่พัก เหมารถ & วันเดย์ทัวร์ (Smart Travel Marketplace)
* **🏨 ที่พักใกล้จุดหมาย:** โรงแรม/โฮสเทลที่เดินถึงได้ใน 200–450 เมตร พร้อมราคากลางต่อคืน
* **🚗 เหมารถทั้งวัน ฿1,500:** เรตราคาเหมามาตรฐานรวมน้ำมัน ไม่ต้องกังวลเรื่องการต่อรองราคา
* **🎟️ วันเดย์ทัวร์ชุมชน:** ทริปท่องเที่ยวท้องถิ่นที่ยืนยันราคาแน่นอน พร้อมส่งขอใบเสนอราคาผ่าน LINE

### 6. 🗺️ ครอบคลุม 4 จังหวัดท่องเที่ยวชั้นนำ (Multi-Province Hub)
* 🌸 **เชียงใหม่ (CNX):** รถสี่ล้อแดง (฿30), Smart Bus RTC (฿20)
* 🏙️ **กรุงเทพฯ (BKK):** วินมอเตอร์ไซค์, Airport Rail Link, BTS
* 🏖️ **ภูเก็ต (HKT):** รถโพท้องสีชมพู (฿15), Phuket Smart Bus (฿100)
* 🌴 **เกาะสมุย (USM):** สองแถวรอบเกาะสมุย (฿60), เรือเฟอร์รี่

---

## 🎨 Design System & Typography

* **ฟอนต์หลัก:** `K2D` (ภาษาไทย สไตล์ Geometric เป็นมิตร อ่านง่าย) + `Quicksand` (ภาษาอังกฤษ สไตล์โค้งมน ทันสมัย)
* **มาตรฐานการแสดงผล (Accessibility):** ตัวอักษรขนาดขั้นต่ำ 10px - 11px รองรับการอ่านในทุกสภาพแสง
* **สองภาษา 100%:** สลับภาษาไทย 🇹🇭 และภาษาอังกฤษ 🇬🇧 ได้ทันทีทุกหน้า

---

## 📁 โครงสร้างโปรเจกต์ (Project Structure)

```text
localroute/
├── index.html                           # ตัวแอปต้นแบบ Interactive Prototype (Vanilla HTML5/JS/Tailwind/Leaflet)
├── README.md                            # เอกสารแนะนำและคู่มือการใช้งาน
├── LICENSE                              # สัญญาอนุญาตแบบ MIT
└── design/
    ├── localroute-design-tokens.json    # Design Tokens (Colors, Typography, Elevation, Radii)
    ├── localroute-master-flows.svg      # Figma Master Canvas เวกเตอร์รวมทุกโฟลว 14 หน้าจอ
    ├── localroute-figma-artboards.svg   # Figma Artboards ขนาด 1:1 (390 x 844 px)
    └── localroute-figma-all-flows.zip   # แพ็กเกจไฟล์สำหรับนำเข้า Figma ทั้งหมด
```

---

## 🚀 วิธีเปิดใช้งาน (Getting Started)

### 1. เปิดทดสอบทันทีบนเครื่อง
เพียงดับเบิลคลิกไฟล์ `index.html` เพื่อเปิดบนเว็บเบราว์เซอร์ใดก็ได้ (Chrome, Safari, Edge) โดยไม่ต้องติดตั้งโปรแกรมเสริมใด ๆ

### 2. นำไปจัดแสดงบน Portfolio
* สามารถนำลิงก์ [GitHub Pages](https://saitarn-dev.github.io/localroute/) ไปแปะเป็นปุ่ม CTA บน Notion, Behance, หรือเว็บไซต์พอร์ตโฟลิโอของคุณ
* สามารถฝังผ่าน `<iframe>` ขนาด 390x844 px เพื่อให้ผู้ตรวจกดเล่นได้โดยตรง

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
