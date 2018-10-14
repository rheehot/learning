 > git branch 삭제
 ```
 $ git branch -d 브런치이름
 ```
 > git push할 원격저장소 변경
 ``` $ git remote -v
     $ git remote set-url origin 변경할 주소
 ```
 > Git - fatal: Unable to create '/path/my_project/.git/index.lock': File exists 오류 발생 해결법.
 
 ``` $rm -f ./.git/index.lock```
 
 > push할 때 로컬과 원격 저장소를 연결한다.
 
 ``` $ git remote add origin 원격저장소 주소```
 
 > git 저장소 상태 확인
 
 ``` $ git status ```
 
 
 
 
 - 처음 repogitory를 만들면 master브랜치가 있다.
 
 ``` checkout```명령어를 실행해서 다른 별도의 브랜치를 두고 작업할 수 있다.

![틸드, 캐럿](https://backlog.com/git-tutorial/kr/img/post/stepup/capture_stepup1_3_2.png)
Branch는 master에 있는 소스코드에 새로운 기능을 추가하거나, 버그를 수정하는 등의 소스 내용의 변경을 줄 때 master의 소스 코드는 그래로 두고 별도의 루트에
소스코드의 내용을 바꾸는 것.

나중에 branch를 master와 merge해서 소스코드를 버전 업 시킨다.

## Branch 종류
 1. 통합 브랜치(International Branch)
 - 서비스 실행가능한, 배포가능한 버전
 
 
  2. 토픽 브랜치(Topic Branch)
   - 통합 브랜치로부터 만든다.
   - 버그 수정, 기능 추가같은 단위 작업을 위한 브랜치
   - 토픽브랜치 작업 끝나면 통합 브랜치로 통합한다.
   
 ## stash
  - 파일의 변경 내용을 일시적으로 기록해두는 공간.
  - 변경은 되었는데, commit이 안된 내용을 일시적으로 저장한다.
  
  ## Branch merge
  - 작업이 끝난 branch를 다시 master branch나 branch끼리 합치는 것.
  - ```merge```는 여러 branch를 1개로 합칠 수 있다.
  
  1. ```fast-forward```(빨리 감기)
   - 다른 branch에 master의 변경사항 없는 이력도 가지고 있다면, master를 작업이 끝난 branch로 이동함으로써 병합이 된다.
 이게 ```fast-forword```이다.
  - 빨리감기 전
  ![빨리감기 전](https://backlog.com/git-tutorial/kr/img/post/stepup/capture_stepup1_4_1.png)
  - 빨리감기 후
  ![빨리감기 후](https://backlog.com/git-tutorial/kr/img/post/stepup/capture_stepup1_4_2.png)
  - ```non-fast-forward``` : master와 merge한 branch가 남아 있어 그 branch로 실행한 작업 확인 및 branch 관리 면에서 더 유용하다.
  2. ```merge commit```(병합 커밋)
   - 이력이 계속 남아있다.
   - fast-forward와 다르게 master에 변경 이력이 있고, 다른 branch와 merge할 경우```merge commit```을 실행한다.
  
  3. rebase
   - branch가 master에 merge될 때 branch의 작업 이력이 master 이력에 추가가 된다.
   - branch의 내용과 master의 commit 버전과 충돌나는 부분이 생기는데, 이는 직접 수정해줘야 한다.
   - 원래의 commit이력이 변경되기 때문에 사용하면 안된다.
   
   
   
   topic branch에 통합 branch의 최신 코드를 적용하는 일이라면 ```rebase```를 사용한다.
   통합 branch에 topic branch를 불러올 경우 우선 rebase를 한 후 ```merge```를 한다.
   
   
   https://backlog.com/git-tutorial/kr/stepup/stepup1_5.html
