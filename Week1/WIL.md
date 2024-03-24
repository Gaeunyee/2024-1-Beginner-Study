##Git으로 폴더 관리하기

Terminal -> powershell 옆 + -> Git Bash

$ git init . // 폴더 생성 시 초기화

$ rm -r .git // 관리 그만두기

##Git으로 관리 대상 파일 등록하기

$git add (파일명) // 하나씩 등록

$git add . // 모든 파일 등록

$ git rm ---cached (파일명) // unstage로 되돌리기

##파일 로컬 저장소로 옮기기

$git commit -m (커밋 메시지) 

###커밋 메시지의 종류
- feat - 새로운 기능 추가
- refactor - 기존 코드 개선
- fix - 버그 수정
- chore - 코드 외 설정 변경
- docs - 문서화
- test - 테스트 코드

##GitHub 업로드 전 작업

$ git remote add origin (주소) // 주소는 깃허브 리포지토리에서 복사

$ git branch -M main

$ git push -u origin main

##Github에 업로드하기

$ git add (파일명)
$ git commit -m (커밋 메시지)
$ git push origin main

[Gaeunyee] (https://github.com/Gaeunyee/Gaeunyee)

