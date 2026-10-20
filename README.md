# THAM AI Orchestrator Academy × Bababeam

**สอน AI ให้ใช้ GitHub วางแผน มอบหมาย Agent Team ตรวจงาน และส่งต่อความรู้ — 100% ออนไลน์ ไม่ต้องดาวน์โหลดไฟล์**

สวัสดี **น้องของพี่เอก** และ **Bababeam**! จุดประสงค์ของ Academy นี้คือสอนให้ Bababeam ได้รับโจทย์ **ครั้งเดียว** แล้วทำงานย่อยทุกอย่างที่ปลอดภัยและอยู่ในขอบเขตที่ได้รับอนุญาตต่อได้เองจนมีผลลัพธ์ตรวจสอบได้ โดยไม่ถามว่า “ทำต่อไหม?” ซ้ำ ๆ

> **One-shot ไม่ใช่อนุมัติทุกอย่าง:** Bababeam ต้องขออนุญาตเมื่อมีการใช้เงิน เพิ่มสิทธิ์บัญชี เปิดเผยข้อมูลส่วนตัว ลบข้อมูล ส่งข้อความภายนอก Merge/Deploy ของจริง หรือการตัดสินใจสำคัญอื่น ๆ

## สำหรับน้องของพี่เอก — เริ่มใน 3 ขั้นตอน

1. เปิด Repo นี้: https://github.com/E0993599799/academy-ai-onboarding
2. เปิด [START-BABABEAM.md](START-BABABEAM.md) เพื่อดูคำสั่งเริ่มเรียนที่เตรียมไว้
3. ส่งลิงก์ Repo นี้และคำสั่งต่อไปนี้ให้ Bababeam **เพียงครั้งเดียว**:

> Bababeam อ่าน https://github.com/E0993599799/academy-ai-onboarding โดยเริ่มจาก README.md → START-BABABEAM.md → AGENTS.md → CURRICULUM.md → บทเรียน แล้วเริ่มเรียน Day 1 เลย ทำต่อเองทุกขั้นที่ปลอดภัยและมีสิทธิ์ ไม่ต้องถามยืนยันซ้ำ ยกเว้นการตัดสินใจสำคัญ รายงานผลพร้อมหลักฐาน GitHub และ Handoff

**ไม่ต้อง Clone, โหลด ZIP, ติดตั้งโปรแกรม หรือใช้ไฟล์ภายในเครื่องเพื่ออ่านหลักสูตร** ขอเพียง AI ที่เปิดลิงก์ GitHub ได้ การฝึกเขียน GitHub จริงต้องใช้บัญชีและสิทธิ์ของน้อง หรือ Repo ฝึกที่เจ้าของอนุญาต

## สำหรับ Bababeam — ต้องทำทันที

- อ่าน [คู่มือเริ่มต้น](START-BABABEAM.md), [กติกาการทำงาน](AGENTS.md), [หลักสูตร](CURRICULUM.md), [One-Shot Playbook](playbooks/ONE-SHOT.md) โดยเปิดจาก GitHub จริง
- ตรวจ Capability: อ่านเว็บ/อ่าน GitHub/เขียน Repo/Issue/PR/รันโค้ด/สร้าง Agent/Memory/Runner พร้อมหลักฐาน
- เริ่มบทเรียนที่ 1 โดยไม่ต้องถามว่า “พร้อมไหม?”
- ทำต่อส่วนที่ปลอดภัยได้เอง, ถ้าเขียน GitHub ไม่ได้ให้ simulation แบบซื่อสัตย์; อย่าแต่งลิงก์หรือแกล้งทำว่าได้เรียก Agent
- ถ้าติด Approval Gate ให้ถามเป็น **หนึ่งคำถามที่จำเป็นพร้อมตัวเลือก** และทำงานอิสระส่วนอื่นต่อ
- จบบทด้วย **Objective | Actions | Evidence | PASS/FAIL/UNVERIFIED | Blocker | Next Step | Handoff**

## แผนเรียน 14 วัน (เลื่อนขั้นตามหลักฐาน)

| วัน | Module | หลักฐานที่จะได้ |
|---|---|---|
| 1–2 | [พื้นฐาน AI และสิทธิ์](modules/01-foundations.md) | Capability + Risk Map |
| 3–4 | [GitHub](modules/02-github.md) | Issue → Branch → Commit → PR |
| 5–6 | [Planning](modules/03-planning.md) | Task Contract / Acceptance |
| 7–8 | [Agent Team](modules/04-agent-team.md) | Delegation / Ownership |
| 9–10 | [Memory & Handoff](modules/05-memory-handoff.md) | Fresh-session handoff |
| 11–12 | [Verification & Recovery](modules/06-verification-recovery.md) | Tests / Proof |
| 13–14 | [Final Capstone](modules/07-capstone.md) | PR + Review + Report |

ใช้ 14 วันเป็นเป้าหมาย ไม่ใช่รับประกันความสามารถ AI ทุกแพลตฟอร์ม เรียนและผ่านตามการประเมินจริง

## เอกสารสำคัญ

- [Bababeam: Start Here](START-BABABEAM.md) · [Agent Rules](AGENTS.md) · [Curriculum](CURRICULUM.md)
- [สั่งครั้งเดียว](playbooks/ONE-SHOT.md) · [เมื่อไรต้องขออนุมัติ](playbooks/APPROVAL-GATES.md)
- [Task Contract](templates/TASK-CONTRACT.md) · [Handoff](templates/HANDOFF.md) · [Proof Report](templates/PROOF.md)
- [คะแนนสอบ](assessments/RUBRIC.md) · [ตัวอย่างภารกิจ](examples/DEMO-MISSION.md)

## ขอบเขตความปลอดภัย

Repo นี้ **Public**: ห้ามใส่ Token, Password, .env, ข้อมูลลูกค้า, Private Repo, บทสนทนาส่วนตัวหรือเอกสารบริษัทลงในไฟล์/Issues/PR

**อย่าใช้ Repo หลักสูตรนี้เป็นสนามฝึกเขียน** ให้ใช้อีก Repo ที่น้องเป็นเจ้าของและอนุญาต (ตั้งเป็น private ได้) ไม่มีการเชื่อมสิทธิ์เข้ากับโปรเจกต์ Forge/BPMP/Production ของคนอื่นโดยอัตโนมัติ ไม่มีค่าใช้จ่ายจำเป็นและห้ามเปิด Paid Services เอง

**Done = มีหลักฐานตรวจได้** · ถ้าไม่มี Tool/Scheduler จริง ต้องแจ้งข้อจำกัดตามตรง ไม่สัญญาว่าจะทำงานเบื้องหลังได้เสมอ

**รุ่น 1.0 • Bababeam Online Academy**
