팀개발을 위한 Git, GitHub 시작하기

#1. Git Bash 명령어
-git init
[.git]폴더 생성(Git으로 생성한 버전들의 정보와 원격 저장소 주소 = 로컬저장소)

-git config --global user.email "hello.git.GitHub@gamail.com"
-git config --global user.name "Cat-Hanbit"
버전관리를 위한 내 정보 등록

-git add README.txt
커밋

-git commit -m "설명추가"
커밋의 상세설명 추가

-git log
지금까지 만든 커밋의 로그 확인

-git checkout ~~
로그에서 확인한 커밋으로 돌아가기

-git remote add origin 깃허브주소
로컬 저장소에 연결한 원격 저장소 주소 저장

-git brach -M main
커밋을 저장할 브런치 생성

-git push origin main
메인브런치에 커밋 올리기

-git clone 깃허브주소 .
원격저장소의 파일을 로컬파일로 내려받기
* ' .'을 붙이지 않을시 로컬폴더 안에 새로운 레포지토리 이름으로 새로운 폴더가 생김

-git pull origin main
원격저장소에 있는 새로운커밋으로 업데이트 하기