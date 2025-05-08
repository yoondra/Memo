# GIT Commands

:small_blue_diamond: :point_right: :red_circle::black_circle: :white_circle: :white_square_button: :black_square_button: :white_check_mark: :copyright: :clock6: :ok:

## :white_check_mark: git flow
- master: 최종 릴리즈에 사용 되는 안정된 버전
- develop: 다음 릴리즈를 위해 개발중인 최신 버전
- feature: 특정 기능 개발을 위한  branch
- release: 릴리즈 점검을 위한 branch
- hotfix: 긴급 버그 픽스를 위한 branch
- support: 버전 호환성 문제를 처리하기 위한 branch
  
``` $git flow init ```

### Features
- 특정한 기능을 개발하기 위한  
  
``` git flow feature start <branch name> ```

## :white_check_mark: 원격 저장소 위치 확인
``` git remote -v ```
### 특정 브랜치만 clone 하기
```
git clone -b <branchname> 
git clone -b <branchname> <remote-repo-url> 
git clone -b <branchname> --single-branch <remote-repo-url> 
```
### 특정 tag만 clone 하기
```
git clone -b <tagname> 
git clone -b <tagname> <remote-repo-url> 
git clone -b <tagname> --single-branch <remote-repo-url> 
```

## :white_check_mark: branch
#### 새로운 branch 생성
``` git branch <branchname> ```
#### 새로운 branch 만들고 checkout
``` git checkout -b <branchname> ```
#### 현재 사용 중인 branch 나열
``` git branch ```
#### 원격 저장소의 branch checkout
```
git branch -r 명령으로 원격 브랜치 확인 후 
git checkout -t <remote branch name>           
git checkout -t origin/<branchname>
```    
#### 현재 branch를 원격 저장소의 branch로 변경

``` git branch --set-upstream-to=origin/<branch> <현재branch> ```
