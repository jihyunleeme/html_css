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

### 간격 만들기
 - row-gap : row의 간격
 - column-gap : column 간격
 - gap : row. column

### 그리드 형태 자동정의
통제를 벗어난 위치의 트랙크기 지정.  
컨텐츠의 갯수를 알수 없을 때 grid-auto-rows 쓰기
  - grid-auto-columns
  - grid-auto-rows


참고: 
- Youtube "CSS Grid Crash Course 2022"  
  [https://youtu.be/0xMQfnTU6oo](https://youtu.be/0xMQfnTU6oo)  
- 1분코딩 이번에야말로 CSS Grid를 익혀보자  
  [https://www.youtube.com/watch?v=0xMQfnTU6oo](https://www.youtube.com/watch?v=0xMQfnTU6oo)