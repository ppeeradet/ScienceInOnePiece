# Science in One Piece – อีสต์บลู

เกมวิทยาศาสตร์ระดับประถมในธีม One Piece

- Production: https://ppeeradet.github.io/ScienceInOnePiece/
- Canonical production file: `index.html`
- Status: Active
- Architecture: static single-file HTML application

## Repository policy

- `index.html` คือ production version หลักเสมอ
- ไม่สร้าง `update.html` หรือสำเนา production เพิ่ม
- ใช้ Git history, tags และ releases สำหรับประวัติเวอร์ชัน
- Phase 1 เป็น metadata-only: ไม่แก้ gameplay หรือ `index.html`
- เก็บไฟล์ legacy ไว้ก่อนจนกว่าจะผ่านการ review

## Legacy HTML inventory

- `index_OnePieceScience.html` — duplicate legacy; SHA-256 เหมือน `index.html` ณ วันที่ตรวจ

## Branch relationship

- `main` เก็บตัวเกมและ metadata สำหรับ GitHub Pages
- `data` เก็บคลังคำถามที่ตัวเกมเรียกใช้
- ต้องรักษาความสัมพันธ์นี้ไว้ และไม่ย้ายข้อมูลข้าม branch โดยไม่มีการตรวจสอบ URL ที่ตัวเกมอ้างอิง

## Local use

เปิด `index.html` ในเว็บเบราว์เซอร์ หรือใช้ลิงก์ Production ด้านบน

