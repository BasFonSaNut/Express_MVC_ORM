# Express_MVC_ORM
การเขียน React-Expresss ภายใต้ concept MVC แก้ไข code จากแนวคิดต้นฉบับปี 2020 เนื่องจากอาจรันไม่ได้ ณ วันปัจจุบัน
แนะนำให้ไปดูแนวคิดกระบวนการ ที่ทำ step-by-step จนสุดท้ายสู่ปลายทาง MVC (อย่าเอาแต่โค้ดไปอย่างเดีย ให้ไปดูแนวคิดเขาเสมอ)

original Idea : https://www.youtube.com/playlist?list=PL4cUxeGkcC9jsz4LDYc6kv3ymONOKxwBU
original github sourcecode: https://github.com/iamshaunjp/node-crash-course
ตอนไปเอามาจากต้นฉบับ ให้ไปแก้ package.json ซึ่งของเดิมจะตั้งไว้ที่ server.js ซึ่ง ตั้งแต่ EP6 เป็นต้นไป จะไม่ใช้ server.js แล้ว
และใช้ nodemon ในการรัน ให้ไปแก้ ตาม comment ด้านล่าง

npm install --save #ลง package ทั้งหมดที่มีรายชื่ออยู่ใน package.json อย่าลืม --save ด้วย เพื่อไม่ต้องไปในลงใน node lib กลาง ต้องการใช้ให้มีผลในโปรเจคนี้เท่านั้น
npm install --save nodemon #ลง nodemon อย่าลืม --save ด้วย เพื่อไม่ต้องไปในลงใน node lib กลาง ต้องการใช้ให้มีผลในโปรเจคนี้เท่านั้น
แก้ไข package.json file at script part change to nodemon ถ้าหากไป load มาจากต้นฉบับด้วยตัวเอง หากใช้ตัวนี้ไม่ต้องแก้ไข เพราะแก้มาให้แล้ว
"main": "app.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "nodemon app.js"
  },

React-Express  MVC  ตัวนี้ แก้ไขส่วน Db มาใช้ที MongoDB ที่เครื่องตัวเอง แทนการใช้ MongoBB ของ Atlas (ฟรีไม่ต้องลง)
โดยเล็งเห็นว่า ก็มี cloud บางเจ้าให้ทำผ่าน ssh เพื่อไปนั่งเป็น admin ที่ MongoDB ได้เลย ไหน ก็จะเรียนรู้แล้วก็เรียนรู้การเป็น DB admin ไปด้วยในตัว
วันไหนไม่มีเน็ต ก็อย่างน้อยได้ใช้เครื่องตัวเองทำงานแทน
  install mongodb , use localhost instead Atlast
  DB username: MongoDB
  create database : name note-tuts, create collection : name Blog

run 
  npm start

ต้นฉบับ แนวคิดปี 2020 มารันตอนนี้อาจไม่สามารถรันได้
source code ฉบับ modify 2023 ตัวนี้ อยู่ที่ :  https://github.com/BasFonSaNut/Express_MVC_ORM 
