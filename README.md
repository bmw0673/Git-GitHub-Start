# Git 명령어 모음

# 📌 Git 자주 사용하는 명령어

터미널에서 자주 사용하는 명령어입니다.

---

## 🔑 주요 명령어

| 명령어 | 설명 | 예시 |
|------|------|------|
| `git init` | [.git]폴더 생성 | `` |
| `git config --global user.email "{user_email}"` | 유저 이메일 등록 | `git branch -M new_name` |
| `git config --global user.name "{user_name}"` | 유저 이름 등록 | `git branch -d branch_name` |
| `git add {파일명}` | 파일 스테이징 | `git add README.txt<br>파일명 대신 . 을 붙이면 전체 파일 스테이징` |
| `git commit -m "{커밋메세지}"` | 스테이징된 파일 커밋 | `git commit -m "설명추가"` |
| `git log` | 지금까지 만든 커밋 로그 확인 | `git log` |
| `git checkout {커밋ID}` | 특정 커밋시점으로 돌아가기 | `` |
| `git remote add origin {깃주소}` | 로컬저장소에 연결할 원격저장소 주소 저장 | `` |
| `git push origin {브랜치명}` | 원격저장소에 커밋 올리기 | `` |
| `git clone {깃주소} .` | 원격저장소의 파일 내려받기 | `' .'을 붙이지 않을시 로컬폴더 안에 새로운 레포지토리 이름으로 폴더 생성` |
| `git pull origin {브랜치명}` | 원격저장소에 있는 새로운커밋으로 업데이트 하기 | `` |
| `git fetch` | 원격저장소의 변경사항 확인하기 | `` |

---

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
