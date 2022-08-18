# Kurulum
```js
npm i yunaz.db

index.js Main dosyasınız isimi neyse onun içine verdiğim şeyi ekleyin

const db = require('yunaz.db')
```

# Dosya Kurulumu 
```js
yunazdb Adlı bir Kklasör oluşturunuz ardından içine database.json adlı bir dosya oluşturun sonra bu dosyasının içine {} şu işareti atın ve hazır!
```

# Database Ekleme Yapma
```js
const db = require('yunaz.db')
db.add("İsim","Değer")

Burda Yazılacak Şey
{
  "İsim":"Değer"
}
```

# Databaseten Veri Çekme
```js
const db = require('yunaz.db')
let yunaz = db.fetch("İsim")
console.log(yunaz)

Az önce eklediğimiz veri İsim ve değeri Değer bizim konsolumuza burda Değer değeri dönecektir.
```

# Databaseten Veri Silme
```js
const db = require('yunaz.db')
db.delete("İsim")


Az önce  eklediğimiz veri İsim ve değeri Değer burda bunlar ailinecektir ve databaseinizde başka bir veri bhlunmuyorsa {} database.json dosyamız böyle gözükecektir 
```

# Databasete Veri Olup Olmadığını Kontrol Etme
```js
const db = require('yunaz.db')
db.has("İsim")

Burda değerimiz buluyorsa true bulunmuyorsa false değerini döndürecektir az önce sildigimiz için false döndürecektir 
```

# Matematik İşlemleri


```js
const db = require('yunaz.db')

db.math(2,"+",2) //4
db.math(2,"*",3) //6
db.math(3,"/",3) //1
db.math(3,"-",3) //0

```

# Hazır Olunca İşlem Döndürme


```js
db.on("ready",console.log("Database Hazır!")) //Konsola hazırım yazdırır

db.on("ready",db.add("yunaz","db")) //Database'e kayıt işlemi uygular
```

# Npm

<a href="https://www.npmjs.com/package/layon.db">Npm Linki</a>
<p>Developed By <a style="color:ORANGE" href="https://discord.com/users/920315243106795570">YunusDEV</a>
<li>Basit bir database modülüdür ve halen geliştirme aşamasında.</li>
