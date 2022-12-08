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
[oh my zsh](https://ohmyz.sh, "oh my zsh")

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
