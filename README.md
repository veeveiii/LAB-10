#ใบงานที่ 10
##การเขียนโปรแกรมกราฟฟิกส์ด้วย GDI+ (2)
##กล่าวนำ
ใบงานนี้ มีวัตถุประสงค์ เพื่อให้นักศึกษา ได้รู้จักกับ GDI+ ซึ่งจะช่วยให้นักษาสามารถ
* วาดรูปร่างต่างๆ โดยใช้ GDI+ ได้


## การวาดเส้นตรง
การวาดเส้นตรง เป็นการเชื่อมต่อระหว่างจุด จำนวน 2 จุด  โดยใช้ออบเจกต์ Pen เป็นตัวกำหนดลักษณะของเส้น 

แก้ไข code ต่อไปนี้ในฟังก์ชัน private void Form1_Paint(object sender, PaintEventArgs e)
* [Graphics.DrawLine Method](https://msdn.microsoft.com/en-us/library/system.drawing.graphics.drawline(v=vs.110).aspx)

<p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-1.png">
</p>

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15135643_1142001425920107_229483349_n.png?oh=3202ff5b3a7da59cd6797c10b1ffab79&oe=583180D7)
<hr>
## การวาดเส้นตรงด้วย pen style และ brush
* [PenType Enumeration](https://msdn.microsoft.com/en-us/library/system.drawing.drawing2d.pentype(v=vs.110).aspx)
 <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-2.png">
</p>

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15134414_1142001429253440_1602962741_n.png?oh=eec5e66c22212b9ba3415579969282cf&oe=58316504)
<hr>


## การกำหนดจุดปลายของเส้นตรงด้วย style แบบต่างๆ

* [LineCap Enumeration](https://msdn.microsoft.com/en-us/library/system.drawing.drawing2d.linecap(v=vs.110).aspx)
<p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-3.png">
</p>

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15086231_1142001452586771_1797168829_n.png?oh=606c870c973fcbac857d00fabc979dbb&oe=58305B7D)
<hr>


##การวาดเส้นโค้ง
การวาดเส้นโค้ง ทำได้โดยการกำหนดจุดไว้ใน array ของ point แล้วส่งให้กับฟังก์ชัน DrawCurve ดังตัวอย่างต่อไปนี้
<p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-4.png">
</p>

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15087012_1142001455920104_123035526_n.png?oh=4b888eb9abdedba1b630a4f430bd17ae&oe=583096A4)
<hr>

## การวาดเส้นโค้งด้วย Graphics path
 <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-5.png">
</p> 

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15135535_1142001439253439_1749180883_n.png?oh=652992cab5dac61d26175ac4162c3b8b&oe=5830AE90)
<hr>

## การวาดรูปทรงสี่เหลี่ยม
### การวาดสี่เหลี่ยมครั้งละรูปเดียว
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-6.png">
</p> 

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15058685_1142001442586772_82364502_n.png?oh=f2ce245178aeb86cf9cfa04d778bf482&oe=58317108)
<hr>


###การวาดสี่เหลี่ยมพร้อมกันครั้งละหลายๆ รูป
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-7.png">
</p> 

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15058655_1142001445920105_1158115889_n.png?oh=2479fa8dd92d2bb2c4c4606e9c0a36b0&oe=58316DC0)
<hr>


## การวาดวงกลมและวงรี
วงรีต่างจากวงกลมตรงที่เส้นผ่านศูนย์กลางในแกนตั้งและแกนนอนจะไม่เท่ากัน ในภาษาโปรแกรมส่วนใหญ่จะมีเฉพาะฟังก์ชันวาดวงรี ถ้าต้องการวาดวงกลม ให้กำหนดเส้นผ่านศูนย์กลางในแกนตั้งและแกนนอนให้เท่ากัน
   <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-8.png">
</p> 

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15087045_1142001435920106_1854138544_n.png?oh=a63e8a97809eea271bf2a4bbdef1bfed&oe=583071DF)
<hr>


## การวาดส่วนโค้ง (Arc)
   <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-9.png">
</p> 

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15134262_1142001449253438_1514897104_n.png?oh=c5eabce69a1c6d85faceefc79084160d&oe=58318497)
<hr>


## การวาดรูป Pie
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-10.png">
</p>  

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15086291_1142001432586773_1499529925_n.png?oh=a02d5d6acb48f1d6387da4cab29fe6f1&oe=58305360)
<hr>

## การสร้าง graphics path จากรูปต่างๆ 
  <p align="center">
<img src= "https://github.com/Desktop-Programming-Lab-2559/LAB-10/blob/master/imgs/lab10-11.png">
</p>  

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t34.0-12/15139348_1142001465920103_1491681405_n.png?oh=77c880636fe65e4b1efc8050ae179fc2&oe=58316EBB)
<hr>

#แบบฝึกหัด
ให้วาดรูปวิว โดยใช้รูปร่างต่างๆ ที่ทำการทดลองใน Lab นี้

###ผลการทดลอง
![](https://scontent.fbkk2-3.fna.fbcdn.net/v/t35.0-12/15126066_1142015035918746_1446580344_o.png?oh=e0b12d880ef404e3ed45ca5a431ee451&oe=58304469)
<hr>

##เอกสารอ้างอิง
### [Graphics Methods](https://msdn.microsoft.com/en-us/library/system.drawing.graphics_methods(v=vs.110).aspx)
### [System.Drawing Namespace](https://msdn.microsoft.com/en-us/library/system.drawing(v=vs.110).aspx)
### [GDI+ .NET Color & HatchStyle Chart](https://drewnoakes.com/snippets/GdiColorChart/)

<hr>
<hr>
Ailada Samingkaew 57030249 
<hr>
<hr>

