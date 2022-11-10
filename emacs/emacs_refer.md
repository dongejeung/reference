
## Emacs references

# for GUI Interface

Install :

in archlinux => sudo pacman -S emacs


set Hangle(GUI emacs)
> toolbar > Options > Multilingual Environment > Set Language Environment > Korean

 
Settings : in editor
alt-x > customize


Cursor move :
(Shift) Tab 


set font : 
> toolbar > Options > set Default Font


view tutorial :
C-h t

Capital C means Ctrl / it means Control
Capital M means META or EDIT or ALT
- means combine
ESC means 


short keys :

Exit emacs : C-x C-c

C-v : move page forward
ESC v : move page backward
C-l : 커서를 중심으로 화면을 커서가 하단/중단/상단 에 오는 위치로 변경해줌.


move cursor :
             C-p(previous)
C-b(back)      cursor        C-f(forward)
              C-n(next)


C-p 이전 라인
C-n 다음 라인
C-b 이전 한 문자
C-f 다음 한 문자

M-f 다음 문자
M-b 이전 문자


cf) 대부분의 Meta 문자는 언어가 정의하는 단위(낱말, 문장, 단락)의 작동에 사용되고,
제어 문자는 편집하는 것과는 관계없는 기본 단위(문자, 줄 등등)에 사용됨.


-------
HHKB 특성상,
좌우위아래, home, end, pgdn, pgup 은 오른손으로 조작하는 게 낫겠다.

C-n : 다음 줄로 이동
C-p : 이전 줄로 이동 
M-a : 문장앞으로 이동
M-e : 문장 뒤로 이동
C-l : 커서 위치를 중심으로 상, 중, 하로 이동.


C-x C-c : emacs 종료
M-< : 맨 앞으로 이동
M-> : 맨 뒤로 이동

C-u n : 다음에 하는 동작을 n 회 만큼 반복
(M-n 도 가능)

C-g : emacs 동작 중지

C-x 1 : 창을 하나만 남기기


지우기

Backspace : 직전 한 글자 지우기
C-d : 직후 한 글자 지우기

M-bs : 직전 한 낱말 지우기
M-d : 직후 한 낱말 지우기

C-k : 커서 위치로부터 줄 끝까지 죽이기
M-k : 현재 문장의 끝까지 죽이기

C-@(C-SPC) 커서 이동 C-w : 두 범위 사이 글자 삭제


cf) 죽이기 는 잡아당기기(yanking) 으로 다시 살릴 수 있음.
지우기는 다시 살릴 수 없음.

C-k : 커서 부터 줄 끝까지 지우기. 한 번 더 하면 빈 공간 올려짐.
C-y : 최근 죽인 부분 되살리기.
M-y : 죽인 것들을 계쏙 되살리기


C-x u : 무르기
(C-/ 도 됨.)


C-x C-f : 파일 찾기

cf) minibuffer : 최하단의 입력공간.

C-x C-s : 파일 저장.(갈무리라고 써있냐)



