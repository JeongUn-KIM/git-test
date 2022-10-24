Reset Test file

- - reset : staging이나 commit을 취소. 커밋x
    
    `--soft` 
    
    - add 만 한 상태
    - commit 취소
    - HEAD가 가리키는 커밋 이동
    
    `--mixed` *(default)* 
    
    - working dir 내용 유지
    - commit 취소, add 취소
    - Index를 HEAD가 가리키는 상태로 이동
    
    `--hard`
    
    - working dir 내용까지 해당 커밋 상태로 변환
    - 워킹 디렉토리를 Index의 상태로 전환
    - 복원 불가!!

> push 하기 전에 commit 만 취소하는건 reset 명령어로 왓다갔다 할 수 있는데 
origin 에 push 한 상태라면, reset 으로 commit 을 되돌리고 git push -f origin main 으로 
강제 push 를 해줘야 원격 리포지토리에 반영된다.
