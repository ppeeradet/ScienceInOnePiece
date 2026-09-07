# Changelog

การเปลี่ยนแปลงสำคัญของโปรเจกต์นี้จะบันทึกไว้ในไฟล์นี้

## [Unreleased]

### Added

- เพิ่มเอกสารมาตรฐานของ repository: `README.md`, `CHANGELOG.md` และ `version.json`
- ระบุ `index.html` เป็น canonical production file
- บันทึกสถานะไฟล์ HTML legacy จากการเปรียบเทียบ SHA-256
- เพิ่ม `FIREBASE_RULES.md` เพื่อบันทึก Firestore policy และการตรวจหลังเผยแพร่

### Fixed

- แทนที่ Test Mode rule ที่หมดอายุด้วยกฎถาวรสำหรับ `science_eastblue_lb`

### Security

- จำกัดการเขียน leaderboard ให้ชื่อผู้เล่นตรงกับ document ID
- ปฏิเสธคะแนนติดลบ คะแนนที่ลดลง และการลบ leaderboard

### Changed

- ไม่มีการเปลี่ยน gameplay หรือ `index.html`
