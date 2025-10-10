# 브랜치 생성 및 이동

git checkout -b feature/login

# 코드 작업

...

# 커밋 및 원격 push

git add .
git commit -m "feat: 로그인 기능 구현"
git push origin feature/login

# (GitHub에서 PR 생성 → develop merge)

# 또는 직접 로컬에서 머지할 경우:

git checkout develop
git pull origin develop
git merge feature/login
git push origin develop

# 병합 후 브랜치 정리

git branch -d feature/login
git push origin --delete feature/login
