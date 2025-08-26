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

# 📌 Git Branch 옵션 정리

`git branch` 명령어는 **브랜치 생성, 조회, 삭제, 이름 변경** 등에 사용됩니다.  
아래는 자주 쓰는 옵션 모음입니다.  

---

## 🔑 주요 옵션

| 옵션 | 설명 | 예시 |
|------|------|------|
| `-m` | 브랜치 이름 변경 | `git branch -m old_name new_name`<br>현재 브랜치를 바꿀 때 →<br> `git branch -m new_name` |
| `-M` | 강제 이름 변경 (같은 이름이 이미 있어도 덮어씀) | `git branch -M new_name` |
| `-d` | 브랜치 삭제 (병합된 경우만) | `git branch -d branch_name` |
| `-D` | 브랜치 강제 삭제 (병합 안 되어도 삭제됨) | `git branch -D branch_name` |
| `-a` | 모든 브랜치 보기 (로컬 + 원격) | `git branch -a` |
| `-r` | 원격 브랜치만 보기 | `git branch -r` |
| `--list` | 브랜치 목록 필터링 | `git branch --list "feature/*"` |
| `-v` | 브랜치별 마지막 커밋 메시지 표시 | `git branch -v` |
| `-vv` | 추적 중인 원격 브랜치 정보까지 표시 | `git branch -vv` |
| `--set-upstream-to=<remote>/<branch>` | 현재 브랜치를 특정 원격 브랜치와 연결 | `git branch --set-upstream-to=origin/main` |

---
