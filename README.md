# iRover
  ใช้สำหรับภาษา microPython ipst-WiFi + iKB <br>
  from irover  import * <br>
  i=IROVER() <br>
## การระบุขาใช้งาน
i0 - i7 เรียกใช้พอร์ตบนบอร์ด iKB <br>
## ตัวอย่าง อ่านค่าดิจิตอล 
  x= i.input(i5)   อ่านค่า input จากบอร์ด ikb พอร์ตหมายเลข 5 <br>
  x= i.input(5)   อ่านค่า input จากบอร์ด ipst-wifi พอร์ตหมายเลข 5
  x= i.IN(5)   อ่านค่า input จากบอร์ด ipst-wifi พอร์ตหมายเลข 5
 ## ตัวอย่าง กำหนดขาดิจิตอล 
  i.output(i5,1)   กำหนดลอจิก 1 ที่พอร์ตหมายเลข 5 บนบอร์ด iKB <br>
  i.output(5,1)   กำหนดลอจิก 1 ที่พอร์ตหมายเลข 5 บนบอร์ด ipst-wifi
  i.OUT(5,1)   กำหนดลอจิก 1 ที่พอร์ตหมายเลข 5 บนบอร์ด ipst-wifi
 
## ตัวอย่าง อ่านค่า Analog 
  จุดต่อที่สามารถ<br>
  x= i.analog(i5)   อ่านค่า analog จากบอร์ด iKB พอร์ตหมายเลข 5 การคืนค่า 0-1023 <br>
  x= i.analog(i5,-100,100)   อ่านค่า analog จากบอร์ด iKB พอร์ตหมายเลข 5 การคืนค่า -100 ถึง 100 <br>
  x= i.analog(34)   อ่านค่า analog จากบอร์ด ipst-wifi พอร์ตหมายเลข 34 การคืนค่า การคืนค่า 0-1023 <br>
# ตัวอย่าง คำสั่งมอเตอร์
## คำสั่งควบคุมมอเตอร์ช่อง 1 ให้เดินหน้า 100 %
k.motor(1,100)  
## คำสั่งควบคุมมอเตอร์ช่อง 2 ให้ถอยหลัง 100 %
k.motor(2,-100)                                                    
## คำสั่งควบคุมเซอร์โวมอเตอร์พอร์ต 15 ให้หมุนไปที่มุม 90 องศา
k.servo(15,90) 	
## เดินหน้า 100 %
k.fd(100) 	 
## ถอยหลัง 80 %
k.bk(80) 	  
## หมุนซ้าย 60 %
k.sl(60)
## หมุนขวา 40 %
k.sr(40) 	    
## เลี้ยวซ้าย 60 %
k.tl(60) 	 
## เลี้ยวขวา 60 %
k.tr(60) 	   
## เดินหน้าแบบปรับความเร็วแต่ละมอเตอร์ 1 = 100 % มอเตอร์ 2= 50 %
k.fd2(100,50) 
## ถอยหลังแบบปรับความเร็วแต่ละมอเตอร์ 1=  55 % มอเตอร์ 2= 50 %
k.bk2(55,50) 	  
## หยุดเคลื่อนที่
k.stop()	   
  
