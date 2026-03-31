![GitHub Release](https://img.shields.io/github/v/release/RuruBros/RuruGrab-Releases)

# RuruGrab

### 🛠️ 기능 설명
* **긁어오기**
  * **다운로드**: Youtube, Instagram, Twitter(X), sukebei 및 (Telegram)
  * **텍스트**: 사이트에서 텍스트를 markdown으로 추출 및 뷰어
  * **메타데이터**: 미디어 메타데이터 관리
 
* **도구**
  * **파일관리**: 파일정리, 자동 이름변경, 중복 파일 찾기의 기능을 제공합니다
  * **원 스페이스**: 외장 디스크 등 흩어져 있는 파일을 인덱싱해서 하나처럼 보여줍니다
  * **채팅**: XMPP 채팅, 회원 가입은 각종 XMPP 서버를 이용해 주세요
  * **볼트**: 마스터 비밀번호로 보호되는 로컬 전용 암호화 노트 저장소입니다
  * **QR**: 다양한 형태의 QR 코드를 생성합니다

* **Telegram Bot**을 이용한 AI봇
  * Telegram Bot을 따로 생성하고 각종 설정을 한 뒤, telegram에서 rurugrab 앱에게 각종 작업을 맡길 수 있습니다.

### 📌 필수 요구사항
* 현재 베타 릴리스(2026년 4월 기준)는 **Windows 11 x64**에서만 지원됩니다.
* 기타 운영 체제는 향후 지원 예정입니다.

### 🚀 설치 방법 (Installation)

1. **데스크톱 앱 설치**
   * [Releases] 탭에서 최신 설치 파일(`.exe` 또는 `.msi`)을 다운로드(**Download**)합니다.

2. **브라우저 확장 프로그램(Extension) 수동 설치**
   * 브라우저 주소창에 `chrome://extensions/` 또는 `edge://extensions/` 입력 후 접속합니다.
   * **개발자 모드(Developer mode)**를 활성화합니다.
   * **압축해제된 확장 프로그램 로드(Load unpacked)** 버튼을 클릭합니다.
   * RuruGrab이 설치된 경로 내의 `extension` 폴더를 선택합니다. 
     *(경로 예시: `C:\Users\<사용자명>\AppData\Local\RuruGrab`)*

### 🎮 주요 기능 및 사용법 (How to Use)

* **미디어 저장 (Grab)**
  * 앱을 실행한 상태에서 X(Twitter), YouTube, Instagram의 이미지나 영상을 우클릭합니다.
  * **RuruGrab -> Grab** 메뉴를 선택하여 저장합니다.
  * 앱 창을 닫아도 **시스템 트레이(System Tray)**에서 백그라운드로 계속 실행됩니다.

* **Telegram** 다운로드 제한 컨텐츠
  * Extension이 설치된 상태에서, Telegram Web의 영상을 플레이하면 다운로드 버튼이 상단에 노출 됩니다.

* **메타데이터(Metadata) 설정**
  1. `시스템 > 설정 > 기능제어`에서 **메타데이터** 를 **ON** 합니다.
  2. `시스템 > 연동 > 프로바이더`에서 필요한 프로바이더를 활성화합니다.
  3. `긁어오기 > 메타데이터` 에서 검색, 로컬에 저장된 데이터가 없을 경우 **"Let the cat scout"** 버튼을 클릭하면 2번에서 활성화한 프로바이더들을 통해서 데이터를 수집하여 자동 저장합니다.

* **버그 리포트:** 버그나 기능 요청은 [GitHub Issues](https://github.com/RuruBros/RuruGrab-Releases/issues)에 보고해주세요.
