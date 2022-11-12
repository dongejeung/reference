
# archlinux 사용 History

- image : ARCH_202210
- gui interface : gnome
- 뭐 이 같은 수행을 해도 왜 됐다 안됐다 하냐? what the..
-------
 history : rufus 를 이용해 bootable usb 만듬. 
 기존 nvme01의 내용 삭제.
boot with usb

dd if=/dev/zero of=/dev/nvme0n1 bs=512 count=xxxx
(꼭 필요한 작업인지는 모르겠음)

parted -l => 파티션 내용 확인. 

기본적으로 archinstall 을 이용해 install 함.
자꾸8192 에러 발생. 
kde 로 깔았다가, gnome 으로 interface 변경해서 재설치.
같은 수행을 여러 번 시도했는데, 갑자기 될 때가 있음...
kde 환경에서 한글 입력기에 이슈가 있어 scim 시도 실패.
fcitx 부분 에러. bluetooth keyboard 인식이 안됐다가 갑자기 됨. 
pacman -S bluez-utils 인가 설치하고 그럼.
nimf 입력기 설치중에 qt4 의존성 문제로 설치하는데 너무 오래걸려서 끔.
걍 가벼워 보이는 gnome 으로 재설치. 
gnome 에서 nimf 설치중에 잘 안됨. gnome 이라 걍 ibus 한글 입력기 설치.
터미널에서 backs, enter 사용시에 한글일 경우 잘 동작 안하는 이슈 있는데 그냥 사용하는 중. 
인스톨시 설치할 프로그램으로 동영상 가이드대로 firefox vim htop neofetch 셋팅.
partition 은 wipe and suggested partition layout select.
not seperate /home for user. 
mirror region => south korea
set root pwd
add user
desktop > gnome > nvidia prioraty? spell 헷갈림. 
use networkmanager


settings :
gnome extension :
https://extensions.gnome.org/
recommendation of gnome extension :
vitals
openweather




locale set ko_KR.UTF-8
pacman -S terminus-font noto-fonts-cjk ttf-dejavu
edit local.conf with xml 
google-chrome stable 설치.   


pacman package list :
vlc => for video 
gdm => for font
clipgrab => for video download for example youtube video
(cf. youtubedl)
emacs => IDE 
dnf
jdk17-openjdk
xdotool
lxpanel
man
zsh
ripgrep : enhanced grep


aur repo : https://aur.archlinux.org/
download with above site and install with command makepkg -si(for deps)
eclipse-jee 2:4.25-1 => lastest now 

git clone https://aur.archlinux.org/snapd.git
cd snapd
makepkg -si
sudo systemctl enable --now snapd.socket
sudo ln -s /var/lib/snapd/snap /snap
sudo snap install eclipse --classic
위의 내용 말고 걍 이클립스 사이트가서 노설치 버전 받을란다.
https://www.eclipse.org/downloads/
ver : eclipse-jee-2022-09-R-linux-gtk-x86_64.tar.gz
theme : planet-themes => dark
font : basic D2coding bold
plugin : vrapper(for vim style)
etc : error when open .md file.
=> so can't open eclipse 
=> when use eclipse vrapper > content assistant short key is C-/



=> sudo pacman -S webkit2gtk






git clone :
D2fonts > open with file browser & execute


edit bashrc & bash_aliases

bashrc : 
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi

bash_aliases : 
alias ll='ls -l'
alias la='ls -al'

alias bashrc='source ~/.bashrc'
alias goa='sudo vim ~/.bash_aliases'
alias pf='ps -ef | grep $1'


vmware :
Download VMware-Player-Full-16.2.4-20089737.x86_64.bundle
sudo sh *.bundle
dir => /etc/init.d
sudo pacman -S linux-headers

vmmon
vmnet
없다고 오류
dnf kernel-devel 추천
sudo pacman -S dnf


virtualbox :
vmware 대용으로 설치
https://www.virtualbox.org/wiki/Downloads
extension pack Download
https://download.virtualbox.org/virtualbox/7.0.2/
download guestadditions & add odd 
active window top bar > view > fix guest display 
virtualbox > preference > display graphic controller > VBoxVGA(for resize fixel)

  

xdotool : linux macro

move workspace :
xdotool get_desktop : get workspace num
xdotool set_desktop n : move workspace n
set_desktop_for_window : xdotool getactivewindow set_desktop_for_window 0


oh my zsh : 
sudo pacman -S zsh
touch ~/.zshrc
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
PATH : $ZSH => ~/.oh-my-zsh
>>> plugin


zsh plugin :
autousggestions

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions


edit ~/.zshrc
plugins=(git zsh-autosuggestions sudo web-search iterm2 docker zsh-syntax-highlighti    ng copydir copyfile copybuffer dirhistory zsh_reload history jsontools alias-tips)

zsh-autosuggestions : use tab > tab select suggestion

sudo : command + esc * 2

web-search : https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/web-search/web-search.plugin.zsh
> go zsh's plugin path i can edit plugin code maybe

copydir : type copydir
> copy current path to system clipboard
(but it doesn't work in my zsh)

copybuffer : also doesn't work in my zsh

dirhistory : https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/dirhistory
M(alt) + direct key
left : previous dir
right : next directory
up : parent dir
down : first child dir by alphabetical order

history :
h : history
hs hisotry | grep
hsi : history | grep i

jsontools : response json + | pp_json
pp_json : pretty prints.
is_json : returns true if valid json; false otherwise.
urlencode_json : returns a url encoded string for the given json.
urldecode_json : returns decoded json for the given url encoded string.





alias-tips :
cd ~/.oh-my-zsh/plugins
git clone https://github.com/djui/alias-tips.git
export ZSH_PLUGINS_ALIAS_TIPS_TEXT="Alias tip: "


dbeaver :
Download main site
change theme dark. font D2coding
plugin > Vrapper(chg vim pattern)
http://vrapper.sourceforge.net/update-site/stable
아이 위에꺼 설치 에러 나잖아
https://dbeaver.com/docs/wiki/Optional-extensions/
아 디비버는 걍 쓰자 귀찮아서 진짜 



enrole startup scripts : 시작 프로그램 등록하기.
/etc/init.d/
위의 경로에 .sh 파일 넣어두면 된다고 함.
위에 꺼 말고
~/.config/autostart/*
에 넣어두고 권한 설정하면 된다고 함.



