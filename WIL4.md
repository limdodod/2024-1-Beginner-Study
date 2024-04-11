Git와 Github
============

 브랜치 전략
---------------------
### Git Flow Vs Github Flow

# Git Flow
    Main Branches: 
    main(master), develop

    Supporting branches: 
    feature, release, hotfix

1. main

    : 프로젝트 생성 시 기본으로 생성되는 브랜치
    : 영원히 존재하는 첫번쨰 브랜치
    : 병합될 때마다 제품의 새로운 버전 탄생
    : main 대신 master 사용하기도 함

2. develop

    : 영원히 존재하는 두번째 브랜치
    : feature 브랜치의 기반

3. feature

    : develop 브랜치에서 분기하여 작업
    : 기능 개발 완료 후 develop으로 병합

4. release

    : 배포 준비를 위한 브랜치
    : 버그 수정 + QA 작업
    : develop 브랜치에서 분기해 main 브랜치로 병합

5. hotfix

    : 배포 환경에서 즉각적인 수정이 필요한 경우
    : main 브랜치에서 분기
    : main, develop 모두에 병합

# Github Flow
    Main & Feature 브랜치만 사용
1. main

    : 항상 배포 가능 상태로 유지
    : main으로 병합 전에 test 필요

2. feature

    : main 분기-> 작업-> main 병합
    : 브랜치의 목적을 이름에 담아야 함
    : Git Flow에 비해 코드 리뷰 중요

