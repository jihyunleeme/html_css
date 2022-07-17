# Grid
Flex 한방향 레이아웃 시스템 (1차원)  
Grid 두방향(가로-세로) 레이아웃 시스템 (2차원)
- display: grid;

### 그리드 형태 정의 
- grid-tempalte-rows
- grid-template-colums
  - fr(fraction) : 1fr 1fr 1fr = 1:1:1
- repeat 함수
- minmax 함수 : 최솟값, 최댓값
  - minmax(100px, auto) : 최소한 100px, 최대는 자동으로(auto)
  - repeat(3, minmax(100px, auto))
  - auto-fill, auto-fit

### 간격 만들기
 - row-gap : row의 간격
 - column-gap : column 간격
 - gap : row. column

### 그리드 형태 자동정의
통제를 벗어난 위치의 트랙크기 지정.  
컨텐츠의 갯수를 알수 없을 때 grid-auto-rows 쓰기
  - grid-auto-columns
  - grid-auto-rows

## 각 셀의 영역 지정
그리드 아이템에 적용하는 속성.
`grid-column-start`  
`grid-column-end`  
`grid-column`  
`grid-row-start`  
`grid-row-end`  
`grid-row` 
그리드 라인의 번호로 범위 지정.
```css
grid-column-start : 1;
grid-column-start : 3;
/*  위 코드는 아래와 같다. */
grid-column: 1 / 3;

/* 몇개의 셀을 차지할지 지정하기 */
grid-column : 1 / span 2;
```

## 세로방향 정렬
- align-items: stretch;
  - stretch : 그리드 영역 전체 너비 채우기, 수직방향으로 끝까지 늘어남. // 기본설정
  - start
  - center
  - end

## 가로방향 정렬
justify-items

## place-items
- `align-items`와 `justify-items`를 같이 쓰기
- 순서는 `align-items`, `justify-items`. 둘 중 하나만 쓰면 두 속성 모두 적용.

## 개별 아이템 세로 정렬
`align-self`
아이템을 세로(colum축) 방향으로 정렬.


참고: 
- Youtube "CSS Grid Crash Course 2022"  
  [https://youtu.be/0xMQfnTU6oo](https://youtu.be/0xMQfnTU6oo)  
- 1분코딩 이번에야말로 CSS Grid를 익혀보자  
  [https://www.youtube.com/watch?v=0xMQfnTU6oo](https://www.youtube.com/watch?v=0xMQfnTU6oo)