# talent sharing git session by Ben !!

## 순서
#### 1. 원격 레포지토리 연결 
-  git config --global user.email "you@example.com  
   - 이메일 설정
-  git config --global user.name "Your Name"
   - 이름 설정 
- 로컬에서 원격저장소로 push 할 파일들이 있는 위치로 이동하기 ( 프로젝트 최상위 폴더 )
- 원격 레포지토리 주소 복사
- git clone "원격 레포지토리 주소"
- git remote add origin "원격레포지토리 주소"
  
#### 2. 브랜치 생성
- git branch "브랜치 명"
  - 브랜치 생성 
- git branch -a 
  - 브랜치명 조회
- git branch -d "브랜치 명"
  -  브랜치 삭제 
- git checkout "브랜치 명" 
  - 브랜치 이동 

#### 3. 커밋하기
- git status 
  - 현재 로컬 저장소 상태확인
- git add 파일명 or git add . (전체)
  - 파일 staged 상태 (커밋을 준비하기 위한 상태)
- git commit -m "메세지"
  - 변경 사항을 버전 기록에 새 커밋으로 저장하는 데 사용됩니다. 각 커밋은 특정 시점의 프로젝트 스냅샷을 나타냅니다.

#### 4. 원격 저장소에 올리기
- git push origin "브랜치명"
  - 여기서 origin 은 원격 저장소의 이름 ( origin은 기본이름, 설정 가능 ) 
- git pull origin "브랜치명"
  - 반대로 원격 저장소의 버전을 받아올 때 사용하는 명령어 

#### 5. 협업에서 버전 맞추기

- git pull origin dev
  - 먼저 dev (약속 된 개발 버전) 파일 위치에서 git pull origin dev
- git merge dev
  - 내가 작업 중인 브랜치로 이동해서 git merge dev 
  - 이 때 다른 사람이 작업한 내용이 내 브랜치에 적용되면서 버전 일치 