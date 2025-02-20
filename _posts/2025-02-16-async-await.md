---
layout: post
title: "[JavaScript]Callback, Promise, async await 차이점"
date: 2025-02-16 11:00:59
modified: 2025-02-16 11:00:59
tag: [JavaScript]

---

## async await
async await는 비동기 프로그래밍을 동기 프로그래밍처럼 작성할 수 있도록 함수에 추가된 기능이다.


### 동기와 비동기
#### 동기(Synchronous)
- 동기 작업은 순차적으로 진행된다. 하나의 작업이 완료될때까지 다음작업이 실행되지 않는다.

#### 비동기(Asynchronous)
비동기 작업은 병렬적으로 진행된다. 결과가 나올때까지 기다리지 않고 다른 작업을 계속할 수 있다.

### 1. Callback 함수
비동기 작업이 완료되었을때 실행할 함수를 전달하는 패턴으로 주로 다른 함수가 비동기 작업을 수행한 후 호출된다.
콜백 지옥이라 불리는 코드 가독성 및 유지보수 문제를 일으킬 수 있고, 복잡한 비동기 작업을 다루기 어렵다.

```javascript
function asyncTask1() {
  return new Promise((resolve) => {
    setTimeout(() => {
      console.log("Task 1 완료");
      resolve("result1");
    }, 1000);
  });
}

function asyncTask2(prevResult) {
  return new Promise((resolve) => {
    setTimeout(() => {
      console.log("Task 2 완료, 이전 결과:", prevResult);
      resolve("result2");
    }, 1000);
  });
}

function asyncTask3(prevResult) {
  return new Promise((resolve) => {
    setTimeout(() => {
      console.log("Task 3 완료, 이전 결과:", prevResult);
      resolve("result3");
    }, 1000);
  });
}

//callback hell
```

## 2. Promise
콜백 헬로인해 ES6에서 비동기처리를 위한 또 다른 패턴으로 도입되었다. 비동기 처리 시점을 명확하게 표현할 수 있는 장점이 있다.
Promise는 세가지의 상태를가질 수 있고 비동기 작업의 성공 또는 실패를 처리하기 위한 then(), catch() 매서드를 제공한다.
프로미스는 비동기 상태를 값으로 다룰 수 있기 때문에 async await 보다 큰 개념이다. 


```javascript
asyncTask1()
  .then(result1 => asyncTask2(result1))
  .then(result2 => asyncTask3(result2))
  .then(finalResult => console.log("모든 작업 완료:", finalResult))
  .catch(error => console.error("Error:", error));
  // promise 체이닝 사용
```

## 3. async-await
promise가 자바스크립트 표준이된 2년 후에 async await도 자바스크립트의 표준이 되었다. async await을 이용하여 비동기 코드를 작성하면 프로미스의 then 매서드를 체인 형식으로 호출하는 것보다 가독성이 좋아진다. async 함수는 비동기 작업을 수행하고 await 키워드를 사용하여 promise 완료를 기다린다. 그렇다고 async await가 promise를 완전히 대체 할 수 있는 것은 아니다. promise는 비동기 상태를 값으로 다룰 수 있기에 async await보다 큰 개념이다.


```javascript
async function runTasks() {
  try {
    const result1 = await asyncTask1();
    const result2 = await asyncTask2(result1);
    const result3 = await asyncTask3(result2);

    console.log("모든 작업 완료:", result3);
  } catch (error) {
    console.error("Error:", error);
  }
}

runTasks();

```


이렇듯 `callback` 의 경우 구현이 단순하지만 콜백 지옥이 발생하며, 가독성이 낮기에 `promise`의 `then()`체이닝 방식으로 콜백 지옥을 해결 할 수 있다.
`asyn-await`의 경우 코드 구조가 깔끔하고 `try catch`로 에러처리가 가능하여 유지보수가 쉽지만 `await`는 동기적으로 동작하기 때문에 병렬 실행에는
추가적인 작업이 필요하다는 단점이 있다. 