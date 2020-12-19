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
