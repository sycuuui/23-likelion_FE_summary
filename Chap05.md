### Git & Github의 등장과 역할

- SCM (Sorce Code Management) : 저장소에 저장된 소스의 변경사항과 작업자를 추적
- git : 소스 이력 추적을 위한 버전 관리 시스템
- github : git 프로젝트를 관리하는 저장소 제공

---

### Git 설치 및 세팅하기 

- git config --global user.name "영문으로 이름 작성" : git 사용자 등록 
- git config --global user.email "email 작성"
- git config --list : 입력이 잘 되었는 지 확인함

---

### Git 동작 흐름과 구성 요소

- working directory : 현재 작업 중인 프로젝트가 있는 디렉포리
- staging area :  commit 할 파일의 예비 저장소
- local repository : 각 컴퓨터의 git이 관리하는 로컬 저장소 (언제든지 그 전으로 돌아갈 수 있음)
- ![image-20230121150744659](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20230121150744659.png)

---

### 로컬 Git 저장소 생성

1. git init - 나의 프로젝트가 위치한 곳으로 이동 후 터미널에서 명령 생성

2. .gitignore 파일 추가

   - 안에 제외할 파일 넣기
   - 제외할 파일은 commit을 해도 올라가지 않음

3. git status

4. git add. / git add "<파일명>" <- 충돌이 일어날 시 수정 후 이 단계부터 시작

   - git rm -- cached 파일명 : 삭제

   - 나의 프로젝트 중 버전관리에 반영할 파일 지정
   - 버전관리에 반영된 파일의 영역이 staging area

5. git commit -m "<message>" 

   - 로컬 저장소에 변동 기록을 남기기 위해 commit을 실행

6. git branch -M main

   - main / master
     - 즉시 운영 배포할 수 있는 버전
     - 사용자가 지금 이용 중인 코드
     - 모든 작업이 합쳐지는 곳이므로 main에서 작업하는 것은 위험함
   - staging - 상용에 반영하기 전 테스트 버전
   - feature - 새로운 기능 추가 개발(병렬 작업)

---

### Github에 소스 반영

1. git remote add origin <원격 저장소 주소>

2. git push -u origin <브랜치명>

---

### Github으로 협업하기

- clone - .git 포함 
- downlad ZIP - .git 제외
1. git clone https://github.com/[계정명]/[프로젝트명].git
2. git checkout -b <브랜치명> / git checkout <브랜치명> : branch 이동
3. git merge <브랜치명> : 합치기

---

### Git GUI 활용하기

