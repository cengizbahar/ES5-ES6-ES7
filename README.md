# ES5-ES6-ES7
### http://kangax.github.io/compat-table/es5/


## Visual Studio Code Eklentiler
- Live Server
- JavaScript (ES6)
- One Dark Pro

## Değişken Türleri var , let , const

- var : Her yerde kullanılabilir
- let : Değiştirilebilir
- const : Değiştirilemez
- typeof : Türünü kontrol eder

```
// var

var x;
x = "mustafa";
console.log(x);

// let

let fullname="Cengo";
console.log(fullname);
fullname="bahar";
console.log(fullname);

// const

const email="cengiz@gmail.com";
console.log(email);


// typeof

console.log(typeof email);



```
## Primitive Types undefined , null , string , number , boolean
- boolean : Kadın Erkek , iki türü tespit etme, true false

```
// undefined
var x;

// null
var y = null;

// string
var name = "cengiz";

// number
var yas = 36;

// boolean
var online = true;

```

## Reference Types - Objects
- array : Diziler
- objects : Nesne
- function
```
// array
var cars = ['Reno','BMW']

// objects
var person = {
  name : "cengiz",
  age  : "28"
}

// function
var isAlive = function(){
  return: 0;
}


```

## Operatörler 
- % (mod) işareti : kalan , tek ve çift gibi unsurları bulmaya yarar
```
var sonuc;
const x = 60;
const y = 12;

// Aritmetik  Operatörler

sonuc = x + y;
sonuc = x-y;
sonuc = x * y;
sonuc = x / y;

// Kalan gösterme

sonuc = x % y; 
sonuc = x % z;

sonuc = z++; // sayıyı 1 arttırdı ancak hafızada 8 olarak tuttu
sonuc = ++z; // sayıyı 1 arttır ekrana yazdırdı.

sonuc = z--; // 8 olarak hafızada tuttu
sonuc = --z; // 7 olarak yazdırdı

// Atama Operatorleri

sonuc = x; // 60 degeri sonuca aktarılır
sonuc += x; // sonuc = sonuc + x
sonuc -= x;

sonuc *= x;
sonuc /= x;
sonuc %= x;


// Karşılaştırma Operatorleri

let z = 9;
let t = 9;

sonuc = z == t; // dogru ise true yanlış ise false
sonuc = z === t; // typeof kontrol ediyor

sonuc = x != y // 60 != 12 olduğundan true döndürdü
sonuc = z != t // 9 = 9 oldugundan false döndürdü

z = 5;
t = 7;
sonuc = z > t;
sonuc = z < t;
sonuc = z >= t;
sonuc = z <= t;


// Mantıksal Operatorler

// && ( and = ve) şartların ikiside sağlansın
sonuc = (z > t) && (x > y)

// ||  (or = veya ) şartlardan biri sağlansın
sonuc = (z > t) || (x > y)

// ! (not = değil)
sonuc = !(z > t)

```
## Date Object
```
var d = new Dat();
console.log(d);

// set methods
d.setFullYear(1996);
d.setMonth(10);
d.setDate(25);


// get methods
console.log(d.getFullYear());
console.log(d.getMonth()); // 6. indis temmuza denk geliyor
console.log(d.getDate());
console.log(d.getHours());
console.log(d.getMinutes());
console.log(d.getSeconds());
console.log(d.getMilliseconds());
console.log(d.getDay()); // pazar günü 0. indis

```

