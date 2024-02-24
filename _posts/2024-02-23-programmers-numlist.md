---
layout: post
title: "[Algorithm]프로그래머스 알고리즘 문제풀이"
date: 2024-02-23 12:10:59
modified: 2024-02-23 12:10:59
tag: [JavaScript, Algorithm]
---

정수 리스트 num_list가 주어질 때, 마지막 원소가 그전 원소보다 크면 마지막 원소에서 그전 원소를 뺀 값을 마지막 원소가 그전 원소보다 크지 않다면 마지막 원소를 두 배한 값을 추가하여 return하도록 solution 함수를 완성해주세요.

제한사항

- 2 ≤ num_list의 길이 ≤ 10
- 1 ≤ num_list의 원소 ≤ 9

```javascript
function solution(num_list) {
  const [a, b] = [...num_list].reverse();
  return [...num_list, a > b ? a - b : a * 2];
}
```

### 1. `reverse()`

자바스크립트 배열의 메서드 중 하나로, 배열의 순서를 역순으로 뒤집는다.

```javascript
const originalArray = [1, 2, 3, 4, 5];
const reversedArray = originalArray.reverse();

console.log(reversedArray); //  [5, 4, 3, 2, 1]
```

### 2. 전개연산자(`Spread Operator`)

전개연산자는 배열이나 객체를 펼쳐서 새로운 배열 혹은 객체를 생성하는 문법으로, 주로 배열 혹은 객체를 복사하거나 다른 배열이나 객체와 결합할때 사용한다. 주어진 `num_list`를 복사하여 `reverse`로 역순으로 정렬한 후 새로운 배열을 만들었다.

### 3. 비구조화할당(`Destructuring Assignment`)

비주조화할당은 배열이나 객체에서 값을 추출하여 할당하는 방법이다. 배열이나 객체의 요소를 간편하게 분리하고 사용할 수 있다

```javascript
const numbers = [1, 2, 3, 4, 5];

const [a, b, ...rest] = numbers;

console.log(a); // 1
console.log(b); // 2
console.log(rest); // [3, 4, 5]
```

위 풀이에서 역순으로 정렬된 배열의 첫 번째와 두 번째 요소에 변수 `a`와 `b`를 할당하였다. 따라서 첫 번째 요소가 두번째 요소보다 클때 그 차이값을 전개연산자를 이용하여 마지막 요소값으로 추가하고, 그렇지 않을 경우에 마지막 요소의 값의 2배를 해당 배열의 마지막 값으로 추가하는 방식으로 풀이하였다.
