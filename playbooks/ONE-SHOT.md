# ONE-SHOT — สั่งครั้งเดียว ไม่วนถาม

**Flow:** Decode → Capability → Risk → Plan → Execute → Verify → Handoff → Continue

- **Decode:** กำหนด Objective, Acceptance, Scope และ Constraints
- **Capability:** ตรวจว่ามี GitHub/Browser/Agent Tools จริง
- **Risk:** ตรวจ [Approval Gates](APPROVAL-GATES.md) ก่อน mutation
- **Plan:** แยก Task, owner, dependency, evidence, single-writer lock
- **Execute:** ทำทุกงานที่ได้รับสิทธิ์แล้วต่อเนื่อง แก้บล็อกเกอร์แบบปลอดภัยและจำกัด retry
- **Verify:** read-back, test outputs, SHA และ review จริง
- **Handoff:** บันทึกบทเรียนและการตัดสินใจไว้ใน Repo ฝึกของน้องเมื่อมีสิทธิ์
- **Continue:** เลื่อนสู่ขั้นปลอดภัยถัดไปโดยไม่รอคำว่า 'ต่อ'

## ไม่ต้องถามซ้ำ
อ่านไฟล์? อ่านเลย. วางแผน? ทำเลย. สร้าง Draft ที่อนุญาต? ทำเลย. ตรวจ Diff? ตรวจเลย.

## ต้องถามเฉพาะ decision gate
Permission, Billing, deletion, public release, privacy, merge/deploy live, ติดต่อภายนอก หรือการกระทำที่เจ้าของต้องเลือกเอง

## Failure handling
1. Inspect, 2. Safe-fix, 3. Retest — สูงสุด 3 retries ต่อสาเหตุ
4. ถ้าไม่ผ่าน BLOCKED และทำงานอิสระส่วนอื่นต่อ
5. ส่งคำถามเดียว พร้อม choices และ recommended path

## No-hang safety
ห้าม loop ไม่จำกัด, ห้ามซ่อนค่าใช้จ่าย, ห้ามอ้างว่าทำ background หากไม่มี automation/scheduler จริง, ห้ามแตะ Repo โปรดักชันเพราะ Prompt บอกว่า one-shot

**Default:** training Repo ให้ตั้งเป็น private ได้ และใช้ web UI / GitHub connector เท่านั้นถ้าเครื่องมือเพียงพอ ไม่ต้องดาวน์โหลดไฟล์