## String Metotları
```
const ad = "cengiz";
const soyad = "bahar";

var x = ad + ' ' + soyad;


// string concat 
  x = ad.concat(' ',soyad); // birleştirme

// string length
  x = ad.length;
  x = soyad.length;

// string UpperCase & LoverCase
  x = ad.toUpperCase(); // harfleri büyütmek
  x = ad.toLoverCase(); // harfleri küçültmek

//string indexof
  x = xindexOf('x');  harf sırası bulma

// string substring
  x = x.substring(0,5); // 5. den itibaren
  x = x.slice(7); // 7. den itibaren harfleri almak

// string replace
x = x.replace('Mustafa','Cengiz'); // Yer değiştirme methodu


console.log(x);
```
## Number Methotları
```
var x = 10;
x = "10";


x = Number ('10x'); // numbere dönüştürme
x = isNaN('10x');

//  parseInt parseFloat
var sayi = 24.2324;

sayi = parseInt(sayi); // sayımızı int e dönüştürme
sayi = parseFloat(sayi); // sayinin tamamını alıyor

//  preccision fixed

sayi = sayi.toPrecision(2); // sayi elemanını 2 adetini ya da 5 adetini gibi şeyleri alabilip ekrana yazabiliriz
sayi = sayi.toFixed() // virgülden sonrasını atar

// Math Metotları 
var y = 64;

sayi = Math.PI; // Pi sayısı
sayi = Math.round(2.8); // Yuvarlama 3 e eşitler
sayi = Math.ceil(3.8); // Yukarı yuvarlar
sayi = Math.floor(4.9); // Aşşağıya yuvarlar
sayi = Math.sqrt(y) // Karekök hesaplama
sayi = Math.pow(2,4) // Üslü sayıları bulma 2 üzeri 4
sayi = Math.abs(-150); // Pozitif sayı alma mutlak deger

sayi = Math.min(32,54,12,74,3,8,13,43); // En düşük sayıyı getirme
sayi = Math.max(32,54,12,74,3,8,13,43); // En büyük sayıyı getirme

sayi = Math.random()*100; // Rastgele sayı üretir
sayi = Math.round(Math.random()*100)+1; // Küsürat almadan yuvarlayarak rastgele sayı üretir


console.log(x);
console.log(typeof x);
```
## Arrays  ( Dizi )
```
var country = ['Türkiye', 'Bg','Yunanistan'];

var numbers = [15,25,35,29,24];

var cn = ['Türkiye' , 15, null , undefined, ['Cengiz',23]];

// get arrays
console.log(contry[0]); // 0 elemanı çağırdık

// set arrays

country[0] = 'Bursa'; // 0. indisi değiştirdik

country[country.length] = 'samsun'; // sonuncu elemanı yazmak

// add arrays item
country.push(19); // son elemandan sonrasına eklemek
country.push('bahar'); // son elemana string

country.unshift(23); // başa ekleme

// remove arrays item
country.pop(); // sondaki elemanı silme
country.shift(): // en baştaki elemanı silme

//reverse (Ters Çevirme)
.country.reverse(); // terse yazma

// sort
country.sort(); // alfabetik sıraya göre sıralama

// concat (iki diziyi birleştirme)
var x = country.concat(numbers);


console.log(country);
console.log(typeof country); // türünü gösterir
console.log(country.length); // kaç adet olduğunu gösterir
```
## KOŞUL İFADELERİ

```
// if else ifadeleri

var name = "cengiz";
var age = 23;
var drivingLicence = true;

if(name == 'cengiz')
{
  console.log('benim adım Cengiz');
}

if(yas ==)
else {
  console.log('Araç Kullanamazsın')
}

age = 15; // iç içede if else açabiliriz

if( age > 18) {
  console.log('araç kullanabilirsiniz');
}
else {
  console.log('18 yaşından küçükise araç kullanamazsınız')
}


```

## Switch Statements
- Break ifadesini koymalıyız koymazsak her iki durumuda yazacaktır
```
let category = "coffee";

switch(category) {
  case 'coffee';
    console.log('Sade Kahveniz Hazırlanıyor.);
    break;
  case 'coffemilk';
    console.log('Sütlü Kahveniz Hazırlanıyor');
    break;
   default : 
    console.log('Hatalı kategori seçtiniz');
}

let day ;
switch (new Date().getDay()){
  case 0:
    day = 'Pazar';
    console.log('Bugün Günlerden' + day);
    break;
  case 1:
    day = 'Pazartesi';
    console.log('Bugün Günlerden' + day);
     break;
  case 2:
    day = 'Salı';
    console.log('Bugün Günlerden' + day);
     break;
  case 3:
    day = 'Çarşamba';
    console.log('Bugün Günlerden' + day);
     break;
  case 4:
    day = 'Perşembe';
    console.log('Bugün Günlerden' + day);
     break;
  case 5:
    day = 'Cuma';
    console.log('Bugün Günlerden' + day);
     break;
  case 6:
    day = 'Cumartesi';
    console.log('Bugün Günlerden' + day);
     break;
}

```
## Loops ( Döngüler )
```

// while
-----------------------------------
let i = 0;
while (i<10) {
  console.log(i);
  i++;
}
-----------------------------------

//do-while Loops
-----------------------------------
let i = 0;
do{
  console.log(i);
  i++;
}
while(i<10) {
  console.log("Döngü Bitti");
}
-----------------------------------

// for 3 deger giriyor
-----------------------------------
- continue : işlemi tamamladım diğer satırları es geç döngüyü devam ettir
- break : kendinden sonrakileri yazmıyor

for(let i=0; i<10; i++){
 if(i==2) {
  console.log('iki =' +i);
  continue;
 }
 if (i==5) {
  console.log('beş =' + i); 
  break;
  }
 console.log(i);
}

-----------------------------------
// iç - içe for döngüleri içeriden başa dönüyor

for (let i 10; i>0; i--) {
  console.log('i = ' i);
  for(let j=0; j>5;j++) {
    console.log('j =' +j);
  }
}


```

