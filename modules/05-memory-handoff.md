# Module 05 — Memory Bootstrap & Cross-agent Handoff

**Day 9–10**

## หลักการ
Context ของแชทหนึ่งไม่ได้ส่งไปแชทใหม่โดยอัตโนมัติ ต้องใช้ Versioned Knowledge Source ที่อ่านซ้ำได้ แยก facts, decisions, lessons, progress และ handoff

## ใน Training Repo ของเจ้าของ
- README.md = Goal
- AGENTS.md = Working rules
- docs/DECISIONS.md = Decision + reasoning + rejected alternatives
- docs/STATUS.md = Current state + blockers + owners
- docs/LESSONS.md = What failed and why
- docs/HANDOFF.md = Last verified state + next action

## Exercise
1. สร้าง Mission A ใน Training Repo (หรือ simulation)
2. ทำงานครึ่งหนึ่งและเขียน [Handoff](../templates/HANDOFF.md)
3. ให้ AI/Session ใหม่อ่านเฉพาะ Repo แล้วสรุป Goal, Current SHA, Last proof, Blockers, Next safe action
4. Compare คำตอบกับ Source of Truth; ตกหล่นอะไรต้องบันทึก Lesson

หากไม่มี Session ใหม่ให้รายงาน FRESH_SESSION_NOT_TESTED ห้ามเดาว่าผ่าน

## Pass
Handoff อ่านแล้วสานงานต่อได้โดยไม่ต้องถามรายละเอียดเดิม; ไม่บันทึก secrets หรือข้อมูลส่วนตัวใน Repo สาธารณะ

**Next:** [Verification](06-verification-recovery.md)
