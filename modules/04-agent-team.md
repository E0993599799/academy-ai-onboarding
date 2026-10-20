# Module 04 — Agent Team & Delegation

**Day 7–8**

## รูปแบบทีม
- **Bababeam / Orchestrator:** decode, plan, assign, risk, coordinate, verify, handoff
- **Researcher:** หา requirements, constraints และอ้างอิง
- **Implementer:** เขียนเฉพาะ Scope/Branch ที่มอบหมาย
- **Tester:** รันทดสอบและรายงาน Fail
- **Independent Reviewer:** คนหรือ AI ต่างจาก Implementer ตรวจ diff/หลักฐาน; ถ้าไม่มี reviewer จริงห้ามอ้างว่า independent

## Delegation Contract
แต่ละงานต้องมี: Goal, Files/Branch, Owner, Tools confirmed, Forbidden Actions, Deadline/Retry bounds, Dependencies, Expected Output, Tests, Evidence, Handoff

## Exercise
แบ่งงาน Mini Todo Board เป็น: Research / UI Spec / Implementation / Tests / Review แล้วทำ Delegation Map, กำหนด Single Writer ต่อ shared files และ Acceptance Criteria

ถ้าเรียก Agent อื่นได้จริงให้มอบหมายตามสิทธิ์ที่มี ถ้าไม่มีให้ทำ **ROLE SIMULATION** ที่แยกบทบาท แต่ **ห้ามอ้างว่าเรียก agent หรือมี independent review จริง**

## Failure case study
1. Orchestrator เป็นคอขวดและทำทุกอย่างเอง
2. Agents สองตัวเขียนไฟล์เดียวกัน
3. Reviewer คือคนเดียวกับ Implementer
4. Agent ส่ง 'Done' ไม่มี SHA หรือ test proof

## Pass
ทุก task มี owner, boundaries, status, evidence; ทำ parallel เฉพาะงานไม่ชนกัน; ไม่สร้าง worker/runner โดยพลการ

**Next:** [Memory](05-memory-handoff.md)
