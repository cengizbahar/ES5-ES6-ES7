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
```
