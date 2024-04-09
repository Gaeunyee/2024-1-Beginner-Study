# 브랜치 전략

협업에서 서로의 작업에 영향을 주지 않으려면...

- 브랜치 분리
- 브랜치 구분
- main(배포 버전)브랜치의 안전한 관리

    Pull Request를 병합할 때 승인 절차 추가
    Push가 가능한 인원을 제한

## git flow - 브랜치 관리 전략

    2010년에 Vincent Driessen이 고안...

    <https://nvie.com/posts/a-successful-git-branching-model/>

### main Barnches

영원히 존재함 (삭제x)
    - main(master)
        배포 버전, 병합될 때 새 버전 탄생
    - develop
        feature 브랜치의 기반

### Supporting branches
    - feature
        develop에서 분기된 브랜치

        기능 개발 완료 후 develop으로 병합

        이름은 마음대로 지어도 됨
    - release
        develop에서 분기된 브랜치
        
        배포 준비, QA작업

        main에 병합
    - hotfix
        긴급 수정이 필요할 때 사용

        main에서 분기된 브랜치

        main, develop 모두에 병합

## github flow
gitflow의 대안으로 제시된 방법

수시로 배포되는 상황에 어울림

### main
    항상 배포 가능한 상태로 유지
    main 병합 전에 충분한 테스트!

### feature
    feature 이외 브랜치를 구분하지 않음

    main -> feature -> main
    
    브랜치의 이름에 목적이 잘 담겨 있어야 함

    코드 리뷰가 매우 중요! 바로 배포되기 때문에 특히 더 조심해야..

# 개발자로서의 Attitude

## convention을 지키자

긴 시간이 지난 후에도 의도를 파악하기 쉽다.

보기 좋은 떡이 먹기도 좋다고...

## 구글링과 GPT의 중요성

직접 찾아보고 진짜 모르겠을 때만 도움을 요청하자.

고생을 해야 실력이 는다!

## 코드 예쁘게 만들기

public repository의 코드는 개발자의 얼굴과 같다..

잘 설계된 예쁜 코드를 만들어보자.
convention도 잘 지키고...

## 좋은 질문을 하자

물어볼 것을 명확하게 인지한 채로 질문하자.