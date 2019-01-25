# github

### 설치주소

- <https://git-scm.com/>



### 저장소 만들기

```mkdir github``` 디렉토리 생성

```cd github``` 디렉토리 들어가기

```git init``` git의 저장소로 만들기



### git이 관리할 대상으로 파일 등록

```vim f1.txt``` 파일 생성

```git add f1.txt``` git이 파일 추적

```git status``` 현재 디렉토리 상태 확인

※ 변경할 때 마다 add를 해줘야 한다



### 버전 만들기

```git config --global user.name 닉네임``` 버전에 이름 등록

```git config --global user.email 이메일``` 버전에 이메일 등록

```git commit``` commit 메시지에 들어갈 수 있고 거기에 버전을 등록할 수 있다

※ commit 하기전 꼭 add를 해줘야 함

```git log``` log를 확인할 수 있다



### 변경 사항 확인

```git log -p``` 상세한 log를 확인할 수 있다

```git diff 버전ID1..버전ID2``` 버전간의 차이점을 비교

```git diff``` git add 하기 전과 후의 파일 내용 비교 ( 커밋하기 이전 )



### 과거 버전으로 돌리기

```git reset --hard 버전ID``` 적어준 버전 ID로 돌아감

```git revert 버전ID``` 커밋을 취소한 내용을 새로운 버전으로 만든다



### branch 생성

```git branch 브랜치이름``` branch 생성

```git branch``` branch list 확인

```git branch -d``` branch 삭제

```git branch -D``` branch 강제 삭제

```git checkout 바꿀 브랜치이름``` branch 전환

```git checkout -b 생성 후 바꿀 브랜치이름```  branch 생성 후 전환



### branch 정보 확인

```git log 브랜치1..브랜치2``` branch 비교

```git diff 브랜치1..브랜치2``` branch 코드 비교

```git log --branches --graph --decorate --oneline``` 

로그의 모든 브랜치 표시, 그래프 표현, 브랜치명 표시, 한줄로 표시



### branch 병합

```
git checkout A
git merge B
```

A branch로 B branch를 병합 (A ← B)