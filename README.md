# golang

환경 구성
- OS: Windows 11 X64

**WSL2, Ubuntu 설치**
1. DISM(배포 이미지 서비스 및 관리) 명령어로 Microsoft-Windows-Subsystem-Linux 기능 활성화
- dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

2. DISM 명령어로 VirtualMachinePlatform 기능을 활성화
- dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

3. x64 머신용 최신 WSL2 Linux 커널 업데이트 패키지 설치
- https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi

4. 재부팅

5. WSL 기본 버전 2로 변경
- wsl --set-default-version 2

6. Microsoft Store 에서 Ubuntu 설치

7. 설치된 Ubuntu 버전 확인
- wsl -l -v

8. 설치된 WSL2 업데이트
- wsl.exe --update

9. Ubuntu 터미널 실행 후 확인

**Ubuntu 와 vscode 연동**
1. vscode 확장ㅇ서 wsl 설치
2. 우분투 터미널에서 code . 입력 -> 해당 디렉터리 위치에서 vscode 자동 실행

**WSL2, Ubuntu, vscode 에서 git 연동**
1. git 관련 모든 소프트웨어 설치
  - sudo apt-get install git-all
2. 사용자 설정
  - git config --global user.name ____
  - git config --global user.email ____
3. vscode 에서 git repository 생성
  - vscode 에서 Ctrl + Shift + G
  - Initialize Repository 클릭
4. git 웹에서 레포지토리 생성 후 remote 연동
5. vscode 확장에서 git graph 설치


