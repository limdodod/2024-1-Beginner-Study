Git와 Github
============

 Git log
---------------------

    : commit 기록을 최신 순으로 확인
    : --oneline 옵션을 사용하면 각 커밋을 한줄에 요약


  Commit ld
---------------------
    : commit의 식별을 위해 사용하는 16진수

   
  HEAD
---------------------
    : 현재 작업 중인 위치
    : 현재 작업 중인 브랜치의 가장 최근 commit
    : 다음 commit의 base가 되는 commit
    : 새로운 commit이 생기면 HEAD도 변경

  commit--amend
---------------------
    : 마지막 commit의 내용에 변경이 있을 때 사용
    : 완전히 새로운 commit으로 대체
    
    > 'm' 옵션으로 commit 메시지 수정 
      -> $git commit --amend -m"commit message"
    > '--no edit' 옵션으로 commit 메시지 수정 없이 commit 수정
      -> $git commit --amend --no-edit

   reset
---------------------
    : commit 제거
    : 돌아갈 commit의 id 사용
      $git reset '--option'"<commit id>"

    1. reset --soft
      - 커밋만 취소
      - 변경 사항이 staging area로 돌아감

    2. reset --mixed
      - 커밋을 취소
      - 변경 사항을 working directory로 돌아감

    3. reset --hard
      - 커밋을 취소
      - 변경사항을 모두 제거하고 이전 커밋으로 돌아감

 revert
---------------------
     : 커밋을 제거하지 않고 되돌림
     : 되돌리기 위한 새로운 커밋 생성

     > revert --no-edit
       - 편집기 진입 없이 바로 revert 가능
         $git revert --no-edit "<commit id>"
       - 직접 commit하지 않고 revert 내용을 staging area에 올림