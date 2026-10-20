# Module 06 — Proof, Review & Recovery

**Day 11–12**

## Evidence Ladder
- Claimed: AI พูดว่าเสร็จ = ไม่พอ
- Artifact: มี Issue/PR/Commit SHA จริง
- Tested: รัน Test และมี log/output
- Reviewed: ผู้ตรวจอิสระยืนยัน requirement กับ artifact
- Owner-visible: เจ้าของเปิดผลใช้งานจริงได้ (เมื่อภารกิจต้อง Deploy และได้รับอนุมัติแล้ว)

## Recovery Flow
Detect → Classify → Read logs/state → Backup (ก่อน destructive) → Safe fix → Retest → Report → Handoff

Max 3 safe retries ต่อ failure class; ไม่ใช้ infinite loop, ไม่ bypass security, ไม่แอบเพิ่มงบ

## Case studies
A: PR test fail
B: GitHub Write = 403
C: Git diff มี secret
D: Agents เขียนไฟล์เดียวกัน
E: ไม่มี reviewer หรือ runner จริง

สำหรับแต่ละกรณีให้ระบุ cause hypothesis, action, proof, risk, escalation, next safe step

## Pass
มี [Proof Report](../templates/PROOF.md) ระบุ PASS/FAIL/UNKNOWN และจัดการ blocker อย่างไม่ปลอมผล

**Next:** [Capstone](07-capstone.md)
