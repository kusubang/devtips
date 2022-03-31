# WSL 
윈도우즈에서 WSL 디렉토리 찾아가려면 윈도우즈 탐색기의 주소창에 다음과 같이 입력한다.
```
\\wsl$
```
terminal 열때 패스워드 물어 보지 않기  
```
- start wsl2 terminal
- sudo visudo
```
add the following line to the end of the file
```
YourUsername ALL=(ALL) NOPASSWD: ALL
```
ref: https://blog.yavuz.support/stop-wsl2-from-asking-for-sudo-password


### Change font color settings in Ubuntu terminal on WSL
윈도우 디렉토리의 폰트 백그라운드가 표시되어 보기 어렵다. 이럴때는 다음과 같이 한다.

```bash
dircolors -p > ~/.dircolors
```
다음과 같이 수정한다.
```
DIR 01;36 # directory
LINK 01;32 # symbolic link. (If you set this to 'target' instead of a  

OTHER_WRITABLE 01;36 # dir that is other-writable (o+w) and not sticky
```

마지막으로 `eval $(dircolors -b ~/.dircolors)` 실행해서 적용한다.


ref: https://estuarine.jp/2020/09/windows-terminal/?lang=en
