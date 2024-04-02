# commit 되돌리기

## git log

$ git log --online

commit 기록을 최신 순으로 확인

## HEAD

현재 작업중인 위치를 가리키는 포인터
마지막 커밋이 이루어진 장소
HEAD -> [branch name]

## git status

## commit --amend

마지막으로 commit한 내용을 완전히 새로운 커밋으로 바꾼다.

### amend option
- -m : vim 진입 없이 커밋 메시지 수정
- --no--edit : 커밋 메시지를 수정하지 않음


협업 공간에서는 사용하면 안 된다..

##reset
지정한 커밋 아이디의 진행 상태로 돌아간다.

$ git reset --[option] <commit id> //id 이후의 커밋이 모두 삭제됨

### reset option
- soft
    commit만 취소하고, Staging area로 돌아간다.
- mixed
    working directory로 돌아간다.
- hard
    변경 사항을 완전히 삭제한다.

## revert

지금까지의 커밋을 제거하지 않고 이전 상태의 커밋을 새로 생성

- $ git revert --no-edit <commit id>
    편집기에 진입하지 않음
- $ git revert --no-commit <commit id>
    이전 내용을 바로 커밋하지 않고 Staging area에 올린다. (add 다음 단계, 수동으로 커밋함)

reset보단 revert가 더 안전하다.