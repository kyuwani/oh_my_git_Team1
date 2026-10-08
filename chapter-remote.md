# Remote
## 1. Friend
```bash
git pull
echo Line 3, hi >> essay
git commit -am "More another line"
git push
git pull
echo Line 5, blobblob >> essay ; git commit -am "Real Final Is Mine."; git push
```

## 2. Problem
```bash
git commit -am "greeen"
git pull
# 이곳에서 conflict가 발생
# 파일 내용을 수정:
# The bike shed should be cyan
git commit -am "fix conflict"
git push
