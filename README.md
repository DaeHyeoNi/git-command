# branch 명령어
### 로컬 저장소 branch 목록 보기
git branch
### 원격 저장소 목록 보기
git branch -r
 
### branch 목록보기
git branch -a
 
### branch 생성
git branch {이름}
 
### 다른 branch 로 이동
git checkout {이름}
 
### branch 이름 변경
git branch -m {old_name} {new_name}
 
### branch 삭제
git branch -d {name}
 
### 원격 저장소의 Branch 삭제하기
git push --delete {원격 저장소 별칭} {원격 Branch 이름}
 
### PUSH 하기
git pull origin {branch_name}
 
 
 
# commit 만들기
### 현재 git 상태
git status
### 파일을 목록에 추가
git add {파일}
### 폴더 내 파일 전부 목록에 추가
git add .
 
### 스태이지에 넣을 라인 정하기 (파일 내 일부 코드만 commit 할려고 할시)
git add -p
 
### 스테이징된 커밋 보려면
git commit -v
 
### 커밋 만들기
git commit -m "message"
git commit -am "스태이징과 커밋을 한번에!"
 
### 이전 commit에 변경내역 추가
git commit --amend
 
# git remote(원격저장소) 에서 삭제된 branch 업데이트
원격 저장소에서는 이미 삭제된 branch 인데 (merge 되어서 필요없어서 삭제된경우)
 
내 로컬 저장소에는 그대로 있을때 정리하는 방법
 
git remote prune origin
 
 
# 임시저장 (stash)
git stash
 
git stash list

git stash pop

# Merge
### Merge 하기
git merge {브랜치명}
 
### 공백 무시하고 Merge (스페이스를 탭으로 바꾼다거나)
git merge -Xignore-space-change {브랜치명}
 
# 로그보기
git log

git show
