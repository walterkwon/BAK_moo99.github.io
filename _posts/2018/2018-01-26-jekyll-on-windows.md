---
layout: "post"
title: "Jekyll on Windows"
date: "2018-01-26 01:10"
---


## 0단계: Enable the "Windows Subsystem for Linux"

1. Window Power Shell을 '관리자 권한으로 실행'
2. Power Shell 입력창에 다음의 명령어 실행

  `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`


## 1단계: [Install the Windows Subsystem for Linux](https://goo.gl/hwaVQP)

1. 윈도우 스토어에 가서 마음에 드는 Linux distribution를 골라서 다운로드한다.
2. 다운로드가 끝나면, "실행"을 선택
3. UNIX username 과 password를 설정


### 2단계: Update our repo lists and packages

1. 명령 프롬프트(CMD) 실행
2. 입력창에 'bash'를 입력하여 Command Prompt instance를 Bash instance로 전환
3. 아래의 명령어 실행

  `sudo apt-get update -y && sudo apt-get upgrade -y`

4. (업데이트하고 설치하는데 시간이 꽤 걸림) 기다림

### 3단계 : Install Ruby

1. 명령 프롬프트(CMD) 실행
2. 아래의 명령어 실행

  `sudo apt-add-repository ppa:brightbox/ruby-ng`

  `sudo apt-get update`

  `sudo apt-get install ruby2.3 ruby2.3-dev build-essential`

### 4단계 : Ruby gem 업데이트

1. 아래의 명령어 실행

`sudo gem update`

### 5단계 : Jekyll 설치

1. 아래의 명령어 실행

`sudo gem install jekyll bundler`

2. 설치가 잘 되었는지 확인

`jekyll -v`
