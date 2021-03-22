# Vanilla JS
javaScript의 한 종류로 라이브러리 없는 것을 의미함
<br><br><br>


 #### Variable (let, const)

* ES5 변수 : var<br>
* ES6 변수 : let(재할당 가능), const(=상수/재할당 안됨/선언과 동시에 할당되야 함) --- var의 단점 보완

 변수 선언할 때 기본적으로 const 사용. 재할당이 필요한 경우에 한정해 let 사용 습관
  
#### Data Type
<pre><code>
const whatString = 'reference';
const whatBoolean = true; //false
const whatNumber = 123;
const whatFloat = 12.3;
</code></pre>

String : "" or ''로 묶어준다.   
boolean : true, false   
Number : 숫자형   
float : 소수점   

#### Data with Arrays
 단순히 순서에 의해 나열함. 인덱스를 통해 요소에 접근함.
<pre><code>
const week = ['mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun']'

console.log(week); // mon tue wed thu fri sat sun   
console.log(week[1]); //tue   
console.log(week[10]); //undefined
</code></pre>

#### Data with Objects
 Key를 지정하여 Value 값을 담는다. 
<pre><code>
const arrayA = [1, 2, 3]
console.log(arrayA); // 1, 2, 3
console.log(arrayA[1]); // 1

const objectA = {
 name : 'reference',
 age : 32,
 contry: 'Korea',
 favAnimal : ['dog', 'cat'],
 favFood : [
  {name : 'hamburger'},
  {name : 'pizza'},
  {name : 'rice noodle'}
 ]
};

console.log(objectA);
console.log(objectA.age);

objectA.age = 40;

console.log(objectA.age);

objectA = ture;
</code></pre>
    
 object 타입의 변수에 참조 변수는 값 변경이 가능함
 objectA = true;를 통해 const로 선언된 변수에 재할당 불가능알 수 있음

