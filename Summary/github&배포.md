# LikeLion 8th Coding Session

## Github 기초

 + Github
    + 파일의 변경된 내용을 기록<br/>
        + 무엇이 변경되었는지<br/>
        + 어디서 변경돠었는지<br/>
        + 누가, 언제 변경되었는지 <br/>

 + git, Git Bash 설치 <br/>
 + Github 계정 생성, 레포지토리 생성<br/>
 + 명령어<br/>
 
git 저장소를 초기화
```
git init
```
원격 저장소(remote repository) 연결
```
(git remote add origin 레포지토리 주소)
git remote add origin https://github.com/whitepurple/Likelion_unilion_summary
```
폴더에 변경된 모든 파일 staging area에 올리기
```
git add .
```
유사시 돌아갈 수 있는 저장소의 체크 포인트 생성
```
git commit -m "(원하는 내용)"
```
원격 저장소의 master 브랜치에 프로젝트 저장
```
git push origin master
```
   
## Netlify 배포

+ 정적 페이지<br/>
  + 시간이나 사용자의 요청에도 변하지 않는 페이지<br/>
+ 동적 페이지<br/>
  + 시간이나 사용자의 요청에 변하는 페이지<br/>
  
+ 코드 Github에 업로드, Netlify통해서 Github 연동 호스팅<br/>
  1. 코드를 올렸던 레포 이름 기억<br/>
  2. [Netlify](https://www.netlify.com/) Github계정으로 회원가입, 로그인<br/>
  3. New site from Git 클릭하여 진행<br/>
  4. Github 선택<br/>
  5. 배포할 레포지토리 이름 선택<br/>
  6. Deploy site 클릭<br/>
  7. Published 뜨면 배포됨 - url 클릭하여 바로 배포 가능<br/>

## Github 협업
**내 컴퓨터/로컬 환경** <br/>
-> git add -> **Staging area** <br/>
-> git commit -> **Local repository**<br/>
-> git remote add origin 레포지토리 주소 -> **Remote repository**<br/>

+ 자주 사용하는 명령어<br/>

새로운 브랜치를 생성
```
git branch 브랜치명
```

해당 브랜치로 이동
```
git checkout 브랜치명
```

원격 저장소의 특정 브랜치에 프로젝트 저장
```
git push origin 브랜치
```

원격 저장소의 특정 브랜치에서 변경사항 pull 해오기
```
git pull origin 브랜치
```

원격 저장소에 있는 파일 전체 복사
```
git clone http://원격저장소 주소.git
```

git 저장소의 상태를 확인
```
git status
```

+ 협업 진행 방법<br/>

  1. 원격 저장소 생성<br/>
  2. 팀원을 Collaborator로 추가<br/>
  3. 초기 프로젝트 push<br/>
  4. 팀원들의 로컬에 프로젝트 pull<br/>
  5. 팀원 각자의 브랜치를 생성하여 작업<br/>
  6. 브랜치에 작업한 내용을 pull<br/>
  7. master와 merge 하기전 pull request<br/>
      - master와 합치기 전 수정 사항을 팀원과 공유
      - base 브랜치에 compare브랜치를 merge 요구
      - create pull request눌러서 생성
  8. Pull request 확인 후 Master 와 merge<br/>

+ Fork를 이용한 협업<br/>

  1. 작업 하고 싶은 Repository fork 해오기<br/>
      - 우상단의 Fork버튼 누르기
  2. 자신의 로컬에서 작업<br/>
  3. 변경사항을 자신의 브랜치에 push<br/>
  4. 원본 레포지토리 소유자에게 Pull request 요청<br/>
  5. 소유자가 pull request를 승인하여 merge하면 자동으로 collaborator 추가<br/>
