### CSS 적용

- ![image-20230121183844940](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121183844940.png)

---

### CSS 구성

- Box-Sizing : 박스에 적용된 사이즈 구성하기
  - ![image-20230121184205762](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121184205762.png)

- *{box-sizing:border-box} 
- CSS 기본 구조
  - selector{ 속성 : 값 }
- CSS 선택자
  - 요소 전체에 적용 - universal
  - 특정 태그 전체에 적용
  - 특정 클래스에 해당되는 요소에 대해 적용
  - 특정 클래스가 명시된 특정 태그에 대해 적용
  - 특정 아이디에 해당되는 요소에 대해 적용
  - 특정 아이디가 명시된 특정 태그에 대해 적용
  - 부모 요소 내의 특정 자식 요소 (ex ) div p{})
- CSS 주석
  - /* */

---

### CSS 특성

- Cascading
  - 같은 태그에 대한 규칙이 있는 경우 => 마지막으로 작성된 규칙 적용
- Inheritance
  - 부모요소의 CSS 규칙을 자식 요소가 상속하여 적용
  - 자식 요소가 CSS규칙을 가지고 있다면 이를 우선하여 적용
- Specificity
  1. HTML 요소의 style 속성
  2. id 요소
  3. class 요소
  4. 태그의 이름

---

### Box Model

- CSS Box

  - inline
    - ![image-20230121185559927](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121185559927.png)

  - block
    - ![image-20230121185635970](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121185635970.png)

  - inline-block
    - ![image-20230121185909841](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121185909841.png)
- Box-Model

  - Margin 
    - margin: 전체;
    - margin: 상하 좌우;
    - margin: 상 우 좌 하;
  - Border

    - border: 두께 형태 색깔;
  - Padding
    - padding: 전체;
    - padding: 상하 좌우;
    - padding: 상 우 좌 하; 

---

### Box-Sizing

- 박스에 적용된 사이즈 기준 정하기

---

### CSS 단위

- px : 스크린을 구성하는 작은 점
- % : 부모 요소를 기준으로 크기의 설정
- em : 부모 요소의 폰트 크기 / rem : 루트 요소의 폰트 크기
  - 통일된 기준을 잡기 위해서는 rem 단위 사용 권장
- vw  / vh : 각 디바이스별 화면의 너비/ 높이를 기준으로 배율 설정 

---

### 이미지 다루기

- <img src="이미지 경로" alt="대체 문구">
- 이미지 단독으로 사용하는 것보다 div로 마크업 후 사용 권장
- max-width:100%; : 부모 영역에서 벗어나지 않도록 이미지의 너비 상한선을 100%로 설정
- object-fit : cover; : 이미지를 부모 요소의 가운데 즉, 영역의 크기 만큼 확대/축소하여 채움 
  - 원본 비율 유지
- object-fit: contain; :이미지의 비율을 유지하면서 크기를 변형하여 부모 요소를 채움
  - 넓이와 높이 중 가장 먼저 부모 요소의 크기에 도달하는 지점에서 멈춘다
- object-fit: fill; 이미지의 비율을 유지하지 않고 부모 요소의 크기에 맞게 변경하여 채움

---

### Overflow

- overflow : hidden ; :부모 요소 크기에 벗어난 부분을 가려버림
- overflow : scroll; 
  - overflow-x :scroll; 
  -  overflow-y :scroll; 
- overflow: auto; :자동으로 넘치는 부분에 스크롤 생성

---

### 폰트 꾸미기

- Hex color : 16진수로 나타내어 색상 설정
- font-style: italic;
- font-weight:bold
  - ![image-20230121192742956](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121192742956.png)

- text-decoration : underline;
- text-decoration : none;
- 순서 지키기![image-20230121192914602](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121192914602.png)

---

### 테두리 꾸미기

- 테두리 둥글게 만드는게 요즘 트렌드...

---

### 배경 이미지 설정

- background-image: url(); :크기에 맞게 이미지가 반복해서 보임
- background-repeat: no-repeat; :반복하지 않음
- background-size: contain; : 이미지가 온전히 표시되는 것이 우선
- background-size: cover; :요소의 배경을 모두 덮는 것이 우선 -> 넘치면 그냥 짤라버림..
- background-position: center; : 이미지를 가운데로
- 이미지를 레이아웃에 맞는 해상도로 크롭해서 사용하는게 젤 베스트트트트ㅡ틑

---

### 요소 정렬하기

- margin : 0(상하) auto(좌우); :가운데로 요소의 위피를 맞춤
  - 부모 block 요소의 width를 기준으로 자동으로 margin 계산
  - 부모가 width를 가지고 있지 않으면 사용할 수 없음
- text-align: center; : 블록 요소 내의 인라인 요소를 가운데 정렬