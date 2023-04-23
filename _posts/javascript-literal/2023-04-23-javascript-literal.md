---
layout: post
title: 자바스크립트 표현식과 문
date: 2023-04-23 12:00:59
modified: 2023-04-23 12:00:59
tag: [javascript]
---

## 표현식과 문

자바스크립트에서 표현식인 문과 표현식이 아닌 문의 차이는 무엇인지 알아보자.

```javascript
let study = let x; // Uncaught SyntaxError: Invalid or unexpected token
```

표현식이 아닌 문의 경우 값처럼 사용할 수 없다. 위처럼 구문 오류가 난다.

```javascript
let study = 100;

study = x;
```

표현식인 문은 값처럼 사용할 수 있다.

아래 예시를 살펴보면, 크롬 개바자 도구에서 표현식이 아닌 문을 실행하면 완료값 `undefined`를 출력한다. 아래와 같이 변수에 할당 할수도, 참조할 수도 없다.

```javascript
let foo = 10;
>> undefined
```

따라서, 표현식인 문은 값으로 평가될 수 있는 문이며, 표현식이 아닌 문은 값으로 평가될 수 없는 문을 말한다.

## References

모던자바스크립트DeepDive
