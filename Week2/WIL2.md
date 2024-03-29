Git와 Github
============

 GitHub의 Fork/Star
---------------------

 1. Fork

    : 다른 사용자의 Repository를 자신의 계정으로 복사하여 독립적으로 수정& 관리

 2. Star

    : 관심있는 Repository나 프로젝트에 star을 달아 관리

   GitHub의 Issue
---------------------
    : Ropository에서 작업 계획, 토론 및 추적을 위해 활용

   
  GitHub의 Branch
---------------------
    : 기존 브랜치에서 분기되어 생성되는 별도의 작업 공간
    : fork와 달리 같은 Repository에 생성

+ Branch Naming Convention

    > "type/<issue 번호>-<간략한 설명>"

  1. Branch 확인하기
      - 현재 브랜치 확인: $git branch
      - 모든 브랜치 확인: $git branch -a

  2. Branch  생성/삭제
      - 브랜치 생성하기: $git branch "<브랜치 이름>"
      - 브랜치 삭제하기: $git branch -D "<브랜치 이름>"
  
  3. Branch 이동하기
      - 브랜치 이동: $git checkout "<브랜치 이름>"
      - 브랜치 생성 후 이동: $git checkout -b "<브랜치 이름>"
      
GitHub의 PUll
---------------------
    : 분기된 Branch를 다시 병합하기 위한 절차
    : 새로운 변경 제안/ 병합 시 발생하는 충돌 해결
    : Merge에 앞서 코드 리뷰

GitHub의 Merge
---------------------
1. Merge Commit
    : 두 브랜치를 공통 부모로 하는 새로운 commit 만듦
2. Squash and Merge
    : 하나의 커밋으로 main 브랜치로 병합
3. Rebase and Merge
    : 커밋의 base 재설정 -> 모두 새로운 커밋으로 변경


<https://github.com/limdodod/2024-1-Beginner-Study/pull>