# git 기초

.git이라는 폴더는 무엇인가요? 
    커밋이 담겨져 있는 폴더
.git 폴더를 만드는 방법.
    git init

project 폴더?
    내가 작업할 수 있는 공간. (지금은 )

project 폴더에서 git init을 써라
앞으로 0214 디렉토리는 git으로 관리하겠다.

source tree GUI환경에서 하는것. 다운받는 건데 이번에 안함.
cli로 깃을 관리할 줄 아는 사람이 사용할때 빛을 발함...
gui는 개념이 확실해야한다.

git 도움을 주는 확장앱 설치
>git graph

git log 커밋됐던 히스토리를 알 수 있다.
알파벳 j 눌러도 내려가고 방향키 내려도 내려감.

1.gitignore
git init 하면 .git 폴더 생성.
내가 굳이 올릴 필요가 없는 파일 혹은 디렉토리
ex) 
아이디와 패스워드를 저장하는 text파일.
node_modules 코드가 많다.
package-lock.json 

-1 프로젝트 폴더에서 .gitignore 파일 생성.
파일 안에 안올리고 싶은 파일의 이름을 적는다.
*: 모든 파일  ex) *.js


2.reset,revert
커밋을 뒤로 돌아가는 행위
reset 지우는 싶을 때 사용.
git reset --hard [돌아갈 커밋 hash]
revert 4개중 3번째것만 삭제 하고 싶을 때. 
git revert [삭제할 커밋 hash값]


3.branch
커밋을 나누는 행위
특정 시점이나 마지막 시점에서 다른 코드로 만들 수 있는것,,

4.merge, rebase
커밋을 합쳐주는 행위

동그라미 
암묵적으로 '변경된 사항만' 길 폴더 안에 저장된다. 
5만줄 중에 1만줄만 저장되는 것.

구글클라우드와는 다르다. 텍스트로 저장하는 구조이기 때문에. 21분부터 다시 보기.

장점: 용량은 최소화, 기능은 좋다.
단점: 어려움.

깃 삭제
git rm -r [파일명] 로컬과 원격저장소를 다 지우는 행위
git rm --cached -r [파일명] 원격 저장소에서만 지움.

origin 원격저장소의 이름.

git clone [git hub 주소]
복사 붙여 넣기.

피링섹 원격 저장소에 잘 있을때
빨강색 원격저장소에 없음.

git clone: 최초에 가져오는 거
git pull: 최초 다음부터 가지고 오는 것.