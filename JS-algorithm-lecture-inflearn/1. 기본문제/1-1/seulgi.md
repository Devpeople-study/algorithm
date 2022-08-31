# 세 수 중 최솟값
> 100이하의 자연수 A, B, C를 입력받아 세 수 중 가장 작은 값을 출력하는 프로그램을 작성하세요.(정렬을 사용하면 안됩니다)

```javascript
const solution1 = ( a, b, c ) => {
  const answer = Math.min(a, b, c)

  return answer;
}

console.log(solution(2, 5, 1));
```

```javascript
const solution2 = ( a, b, c ) => {
  let answer
  a < b ? (answer = a) : (answer = b);
  c < answer && (answer = c);

  return answer;
}

console.log(solution(2, 5, 1));
```