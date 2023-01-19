---
layout: post
title: Vue.js - 할 일 관리 앱 
date: 2023-1-16 18:00:59
modified: 2023-1-16 18:00:59
tag: [Vue, JavaScript]
---

## `Vue.js`
`Vue.js`는 `React`와 가장 유사하지만 `React`보다는 좀 더 많은 사람들이 접근하기 쉽도록 제작된 자바스크립트 프레임워크이다. `Vue.js`의 창시자인 에반은 `Angular`의 필수적인 요소들만 가지고 화면을 구현하기 시작했고, 이를 오픈 소스화하고 많은 사람들이 참여하여 기능을 점차 붙여나가면서 `Angular`의 양방향 데이터 바인딩과 `React`의 단방향 데이터 흐름의 장점을 모두 결합한 프레임 워크로 탄생 하였다.

이러한 `Vue.js`를 학습하기 위해 아래와 같이 할 일 관리앱을 구현해 보았다. 실무에서 서비스를 만들 때 사용하는 데이터 조작 방법(삽입,조회,변경,삭제)을 할 일 관리앱을 통해 간단히 코드로 구현해보면서 특징들을 아래와 같이 간략히 정리하였다.


## 실행결과

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/99943583/212711300-993fdc81-0bf7-4352-a19f-0c70218724f2.gif)

## `Vue.js`의 특징

1. 상 - 하위 컴포넌트 관계
각 컴포넌트 별로 고유한 유효 범위(`Scope`)를 가지고 있기에 직접 다른 컴포넌트의 데이터를 참조할 수 없다. 가장 기본적인 데이터 전달 방법은 상위 - 하위 컴포넌트 간의 데이터 전달 방법이다.`props`를 통해 상위에서 하위로 속성을 전달할 수 있고(`React`와 유사)  하위에서 상위로는 기본적으로 이벤트만 전달할 수 있다.

아래 코드 예시를 살펴보자.

```javascript
<template>
<section>
  <ul>
    <li v-for="(todoItem, index) in propsdata" :key="todoItem" class="shadow">
     <i class="checkBtn fas fa-check" aria-hidden="true"></i> 
       {{ todoItem }}
      <span class="removeBtn" type="button" @click="removeTodo(todoItem, index)">
        <i class="far fa-trash-alt" aria-hidden="true"></i>
      </span>      
    </li>
  </ul>
</section>
</template>

<script>

    export default {
      props: ['propsdata'],
      methods: {
          removeTodo(todoItem, index) {
          this.$emit('removeTodo', todoItem, index);
  }
   }
    }

</script>

```
위와 같이 하위컴포넌트에서 `props` 속성 을 정의한다.

```javascript
 `props` : ['`props` 속성이름']
```

상위 컴포넌트에서는 아래와 같이 `v-bind`속성을 통해 `props`속성을 넣어준다.
```javascript
  <TodoList v-bind:propsdata="todoItems" @removeTodo="removeTodo"></TodoList>
```
```javascript
//기본예제
<child-component v-bind:props 속성 이름="상위 컴포넌트의 data 속성"></child-component>
```

 위와 같이 `v-bind` 왼쪽 값으로 하위 컴포넌트에서 정의한 `props`속성 이름을 넣고 오른쪽 값으로 상위 컴포넌트의 `data` 속성을 지정해주면 상위 컴포넌트의 특정 속성을 하위 컴포넌트로 전달할 수 있다.


