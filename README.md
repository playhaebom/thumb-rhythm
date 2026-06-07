# 🎵 손가락 DDR 리듬게임 (Finger Rhythm DDR)

보컬 주파수 대역을 실시간으로 추적·분석하여 나만의 음악으로 노트를 동적 생성하는 웹 기반 4키(4-Key) 리듬게임입니다. HTML5 Canvas와 Web Audio API를 활용하여 모바일과 PC 환경 모두에서 끊김 없는 고성능 플레이를 제공합니다.

👉 **[라이브 데모 플레이하기](https://your-github-username.github.io/your-repository-name/)** *(주의: 본인의 깃허브 페이지 주소에 맞게 위 링크를 수정해 주세요!)*

---

## ✨ 주요 특징 (Key Features)

* **보컬 추출 및 동적 노트 생성**: 오디오 파일 디코딩 후 하이패스(300Hz) 및 로우패스(3400Hz) 필터를 거쳐 드럼 킥이나 고음역 노이즈를 제거하고, 오직 목소리(바이브레이션, 음절)에만 반응하는 일반 노트 및 롱노트를 실시간으로 빌드합니다.
* **정밀한 멀티 터치 시스템**: 모바일 멀티 터치 환경에서 각 터치 포인트의 고유 식별자(`touch.identifier`)를 트래킹하여, 손가락을 뗄 때 판정이 꼬이거나 롱노트가 끊기는 버그를 완벽하게 방지했습니다.
* **시각적 이펙트 & HUD**: 오디오 파형(Waveform) 시각화 프로그레스 바, 리얼타임 레이트(`RATE%`) 및 콤보 스코어링 시스템, 스포트라이트 빔 효과와 은하수 배경 파티클 연출이 포함되어 있습니다.
* **난이도 세팅**: 플레이어의 숙련도에 따라 판정 범위(Hit Window)와 노트 하강 속도가 유연하게 조절되는 `EASY` / `HARD` 모드를 지원합니다.

---

## 🎮 조작 방법 (Controls)

### 💻 PC 환경 (Keyboard)
화면 왼쪽 레인부터 순서대로 아래의 키보드를 입력하세요.
* **1번 레인 (Pink)**: `D`
* **2번 레인 (Mint)**: `F`
* **3번 레인 (Blue)**: `J`
* **4번 레인 (Orange)**: `K`

### 📱 모바일 환경 (Mobile Touch)
* 화면 하단의 각 레인 영역을 손가락으로 직접 터치하세요.
* 다중 터치를 지원하므로 동시치기 및 롱노트 유지가 부드럽게 가능합니다.

---

## 🚀 플레이 방법 (How to Play)

1. **난이도 선택**: 메인 화면에서 `EASY` 또는 `HARD` 모드를 선택합니다.
2. **음원 업로드**: `MP3 파일 선택` 버튼을 눌러 소지하고 계신 오디오 파일(`.mp3`, `.wav` 등)을 업로드합니다.
3. **분석 및 대기**: 시스템이 보컬을 추출하고 오디오 파형을 그리는 동안 잠시 기다립니다. (완료 시 게임이 자동 시작됩니다.)
4. **연주 및 탈출**: 리듬에 맞춰 떨어지는 노트를 타이밍에 맞게 타격하세요. 플레이 중 언제든 `EMERGENCY EXIT` 버튼으로 중단할 수 있습니다.

---

## 🛠️ 기술 스택 (Tech Stack)

* **Frontend**: HTML5, CSS3 (Neon Cyberpunk Theme, Orbitron Typography)
* **Graphics**: HTML5 Canvas 2D Context API
* **Audio Engine**: Web Audio API (`AudioContext`, `OfflineAudioContext`, `BiquadFilterNode`)
* **Deployment**: GitHub Pages

---

## 📝 라이선스 (License)

Copyright © 해봄에듀 All Rights Reserved.  
본 프로젝트의 콘텐츠 및 소스코드는 교육용 및 개인 연구용으로 자유롭게 활용할 수 있습니다.
