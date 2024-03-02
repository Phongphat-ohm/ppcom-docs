
# Truemoney Wallet Angpao API
โปรเจกต์ Truemoney Wallet Angpao API  เป็นผู้ให้บริการการเชื่อมต่อระบบทรูมันนี่วอเลทเท่านั้น ไม่มีส่วนเกี่ยวข้องใดๆ กับบริษัท ทรู มันนี่ จำกัด

## วิธีการติดตั้งลง Website ของคุณ
1. สมัครสมาชิกที่ Website
2. เข้าสู่ระบบ รับค่า APIKEY
3. ขอ API ไปที่ server

### ขั้นตอนที่ 1 สมัครสมาชิกที่ Website
* เข้าไปที่ Website [PPCOM](https://ppcom.vercel.app)
    * กดปุ่มสมัครสมาชิก
    * กรอก หมายเลขโทรศัพท์ ชื่อผู้ใช้ รหัสผ่าน

### ขั้นตอนที่ 2 เข้าสู่ระบบ
* กรอกชื่อผู้ใช้และรหัาผ่าน
* หลังจากเข้าสู่ระบบสำเร็จ
    * กดปุ่มคัดลอก APIKEY มา


### ขั้นตอนที่ 3  ขอ API ไปที่ server
```sh
curl --location 'https://ppcom-server.vercel.app/api/topup' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MSwiaWF0IjoxNzA5MzAxNTMyfQ.RHQ4AC64TdIasf3gQjDcolNqxof4F2u0nvUYNE_Z_Nw' \
--data '{
    "code": "https://gift.truemoney.com/campaign/?v=eab53f0f7ea54bf287cca2b28829635a578"
}'
```

#### ข้อมูลค่าที่สมารถตอบกลับ
![response](https://github.com/Phongphat-ohm/ppcom-docs/blob/main/code_20240302_222242_via_10015_io.png?raw=true)
