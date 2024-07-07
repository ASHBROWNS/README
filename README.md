# #ASH github 사용법
#ASH팀의 github 사용법입니다. 꼭 제대로 숙지해주세요!

## 🍴fork를 하는 경우

### fork란?
- 다른 사람의 레파지토리를 복제하여 자신의 레파지토리로 만드는 것이다.

### fork 하는 법
1. 복제할 레파지토리 우측 상단의 'fork'버튼을 누른다.
<img width="301" alt="image" src="https://github.com/ASHBROWNS/README/assets/128370710/f6d83fab-6226-4e69-86a5-298714a58add">


2. owner을 자신의 계정으로 설정하고, 레파지토리 이름과 설명을 적고 생성을 하면 자신의 계정에 복제된 레파지토리가 생성된다.
<img width="710" alt="image" src="https://github.com/ASHBROWNS/README/assets/128370710/a0077b7e-bfbc-4adc-aa5d-98163007b17f">


### organization 활용법

<추후 추가 예정입니다>

#### clone 이란?
원격의 Git 저장소를 로컬에 복제해오는 명령어이다.

<br/>

## clone 방법
<추후 추가 예정입니다>


## commit 하는 법
*주소를 연결한 경우 이 루트만 타면 됩니당 !
`git add .` -> `git commit -m "커밋메세지"` -> `git origin push <branch명>`

### commit 이란?
- Git에서 commit은 변경 사항을 저장소에 기록하여 특정 시점의 스냅샷을 만드는 작업. <br />
  -> 코드가 날아가지 않게 중간저장을 해주는 역할. 저장한 위치로 되돌릴 수 있음.

### 1. `git init`
- git init은 현재 디렉토리를 새로운 Git 저장소로 초기화하여 .git 디렉토리를 생성한다.
- 처음 레포를 연결 할 때 한 번만 해주면 된다.

### 2. `git add .`
- repository에 무엇을 올릴지 정하는 단계.
- 다시 말해 무엇을 commit할 지 정하는 단계.

### 3. `git commit -m "커밋메세지"`
- 커밋을 생성하는 명령어.
- 커밋메세지에는 무엇을 추가했는지, 삭제했는지 등 코드의 변동사항을 적어준다. (하단의 커밋규칙 참고)

### 4. `git branch <branch명>` 란?
- 브랜치를 생성하는 명령어이다.
  #### branch로 이동하는 방법
  `git switch <branch_name>`
  #### branch 생성과 동시에 이동하는 방법
  `git switch -c <branch_name>`
  #### branch를 삭제하는 방법
  `git branch -d <branch_name>`
<br/>

### 5. `git origin push <branch명>` 란?
- 로컬 브랜치의 변경 사항을 원격 저장소의 해당 브랜치로 전송하는 명령어이다.
- 즉 push를 해야 github에 올라가고, 다른 사람이 온라인에서 해당 코드를 볼 수 있다.

### `git pull` 이란?<br />
- 원격 저장소에서 최신 변경 사항을 가져와 로컬 저장소에 병합하는 명령어이다.

<br />

# 5. 커밋 메세지 룰
commit messagre를 어떻게 적을지에 관한 약속이다. 커밋 룰은 팀마다 다를 수 있기 때문에, 전적으로 따르지 않아도 된다. 중요한 것은 변경 사항에 대한 설명이 명확하도록 하는 것이다. 그래야 **history rollback**이 용이할 것이다. 이는 협업할 때 중요하게 작용할 것이다.

| type | description |
| --- | --- |
| ADD | 새로운 기능 추가 |
| FIX | 버그 수정 |
| CHORE | 허드렛일(사소한 일) |
| STYLE | 코드 스타일 관련 변경(코드 포매팅, 세미콜론 누락 등) |
| REFACTOR | 코드 리팩토링 |
| TEST | 테스트 코드, 리팩토링 테스트 코드 추가 |

ex)

```
git commit -m "ADD :: header 구현"
git commit -m "style :: 주석 삭제"
```

<br/>

