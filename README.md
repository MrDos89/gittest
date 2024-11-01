# GIT과 GITHUB
## GIT
### Local git
- GIT : 분산 버전 관리 시스템

- 저장소 생성
```bash
git init
```

- git 설정
```bash                                                 
git config user.name "DoHyung Kim"  
git config user.email mrdos89@gmail.com
#공용 git 설정을 하려면 -g
# 예) git config -g user.name 이름
```

- git 상태 확인
```bash
git status
```

- staging
```bash
git add .
```

- 저장소에 반영 (commit)
```bash
git commit -m "first commit"
```

- 상태 확인과 로그 확인
```bash
git status # 상태 확인
git log # 로그 확인
```

## Local Git to GitHub
- GitHub에서 저장소를 생성
- 저장소 주소
    - https://github.com/MrDos89/gittest.git
```bash
git remote add origin https://github.com/MrDos89/gittest.git
```

```bash
git push -u origin master #첫번째 푸시
git push #기본 원격지 현재 브랜치로 푸시
```


### From Github to Local Git
- 복제할 원격 저장소 주소 확보
- 복제
```bash
git clone https://github.com/MrDos89/gittest.git
# git clone 원격지 주소
# 원래 프로젝트를 만들었던 저장소가 아니라면(clone으로 받아온 프로젝트) 현재 저장소 설정을 바꿔야한다.
# git config user.name "DoHyung Kim"
# git config user.email mrdos89@gmail.com
```