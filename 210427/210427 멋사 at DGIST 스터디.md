# 210427 멋사 at DGIST 스터디



## 1. 개발 환경 설정

### git bash

다운로드 링크 : https://git-scm.com/downloads

설치 참고 사이트 : https://gabii.tistory.com/entry/Git-Git-Bash-219-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0

명령어 참고 사이트 : https://gbsb.tistory.com/10



## 요약

원격 저장소 로컬에 끌고 오기 : `git clone 주소`

로컬저장소 현재 상태 확인 : `git status`

파일 준비 영역으로 옮기기 : `git add`

준비 영역에서 원격으로 옮기기 : `git commit -m "커밋메시지"`

원격 준비 영역에서 원격 서버로 푸쉬 : `git push`



## git config (최초 1회 실행)

```
// git commit에 사용될 username
git config --global user.name "your_name"
 
// git commit에 사용될 email
git config --global user.email "your_email@example.com"
 
// 설정한 내용을 확인할 수 있다.
git config --list
```



## git init

현재 디렉토리를 로컬저장소로 설정

```
// 로컬저장소로 설정할 프로젝트 위치로 이동한다.
cd C:/dev/workspace/eom2017
 
// 로컬저장소로 설정한다.
// (master) 브랜치로 보이면 성공한 것이다.
git init
 
// 만약 init을 취소하려면 아래의 명령어를 입력한다.
rm -r .git
```



## git status

로컬 저장소의 현재 상태 알아보기



## git add

파일을 준비영역(Staging Area)으로 옮긴다. **(GitHub와 연동하려면 git remote로 원격 저장소와 연결해야 함)**

```
// a.html 파일만 추가
git add a.html
 
// 워킹 디렉터리 내 모든 파일을 추가
git add .
 
// 명령 프롬프트에서 상호작용하면서 추가 (나갈땐 q를 입력)
git add -i
 
// 진행중인 파일일 경우, Staging Area에서 워킹 디렉터리로 옮겨온다. 
$git rm --cached a.html
$git rm -r --cached .
```



## git commit

```
// 에디터가 출력되고, 에디터에서 커밋 메시지 입력 후 저장하면 커밋됨
git commit
 
// 간단한 커밋 메시지를 입력후 커밋
git commit -m "커밋 메시지"
 
// Staging Area에 들어간 파일에 대해서만 (워킹 디렉터리는 적용 X)
git commit -a -m "커밋 메시지"
```



## git push

```
// 원격저장소에 저장한다.
git push -u origin master
 
// 에러 - ! [rejected] master -> master (fetch first)
// 이미 변경된 파일이 원격저장소에 있을경우 발생
git pull origin master 
 
// 에러 - ! [rejected] master -> master (non-fast-forward)
git push origin +master

```





### Visual Studio Code

```
비주얼 스튜디오 코드(영어: Visual Studio Code)는 마이크로소프트가 마이크로소프트 윈도우, macOS, 리눅스용으로 개발한 소스 코드 편집기이다. 디버깅 지원과 Git 제어, 구문 강조 기능등이 포함되어 있으며, 사용자가 편집기의 테마와 단축키, 설정 등을 수정할 수 있다.
```



#### 설치

https://code.visualstudio.com/download



#### 기타 플러그인

https://redcow77.tistory.com/409





### Typora

마크다운 텍스트 에디터

https://typora.io/

```
마크다운(markdown)은 일반 텍스트 기반의 경량 마크업 언어다. 일반 텍스트로 서식이 있는 문서를 작성하는 데 사용되며, 일반 마크업 언어에 비해 문법이 쉽고 간단한 것이 특징이다. HTML과 리치 텍스트(RTF) 등 서식 문서로 쉽게 변환되기 때문에 응용 소프트웨어와 함께 배포되는 README 파일이나 온라인 게시물 등에 많이 사용된다.
```





## 2. github deployment

1. https://github.com/
2. github 계정 생성
3. Create new repository
4. Repo name : 이름.github.io 로 설정



## 3. 지난 강의 진도 확인

