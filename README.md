# global-setting

# MAC setting
출처: [Nomad Coders][nomadlink]

[nomadlink]: https://www.youtube.com/watch?v=B26yiuC5zPM "Thank you Nico!!"

## <i>step.1 install homebrew</i>
[home brew](https://brew.sh/index_ko)

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## <i>step.2 install program</i>
```
brew install --cask visual-studio-code google-chrome iterm2
```

## <i>step.3 iterm2 setting</i>
1. 좌측 상단 iTerm2 클릭
2. Preferences -> Appearance -> Theme: Minimal 변경
3. Preferences -> Profiles -> Session -> Status bar enabled 체크 후 좌측 Configure Status Bar 선태 -> battery, CPU, Memory 하단을 드래그하여 설정
  + 하단 Auto-Rainbow: Light Colors 설정

## <i>step.4 iterm2-color-schemes setting</i>
[iTerm Themes](https://iterm2colorschemes.com)

위 사이트에 방문하여 GitHub Dark 클릭 -> <kbd>⌘</kbd> + <kbd>s</kbd> 버튼으로 파일 저장<br>
  -> 다운로드 된 디렉토리로 이동하여 저장된 파일의 확장자(.txt)를 지우고, 파일을 실행항 테마르 적용시킨다.
  
그 후에 Preferences -> Profiles -> Colors -> 우측 하단의 color schemes를 다운받은 스키마로 변경!

## <i>step.5 install oh my zsh</i>
[oh my zsh](https://ohmyz.sh)

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
터미널에 해당 명령어를 입력하여 oh my zsh 설치

## <i>step.6 oh my zsh 꾸미기 Powerlevel 10K</i>
[powerlevel10k](https://github.com/romkatv/powerlevel10k)

1. 해당 링크로 접속 후, Installation -> Oh My Zsh -> 1. Clone the repository 의 코드를 터미널에 입력하여 설치
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

2. 해당 코드로 설정 파일을 vscode로 연다.
```
code ~/.zshrc
```

그리고 아래와 같이 파일을 수정해준다. (line. 11)
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```

후에 iterm2를 종료하고, 다시 시작하면 테마 설정 화면으로 넘어간다.

## <i>step.7 pwerlevel10k 꾸미기</i>
1. 재시작 시 폰트 설치 여부를 묻는다. -> y(yes)
2. 그 후 다시 iterm2를 실행하면 폰트들이 제대로 보이는지 확인한다.(검사 진행)

> 에러 발생!<br>
> 만약 폰트 검사를 하는데 깨져서 나온다?<br>
> Preferences -> Profiles -> Text -> Font: MesloLGS NF로 변경!!

3. 이제 아래와 같은 설정으로 진행한다. (custom 가능.)
```
(2) Classic.
(1) Unicode.
(3) Dark
(2) 24-hour format.
(1) Angled.
(1) Sharp.
(1) Flat.
(1) One line.
(1) Compact.
(2) Many icons.
(1) Concise.
(n) No.

설정 적용
(1) Verbose (recommended)
(y) Yes (recommended).
```

## <i>step.8 install gh</i>
1. install gh
```
brew install gh
```

2. gh auth login
```
gh auth login

Github.com
HTTPS 선택
Yes
Login with a web browser 선택
```
화면에 보이는 코드를 browser에 입력 후 연결 완료

## <i>step.9 vscode extension</i>
```
Prettier - Code formatter
Material Icon Theme
Community Material Theme
```

vscode terminal 아이콘 깨짐 현상 해결<br>
Settings -> terminal font 검색 -> Terminal > Integrated: Font Family: MesloLGS NF 입력<br>

확인해보면 아이콘이 제대로 나옴!