## Template Literals 
```
Eski Yöntem
-----------------------------------
const fullName = "Cengiz Bahar";
const city = "Turkiyede";
const yearOfBirth = 1992;

let val = 'Benim adım' + fullName + city + 'yaşıyorum' + (2020-yearOfBirth) + 'yaşındayım'.

console.log(val);

-----------------------------------
// Template Literals Yeni
: veya
? kontrol etsin


val = `Benim adım ${fullName}. ${city} yaşıyorum. ${(2020-yearOfBirth)} yaşındayım.`
console.log(val);
```
## Object Literals
```

let person = {
  firstName : 'Cengiz',
  lastName : 'Bahar',
  age : 28,
  hobbies : ['music','csgo'],
  adress : {
    city : 'Kocaeli',
    country: 'Türkiye'
  },
  getBirthYear : function() {
    return 1992-this-age;
  }
}

Bu şekilde objemize erişim sağlayabiliriz.

let val;
val = person;

val = person.firstName;
val = person.lastName;
val = person.age;
val = person.hobbies[1];
val = person.adress.city;
val = person.getBirthYear();


let people = [
  {
    firstName : 'Erva',
    lastName : 'Kaba'
  },
  {
    firstName : 'Mergül',
    lastName : 'Bahar'
  }
  
  
]
console.log(person);

```

## Diziler

```
let cars = ['BMW','Mercedes','Audi'];

for (let i = 0; i < cars.length; i++) {
  console.log(cars[i]);
}

//Array
// for-in
-----------------------------------

for(let i in cars) {
  console.log(`index : ${i},value:  ${cars[i]}`);
}
console.log(typeof cars);

-----------------------------------


let people = [
  {
    firstName : 'Erva',
    lastName : 'Kaba'
  },
  {
    firstName : 'Mergül',
    lastName : 'Bahar'
  }  
  
]

// for
-----------------------------------

for(let i = 0; i<people.length; i++) {
  console.log(people[i].firstName);
}


// in
-----------------------------------

for ( let i in people) {
  console.log(`index: ${i},  value : ${people[i].firstName}`);
}


// forEch
-----------------------------------

people.forEach(function (item) {
  console.log(item.lastName);
});


```

##  Functions (Fonkisyonlar)
```
  function karesiniAl(sayi) {
    return sayi*sayi;
  }
  
  let a = karesiniAl(2); // a değeri 4 olacak
  let b = karesiniAl(4); // b değeri 16 olacak
  
  console.log(a);
  console.log(b);
  
  -----------------------------------
  
  function toplam (sayi1,sayi2) {
    function karesiniAl(x) {
      return x*x;
    }
    return karesiniAl(sayi1) + karesiniAl(sayi2);
  }
  let sonuc = toplam(2,4);
  console.log(sonuc);
  
```

##  Function Declaration
```
// Function Declaration
 -----------------------------------
  function sum(a,b) {
    var c = a + b;
    return c;
  }
  console.log(sum(10,20)); 
 
 
//Function Expression  Sıklıkla Kullanılıyor
 -----------------------------------
 const sum = function (a=0,b=0) {
  var c = a + b;
  return c;
 }
 console.log(sum(10,20));
```


## Window Object

```
let val;
var a = 10;
val = window;

val = window.location.href; // sitelinkini alıyor
val = window.location.hostname; // host adresini yakalıyor


console.log(val);

```




