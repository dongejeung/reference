
## Emacs references

# for GUI Interface

Install :

in archlinux => sudo pacman -S emacs


set Hangle(GUI emacs)
> toolbar > Options > Multilingual Environment > Set Language Environment > Korean

 
Settings : in editor
M-x > customize


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


cf) 기본적으로 동작을 할때 기본위치를 정하고 움직임을 습관화하는 게 좋을 것 같다. 특히 HHKB 에 맞춰서 말이다.

- 기본 위치는 f, j 로 홈이 있는 위치를 가장 기본 중심위치로.
- 숫자 중립은 왼손은 1, 오른손은 6을 기준으로 좌우 공백 위치를 기억.
- Fn 키는 우측에만 존재. Fn은 입력할 일이 굉장히 잦고 새끼손가락을 사용. 그러면 상대적으로 M까지의 거리가 더 멈. 한영키도 오른쪽으로 바인딩해서 쓰기 때문에, 
Ctrl, Alt 는 주로 왼쪽을 쓰는 게 나을 듯 하다.
Shift 는 양쪽을 병행해서 써도 괜찮을 것 같고, 
사실 습관이 그렇게 들어서 그렇지 
Backspace, Enter를 중지로 칠 필요없이 새끼손가락으로 쳐보는 시도를 해보는 것도 괜찮을 것 같다.
- Del 키는 입력하기가 좀 더러운데 새끼 손가락으로 칠 경우에는 타건이 불편하다. 차라리 엄지 중지를 쓰는 것이 나을 것 같다. 하지만 보통의 에디터에서는 다른 키들을 이용하여, Del 키 사용을 거의 안할 수 있을 것 같다.
- 우상단의 \(|), `(~) 같은 키는 사실 쓸일이 많지 않다. | 정도는 구분자나 스크립트 사용시 쓸일이 종종 있지만, 해당 위치는 지금 숙지 되어 있다.
- 많이 헷갈리는 것은 숫자와 특수기호의 위치가 헷갈린다는 것이다. 왼손 숫자의 경우 Esc 제외하고 위치를 잡으면 되지만, 오른손은 오른쪽 4칸은 띄우고 중립을 잡아야하기 때문에 숙지가 많이 필요한 것 같다. 감각을 숙달시키는 중이다.
- 특히 자주 틀리는 것은 *() 이런 특수기호들이다. 쓸일이 많고 Shift 키를 이용해서 쓰기 때문에, 헷갈리기 쉽다. 어차피 무각이기도 하고 보지 않고 숙달시켜서 치고, 자주 치는 특수기호들을 고려했을 때에 우측 숫자 중립위치를 두 칸 띄우고 잡는 것이 더 좋겠다. 그리고 좌 Shift 활용도를 높이자.
그리고 좌측 area 의 키를 입력할 시는 우 Shift 를 그 밴대는 좌 Shift 를 활용하는 식의 전략을 쓰는 것이 좋을 것 같다.
Shift는 역시 좌우를 convert 해서 쓰는 것이 좋을 것 같다.
- 왼손 키보드 라인은 t g b 오른손 키보드 라인은 yhn 로 잡다. 그게 편한 것 같다. 
- 특수기호와 숫자의 위치는 좀 더 숙지할 필요가 있는 것 같다. 
- 아까 정한 기준상에서는 오른손 검지, 중지가 90() 이다.
- 항상 동선최소화와 습관화를 하자. 
- 쓸데없이 검지, 중지만을 많이 사용하는 습관을 바꾸자. 그리고 엄지는 최하단의 다섯키 위주로 사용하는 것 같다.
- 처음에는 차라리 천천히 치더라도 정확한 손가락으로 숙달시켜 나가는 것이 중요한 것 같다. 초반에 타건 습관을 어렸을 때 부터 제대로 잡지 않은 부분이 있기 때문에 동선이 좋지 않는 부분이 꽤 있는 것 같다.

- 키보드 타건은 모든 타건에서 숙달 시키기로 하고,
emacs 는 이동기부터 숙달. help 구문 불러오기나 기타 기능별로 확장해 나간다.
- vim 같은 경우도 안주하지 말고, 개선의 연습이 필요하다.
- LISP 이나 확장된 emacs 사용도 꾸준히 해주도록 하자.
- 조바심 낼 것 없이 꾸준히 체계적인 노력을 해준다면, 발전한다.

- 방향키는 중지로, pgup pgdn home end 키는 검지를 사용하는 편이 좋은 것 같다. emacs 사용시에는 해당 이동은 오른손을 쓰는 것이 낫지 싶다. 

- 사실상, C-f C-b M-f M-b C-n C-p C-a C-e 의 이동은
모두 위의 오른손 Fn 조합만을 가지고 이동할 수 있다.

- 주로 사용하게 될 것은 M-a M-e 의 기능인데 이 때에는 오른쪽 M 을 이용하는 것이 좋을 것 같다. 누르고 있으면 연속입력으로 인지된다는 것을 생각하자.

- C-u(M)-숫자 의 반복 매크로 기능은 위의 방향키나 pgup 등의 조작에도 유효하다는 것을 확인 하였다.
M 키의 입력이 한 글자 덜 쳐서 편할 것 같지만, 사실상 10회 이상의 반복의 경우에는 M 키를 누르고 있는 게 더 불편할 수 있다. 걍 C-u 를 습관화 시키자.

- vim 의 모드처럼 emacs 의 hierarchy를 고려하는 사고는 굉장히 중요하다. hierarchy 의 개념 자체가 매우 중요하다.
 
- 그래 신체구조상 Fn 키를 사용하다 보면 우 Shift 등하고 헷갈릴때가 많은 것 같다. 우 Shift 를 약지에 바인딩하는 습관을 들여보자.

- emacs tutorial 파일 TUTORIAL.ko 의 확장자를 md 로 변경한 후, zshrc 파일에다 alias 로 크롬으로 여는 단축키를 지정해 놓음. 해당 파일을 초반에는 열어놓고 연습해 나가자.

- 야임마 buffer 를 사이칸 저장을 갈무리로 번역하는 것은 번역기를 돌린 것인 것인가.. ㅋㅋㅋㅋ


cf) 죽이기는 kill, 삭제는 delete 이다.

C-SPC cursor move C-w : 범위 죽이기.
C-x C-f : find file. (use tab to autocomplete)
C-x b : chg buffer
C-x C-b : show buffer list
C-x s : save some buffer
C-x C-s : save buffer

- short key 가 영어 단어와 관련이 있다는 것을 염두해두면 암기하기가 쉽다.


chg theme
in scratch
(load-theme 'tango-dark)
C-x C-e


# emacs 로 개발환경 구축하기
https://panty.run/lisp-devel-with-emacs/

# 오픈소스SW 라이선스 종합정보시스템
https://www.olis.or.kr/

git clone https://aur.archlinux.org/clisp-git.git
makepkg -si

slime mode 실행시 에러 발생


