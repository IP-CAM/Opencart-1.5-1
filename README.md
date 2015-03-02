# Opencart-1.5
Opencart 1.5

ขั้นตอนการติดตั้ง...
Patsolutions PaymentGateway กับ Opencart 1.5

1. ทำการ  copy Folder /admin  และ Folder /catalog ไปทับ folder เดิมใน ระบบ

2. เข้าไปในส่วนของ admin ไปที่ ส่วนเสริม->การชำระเงิน ->Paysolutions  ทำการ ติดตั้ง
หรือ  ไปที่  Extensions -> Payments -> Paysolutions ทำการติดตั้ง

3. เมื่อติดตั้งเสร็จ ทำการแก้ไข E-mail  - >  E-mail เอาไว้รับ Order ที่สมัครกับทาง Paysolutions 
 Merchant  - > Merchant 8 หลัก ที่ได้จากการสมัครใช้งานกับ Paysolutions
entry_order_status  - >  กำหนดสถานะเมื่อจ่ายเงิน สำเร็จ [ ให้ตั้งเป็น Complete ] 
Status  - >  เปิดใช้งาน PaymentGateway [ ให้ตั้งเป็น Enable ]
Sort Order  - >  การตั้งลำดับของ Payment Gateway

ในส่วนของ  https://control.thaiepay.com/
 
เมนู  ระบบการทำงาน -> การส่งค่ากลับ
Post Back Url  :  -> 
Your Domain.com/index.php?route=payment/paysolutions/callback
กำหนด พารามิเตอร์เพิ่มเติม  
Name : -> status
Value : -> CP

