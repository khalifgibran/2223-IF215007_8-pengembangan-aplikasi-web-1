# Membuat Web Service Dengan Express JS

## Web Service dan RESTful API
- Q: Wah, sepertinya menarik. Apa tuh Web Service ?
- A: Web Service itu gerbang data yang terhubung dengan penyimpanan maupun komputasi di server untuk diakses langsung oleh bahasa pemrograman
- Q: Hmm, jadi konsumennya itu bahasa pemrograman ya ?
- A: Iya, kalo koran Tribun kan konsumennya orang, dibaca orang, web service pembaca utamanya bahasa kayak Javascript, Java, Ruby, Go, dsb.
- Q: Ohh IC IC, trus emang bisa ngapain aja pake Web Service ?
- A: Ya,, kamu bisa request kesitu, misalnya menggunakan HTTP REQUEST, nambah mobil POST /mobil, beli beras POST /belanjaan, liat list buah GET /buah, dsb.
- Q: Ohh gitu,, hmm,, itu cuma bisa pake HTTP ?
- A: Bisa pake yang lain juga kok kayak RPC, dan lain2 (browsing weh :D)
- Q: Oke2, wkwkwk. Trus apa tuh RESTful API itu ?
- A: Standar format web service HTTP berbasis [REST](https://glints.com/id/lowongan/rest-adalah/) dengan url yang merepresentasikan objek (bukan perintah). Misal, kalo mau beli makanan, ga pake url POST /beli-makanan, tapi pake url POST /pembelian, dan GET /pembelian ketika ingin lihat kita sudah belanja apa aja.

## Express JS
- Q: Oke2, trus apa hubungannya dengan praktikum kali ini ?
- A: Ya, kita bikin RESTful API menggunakan Express JS, framework Javacsript yang bisa dipakai untuk bikin web service (untuk mesin), maupun bikin web page (untuk orang)
- Q: Hmm, diinstall pake NPM ?
- A: Yoi, langsung aja dipraktekkan ya, sebelum install express, kita install dulu **nodemon**, **nodemon** ini dipake untuk eksekusi file javascript, mirip ama **node**, bedanya **nodemon** mantau perubahan filenya, dan auto restart kalo filenya diubah. Jadi ga usah repot stop start stop start kalo beres edit
```javascript
npm install -g nodemon  
```
- A: Diinstall nya pake tanda -g artinya global, diinstall disekomputereun. Agar dapat dipakai dari project2 lainnya
- A: Selanjutnya kita install pemeran utamannya, package Express JS, bareng dengan package tetangganya yang namanya cors yang memudahkan web service kamu diakses dari mana aja
```javascript
npm install cors express
```
