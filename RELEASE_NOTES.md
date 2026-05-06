# Roboseasy Studio v0.5.1-0.0.1

## 빠른 설치

### Windows 10/11 (64-bit)

1. [roboseasy-studio-setup_v0.5.1_v0.0.1_win64.exe](https://github.com/roboseasy/roboseasy-studio-deploy/releases/download/v0.5.1-0.0.1/roboseasy-studio-setup_v0.5.1_v0.0.1_win64.exe) 다운로드 (~38 MB)
2. 더블클릭 → SmartScreen "추가 정보" → "실행"
3. Inno Setup 마법사 진행 (5~30분, 인터넷 연결 필수)

설치 가이드: [install_ko.md](https://github.com/roboseasy/roboseasy-studio-deploy/blob/main/install_ko.md)

### Ubuntu 24.04+ (.deb)

```bash
wget https://github.com/roboseasy/roboseasy-studio-deploy/releases/download/v0.5.1-0.0.1/roboseasy-studio_0.5.1-0.0.1_amd64.deb
sudo apt install ./roboseasy-studio_0.5.1-0.0.1_amd64.deb
```

설치 가이드: [install_ko.md](https://github.com/roboseasy/roboseasy-studio-deploy/blob/main/install_ko.md)

## 변경 사항

- 첫 릴리즈
- Linux .deb (정통 Debian 패키징, 설치 시 venv + pip install)
- Windows 인스톨러 (Inno Setup, Python 자동 설치 + venv + pip install + 위저드 안 진행 표시)

## 시스템 요구사항

| 항목 | Windows | Linux |
|------|---------|-------|
| OS | Windows 10/11 (64-bit) | Ubuntu 24.04 LTS |
| Python | 3.10+ (없으면 인스톨러가 자동 설치) | 3.12+ |
| 인터넷 | 첫 설치 시 필수 (lerobot/torch 1~2GB 다운로드) | 동일 |
| 디스크 | ~5GB | ~5GB |

## 무결성 검증

### Windows (PowerShell)

```powershell
Get-FileHash roboseasy-studio-setup_v0.5.1_v0.0.1_win64.exe -Algorithm SHA256
```

### Linux

```bash
sha256sum -c roboseasy-studio_0.5.1-0.0.1_amd64.deb.sha256
```

### 체크섬

- `.deb` SHA256: `2792d69ae5d6d710bb0f6b83140aa2f7bb01fe6562cb7904cc43f8f9e33fd134`
- `.exe` SHA256: `1b54d0606e6760295419005bdb4861ac8c6dedd097d07fdf9ef9593dce4afa4e`
