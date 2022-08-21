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

