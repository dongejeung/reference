C-h t : show totorial
C-x C-c : Exit emacs 
C-g : emacs 동작 중지
C-x 1 : 창을 하나만 남기기(1 대신 다른 숫자 입력시 해당 개수만큼 창이 쪼개짐)

C-u n : 다음에 하는 동작을 n 회 만큼 반복
(M-n 도 가능)

## 이동
C-v : move page forward
C-l : 커서를 중심으로 화면을 커서가 하단/중단/상단 에 오는 위치로 변경해줌.
             C-p(previous)
C-b(back)      cursor        C-f(forward)
              C-n(next)
C-p 이전 라인
C-n 다음 라인
C-b 이전 한 문자
C-f 다음 한 문자
M-f 다음 문자
M-b 이전 문자
C-n : 다음 줄로 이동
C-p : 이전 줄로 이동 
M-a : 문장앞으로 이동
M-e : 문장 뒤로 이동
C-l : 커서 위치를 중심으로 상, 중, 하로 이동.

M-< : 맨 앞으로 이동
M-> : 맨 뒤로 이동

## 편집 
- 지우기
C-d : 직후 한 글자 del
M-bs : 직전 한 낱말 del

M-d : 직후 한 낱말 kill
C-k : 커서 위치로부터 줄 끝까지 kill
M-k : 현재 문장의 끝까지 kill
C-@(C-SPC) 커서 이동 C-w : 두 범위 사이 글자 kill 
C-k : 커서 부터 줄 끝까지 지우기. 한 번 더 하면 빈 공간 올려짐.

- 되살리기(yank)
C-y : 최근 죽인 부분 되살리기.
M-y : 죽인 것들을 계쏙 되살리기

- 무르기
C-x u : 무르기. del 도 실행취소 가능. 단계별로 연속 가능.
(C-/ 도 됨.)
C-_ : C-/ 와 같은 작용

- 바꾸기
M-x replace-string(repl s<TAB>) : 전역으로 문자치환.
(현재 커서 위치부터 끝까지 바꾼다.)


## 탐색 브라우저
C-x C-f : 파일 찾기
C-x C-s : 파일 저장
C-x b : chg buffer
C-x C-b : show buffer list
C-x s : save some buffer
C-x C-s : save buffer


## 검색
C-s : 검색.(incremental)
C-r : reverse search.



## 기타
C-x : 문자 확장. 문자 하나가 뒤따름
M-x : 이름 명령의 확장. 긴 이름이 뒤따름
C-z : emacs 임시로 나오기
=> fg / %emacs 명령으로 resume 가능
(윈도우 모드에서는 걍 최소화 되어 있음.)
M-x recover-this-file : 주기적으로 auto save 된 파일로 복구.
(file 이름 앞뒤로 # 이 붙음. .swp 과 유사.)


## 편집 모드 : 주 편집모드는 항상 하나.
Fundamental / Lisp / Text / etc
M-x Fundamental-mode : 모드 변경
C-h m : documentation on your current major mode.
M-x auto-fill-mode : 마이너 모드. 자동완성.

cf) 모드는 메이저 모드, 마이너 모드가 있음.
마이너 모드는 on/off 방식으로 동시에 사용 가능.


MULTIPLE WINDOWS
C-M-v to scroll the bottom window
C-x o(other) move cursor other window



...
M-x customize-themes
M-x package-install RET modus-themes RET
M-x load-theme RET modus-vivendi RET

Java settings
M-x package-install use-package
M-x package-install lsp-java
M-x package-install dash
야이씨 안되잖아.. ㅋㅋㅋㅋ

https://xpressrazor.wordpress.com/2020/11/04/java-programming-in-emacs/


