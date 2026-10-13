## tags 챕터 해결 방법

### Creating tags
1. git tag 태그이름 명령어를 사용하여 태그 만들기
2. git tag tagname

### Removing tags
1. git tag -d 태그이름 명령어를 사용하여 태그 삭제하기
2. git tag -d v1
3. git tag -d v2
4. git tag -d v3

### Tagging later
1. git log feature-list 명령어를 사용하여 Adding feature 2 커밋이름을 가진 커밋의 hash태그를 확인하기
2. git tag v1 확인한 hash태그 명령어를 입력하여 문제를 해결한다.

### Remote Tags
1. git pull 명령어를 사용하여 원격 저장소에 있는 내용을 가져온다.
2. git log 명령어를 사용하여 첫번째 commit의 hash 태그를 찾습니다.
3. git tag v2 hash태그를 입력하여 첫번째 커밋의 v2이름을 가진 태그를 만듭니다.

