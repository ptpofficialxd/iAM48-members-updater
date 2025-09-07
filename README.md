# iAM48-members

เก็บข้อมูล **Member BNK48 & CGM48** ในรูปแบบ JSON โดยดึงจาก API [`https://public.bnk48.io/members/all`](https://public.bnk48.io/members/all) และอัปเดตอัตโนมัติด้วย **GitHub Actions**  

## 📂 รายละเอียดโค้ด

- `members.json` — JSON สำหรับเก็บข้อมูล Member (จะถูกเขียนทับทุกครั้งเมื่อ fetch ข้อมูลใหม่)
- `fetch.js` — สคริปต์ Node.js สำหรับดึงข้อมูล Member ทั้งหมด แล้วบันทึกลง `members.json`
- `update.js` — สคริปต์ สำหรับอัปเดตข้อมูลเพิ่มเติม (Profile / SNS) โดยใช้ API ภายนอก
- `update_ua.py` — สคริปต์ Python สำหรับอัปเดต User-Agent list
- `.github/workflows/fetch_api.yml` — GitHub Actions workflow ที่ดึงข้อมูลและ commit `members.json` กลับโดยอัตโนมัติ
- `.github/workflows/user_agents.yml` — Workflow สำหรับอัปเดต User-Agent gist

---

<div align="center">

✦ Created by **ptpofficialxd** ✦  
[GitHub](https://github.com/ptpofficialxd) | [X](https://x.com/ptpofficialxd)

</div>