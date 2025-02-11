---
layout: post
title: "[React]객체와 배열의 사용성 개선"
date: 2025-02-10 11:00:59
modified: 2025-02-10 11:00:59
tag: [React, JavaScript]

---

자바스크립트 작성시 단축 속성명과 게산된 속셩명을 이용하여 객체와 배열을 생성하고 수정하는 방법과
또 전개연산자와 비구조화할당을 이용한 객체와 배열의 속성값을 밖으로 쉽게 꺼내는 방법에 대해 아래와 같이 정리해 보았다.


## 단축 속성명과 게산된 속성명
### 단축 속성명
```JavaScript
const name = "Alice";
const age = 25;

const person = {
  name: name, // 중복된 변수명
  age: age
};

console.log(person); // { name: "Alice", age: 25 }
```
객체를 생성할때 속성명과 변수명이 동일하다면, 생략된 형태로 작성할 수 있다.
```JavaScript
const name = "Alice";
const age = 25;
const person = { name, age }; // 속성명을 생략하면 자동으로 변수명이 속성명이 됨

console.log(person); // { name: "Alice", age: 25 }
```

### 계산된 속성명
```JavaScript
function makeObject(key, value) {
  const obj = {};
  obj[key] = value;
  return obj;
}
```
계산된 속성명은 아래와 같이  객체의 속성명을 동적으로 결정할 수 있다. 
```JavaScript
function makeObject(key, value) {
  return ([key] : value);
}
```
## 전개연산자와 비구조화할당
### 전개연산자
전개연산자는 배열이나 객체의 모든 속성을 풀어놓을때 사용할 수 있다. 매개변수가 많은 함수를 호출할때 유용하며, 배열이나 객체를 복사할때도 유용하다.
배열에서 전개연산자를 사용하면 순서가 유지되며 중복된 속성명을 사용하면 최종결과는 마지막 속성명의 값이 된다.

```JavaScript
const sample1 = {a:1, a:2, b:3} // {a:2, b:3}
const sample2 = {...sample1, b:4} // {a:2, b:4}
```


### 비구조화할당
#### (1) 배열 비구조화
배열의 여러 속성값을 아래와 같이 변수로 쉽게 할당할 수 있다
```JavaScript
const arr = [1, 2]
const [a, b] = arr;
console.log(a); // 1
console.log(b); // 2
```

#### (2) 객체 비구조화
객체의 여러 속성값을 변수로 쉽게 할당할 수 있다. 단 배열 비구조화에서는 왼쪽 변수의 이름을 임의로 지정할 수 있지만 객체에서는 기존 속성명 그대로 사용해야 한다.

```JavaScript
const obj = {age:21, name: 'mike'}
const {age, name} = obj; // age:21, name: 'mike'
const {name, age} = obj; // age:21, name: 'mike'
const {a, b} = obj; //undefined
```
객체 비구조화에서 순서는 무의미하며 존재하지 않는 속성명을 사용할 경우 `undefined`가 할당된다.

이처럼 코드를 작성할때 배열과 객체를 얼만큼 활용할 수 있느냐에 따라 코드 작성이 용이해지며 가독성 또한 높여줄 수 있다.
