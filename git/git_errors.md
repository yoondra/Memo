## :white_check_mark: detached head

### 수정 내용 버릴 경우  
``` git checkout branch ```

### 수정 내용 보존 필요한 경우  
``` git checkout -b newbranch ```

## :white_check_mark: untracked files 삭제 하기
```
$ git clean -f          // file 만 삭제 
$ git clean -fd         // directory 도 삭제 
```

## :white_check_mark: merge error 발생 시
```
git reset --hard <branchname>
git reset --hard d678197
```
