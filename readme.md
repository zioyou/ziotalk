## ZioTalk electron 배포 버전관리

### electron 폴더는 예전 폴더

### electron2 폴더는 최신 폴더

### 에러 발생시 대처
```
아래와 같은 에러가 발생한다면
remote: Verify
fatal: Authentication failed for 'http://211.234.105.50:3000/ZCP.omega.ZioTalk/CICD.Client.git/'

아래처럼 입력 후 진행
git credential reject http://211.234.105.50:3000

만약 배포에 문제가 있을때 원복 방법

# git checkout -b <임시 브랜치 내용> <돌아갈 커밋>
git checkout -b test 51786cbd21

# 추후 수정 후 다시 배포하고 난 후
git checkout main
git pull origin main

```