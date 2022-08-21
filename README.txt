Git 폴더 설정 방법
1. 해당 폴더에서 아래 명령어 실행
 -. git init
 -. 대상폴더 : /Users/admin/workspace/contents
2. 실행 결과가 아래와 같으면 성공
 -. Initialized empty Git repository 
3. email, name 설정
 -. git config --global user.email "seingyo@naver.com"
 -. git config --global user.name "Ryan"

첫 커밋 테스트
1. 커밋
 -. git add README.txt 
2. 해당 커밋에 설명 추가
 -. git commit -m "첫 커밋 테스트"

git log 확인
 -. git log

commit 111d51385e13641ec9c9990a5af35e9dce7f89c8 (HEAD -> master)
Author: Ryan <seingyo@naver.com>
Date:   Sun Aug 21 14:25:47 2022 +0900

    두번째 커밋

commit 7165a0f170c4fb3d171c95fbaf9d14717b27d954
Author: Ryan <seingyo@naver.com>
Date:   Sun Aug 21 14:22:16 2022 +0900

    첫 커밋 테스트

[첫 커밋으로 돌아가기]
 -. git checkout 7165a0f
Note: switching to '7165a0f'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 7165a0f 첫 커밋 테스트

[git 폴더가 아닌곳에서 git 명령어 실행시 오류]
fatal: (현재 폴더 또는 상위 폴더 중 일부가) 깃 저장소가 아닙니다: .git

[원격저장소에 커밋 올리기]
1. github에저장소 만들어 놓기
 -. https://github.com/21ckorea/study
2. 로컬저장소에 원격저장소 주소 알려주기
 -. git remote add orgin https://github.com/21ckorea/study.git
3. 원격저장송에 올리기
 -. git push origin master
 -. origin이라는 미리 정의한 원격저장소에 master 브랜치로 올리겠다
 -. name, password를 넣어야 되는데 name은 github에 찍힐 이름이고
 -. 패스워드는 github에 가입한 패스워드인데 패스워드 방식에서 토근 방식으로 바
뀜
 -. https://hyeo-noo.tistory.com/184 사이트 보고 따라해서 토큰 만든 후
 -. password에 토큰을 넣으면 됨
 -. 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

