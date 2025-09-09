# iAM48-members

เก็บข้อมูล **Member BNK48 & CGM48** ในรูปแบบ JSON โดยดึงจาก API [`https://public.bnk48.io/members/all`](https://public.bnk48.io/members/all) และอัปเดตอัตโนมัติด้วย **GitHub Actions**  

## 📂 รายละเอียดโค้ด

- `members.json` — JSON สำหรับเก็บข้อมูล Member (จะถูก overwrite ทุกครั้งเมื่อมีการ fetch ข้อมูลใหม่)
- `fetch.js` — สคริปต์ สำหรับดึงข้อมูล Member ทั้งหมด แล้วบันทึกลง `members.json`
- `update.js` — สคริปต์ สำหรับอัปเดตข้อมูลเพิ่มเติม (Profile / SNS) โดยใช้ API จากภายนอก
- `update_ua.py` — สคริปต์ สำหรับอัปเดต User-Agent list
- `.github/workflows/fetch_api.yml` — Workflow ที่ดึงข้อมูล Member และ commit `members.json` กลับโดยอัตโนมัติ
- `.github/workflows/user_agents.yml` — Workflow สำหรับอัปเดต User-Agent list

---

📖 This project is **open source** — feel free to use, modify, and contribute.  
📖 โปรเจกต์นี้เป็น **โอเพนซอร์ส** — ยินดีให้ทุกคนนำไปใช้งาน ปรับปรุง และพัฒนาต่อได้อย่างอิสระ  

---

<div align="center">

🔗 Based on [oshi48](https://github.com/oshi48)  
✦ Built & maintained by **ptpofficialxd** ✦  
[GitHub](https://github.com/ptpofficialxd) | [X](https://x.com/ptpofficialxd)

</div>
