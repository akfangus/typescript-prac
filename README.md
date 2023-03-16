# 0. 타입스크립트?

- 안전하고 예측가능한 언어에 초점
- JS의 확장 ⇒ superset
- TS는 타입스크립트 컴파일러를 통해 JS로 변환이 됨

- JS는 변수선언시 const, let을 사용하고 변수의 타입을 알려주지않음. ⇒ 이러한 변수는 어떤타입의 변수도 들어갈 수 있음. ⇒ 이는 개발시에 다양한 에러를 초래할 수 있음.

- JS 데이터 타입

1. Primitive Type : 원시형
   1. `number`, `boolean`, `undefined`, `string`, `symbol`, `null` ,`void`
   2. `void` 는 Ts에서 지정한 타입 ⇒ void는 `undefined` or `null`만 가능
2. Object Type : 객체형
   1. `function`, `Array`, `classes`

<aside>
💡 TypeScript는 정적 타입을 지원한다.

</aside>

- 기본적인 TS에서 타입을 지정하는 방식은 Type Annotation, Parameter Annotation

```jsx
//type Annotation
let year: number = 2020;

//parameter Annotation
const sumNumbers = (num1: number, num2: numbber) => {
  return num1 + num2;
};
```

- 타입 추론 : 변수선언과 함께 값을 대입할 때 적용 ⇒ 변수에 초기값에 따라 그 변수의 정적 타입이 적용됨.
