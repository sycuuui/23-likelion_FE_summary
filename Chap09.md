### Float

- : margin을 없애버리다
- 자식 요소의 width 값 자체가 바뀌는게 아니라, 부모 요소의 width 값 만큼 margin이 생기는 것
- 가로 배치 하고 싶은 요소에 전부 float를 선언
- 영상을 보면 이해가 잘 됨..

---

### Clear

- float로 없어진 margin 영역에 대응 clear
- float로 없어진 margin 영역을 무시하고 올라가지 않도록 처리해줌
- margin이 다시 생기는 것은 아님
- ![image-20230121202846789](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121202846789.png)
- Clearfix : clear라는 속성으로 Layout을 바로잡는 기법 
  - ![image-20230121203132080](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121203132080.png)
  - ![image-20230121203155497](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121203155497.png)

---

### Flex

- ![image-20230121203426149](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121203426149.png)

- justify-content: space-between; 
  - 부모요소에 선언하면 블록들의 사이 공간이 같은 비율로 띄어진다

---

### Position

- static : 모든 요소의 디폴트 값 생성되 원래 위치
- relative : 원래 위치를 기준으로 요소를 움직일 때 사용
- absolute : position이 static이 아닌 가장 가까운 부모를 기준으로 함
  - 부모요소가 없으면 body를 기준으로 위치를 움직임
  - absolute가 적용 되면 float등으로 발생하는 요소 간의 관계 무시
  - 대부분 부모가 relative일때 적용한다
- fixed : 브라우저 창을 기준으로 고정된 위치
- sticky : 스크롤로 특정 위치에 도달하면 고정

---

### Grid

- : 페이지 레이아웃의 가이드 라인
- ![image-20230121204553399](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121204553399.png)
- 외부의 라이브러리를 활용하여 완성도 있는 페이지를 만드는 것이 좋음



