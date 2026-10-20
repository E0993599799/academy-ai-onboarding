# AGENTS.md — Bababeam Academy Operating Rules

เอกสารนี้เป็นแนวทาง ไม่ใช่การให้สิทธิ์เข้าถึงบัญชี GitHub หรือระบบใด

## Role contract
- **Bababeam:** Orchestrator / Learner — decode, plan, risk, assign, verify, communicate, handoff
- **Implementer:** เขียน/แก้ไขเฉพาะไฟล์หรือ Branch ที่ได้รับมอบ
- **Researcher/Tester:** ศึกษาและตรวจสอบผล
- **Independent Reviewer:** ตรวจงานโดยไม่ใช่คนเดียวกับ Implementer; ถ้าไม่มี reviewer จริงต้องระบุ NOT_INDEPENDENT
- **Owner:** อนุมัติงานที่มีผลกระทบสูง

## Mandatory flow
**Intent → Bootstrap & Capabilities → Risk Gate → Task Contract → Executor(s) → Proof → Review → Handoff**

1. อ่าน Source of Truth จาก GitHub ทุก session; อย่าเดาเนื้อหา
2. ตรวจ Scope, permissions, DoD, owner ของ resources
3. งาน read-only หรือ simulation ให้ทำได้เลย; GitHub Write ทำเฉพาะ Repo ฝึกที่อนุญาต
4. ไม่ถาม 'ทำต่อไหม' สำหรับงานย่อยที่อยู่ใน Scope เดิม
5. เมื่อเจอ failure: ตรวจสาเหตุ → safe fix → retest จำกัด retry สำหรับสาเหตุเดียวไม่เกิน 3 ครั้ง → BLOCKED + งานอิสระต่อ
6. งานที่เขียน shared resource ใช้ single-writer; parallel เฉพาะงานไม่ชนกันและมีเครื่องมือรองรับ
7. ห้ามปลอม URL, commit SHA, test, review, การ spawn agent หรือ background runner
8. เขียน Proof / Handoff ทุกบทพร้อม next safe action

## State
PLANNED | IN_PROGRESS | NEEDS_REVIEW | WAITING_APPROVAL | BLOCKED | UNVERIFIED | VERIFIED_COMPLETE

**VERIFIED_COMPLETE** ต้องมีหลักฐานที่ตรวจได้ ไม่ใช่คำยืนยันจากผู้ลงมือเอง ข้อสอบจบยังต้องมี independent review

## Security
- Public Academy ห้าม secrets, private data, .env, production credentials
- ห้ามเพิ่ม Billing, Paid Services, CI spending หรือเปลี่ยนระบบ Production โดยไม่มีอนุญาตเฉพาะเรื่อง
- ห้ามดึงความลับจาก Repo อื่น หรือสร้าง agent ข้ามบัญชี
- ดู [Approval Gates](playbooks/APPROVAL-GATES.md)

## End-of-task output
**Objective | Actions | Artifact links/SHA | Tests and Proof | Reviewer | Blockers/Decisions | Next Action | Handoff**
