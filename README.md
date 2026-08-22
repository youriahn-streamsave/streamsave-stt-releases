# StreamSaveSTT

Free desktop app for StreamSave subscribers — generate and translate subtitles from local audio/video files on your own PC (Windows, macOS, Linux). Nothing is uploaded; transcription runs entirely on-device with whisper.cpp.

**This repository hosts installers only.** Source code lives in a separate private repository — this repo exists purely so downloads can be public while the code stays closed.

## Download

| OS | File | Link |
|---|---|---|
| Windows 10/11 (x64) | `StreamSaveSTT.exe` | [Download](https://github.com/youriahn-streamsave/streamsave-stt-releases/releases/latest/download/StreamSaveSTT.exe) |
| macOS (Intel, Apple Silicon via Rosetta 2) | `StreamSaveSTT.dmg` | [Download](https://github.com/youriahn-streamsave/streamsave-stt-releases/releases/latest/download/StreamSaveSTT.dmg) |
| Linux (x64, AppImage) | `StreamSaveSTT.AppImage` | [Download](https://github.com/youriahn-streamsave/streamsave-stt-releases/releases/latest/download/StreamSaveSTT.AppImage) |

These links always point to the latest release. See the [Releases page](https://github.com/youriahn-streamsave/streamsave-stt-releases/releases) for version history and release notes.

## First-run instructions

The app is not code-signed yet (v0.1), so each OS shows an unfamiliar-publisher warning the first time you run it. This is expected — the steps below are safe.

### Windows
1. Run the downloaded `.exe`. Windows SmartScreen will show a blue "Windows protected your PC" screen.
2. Click **More info**, then **Run anyway**.
3. Follow the installer normally.

### macOS
Because the app isn't notarized, right-click → Open may not reliably work on recent macOS versions (Sequoia and later) — use System Settings instead:
1. Open the downloaded `.dmg` and drag StreamSaveSTT into Applications.
2. Try opening the app. macOS will block it ("Apple could not verify...").
3. Go to **System Settings → Privacy & Security**, scroll down, and click **Open Anyway** next to the StreamSaveSTT warning.
4. Confirm with your password/Touch ID. The app will open normally after this one-time approval.

### Linux (AppImage)
```bash
chmod +x StreamSaveSTT.AppImage
./StreamSaveSTT.AppImage
```
No installation needed — it's a self-contained executable.

## What it does

- Local speech-to-text (Whisper models, downloaded on first use and cached)
- Subtitle translation (`.srt`/`.vtt`)
- A built-in benchmark recommends the best model for your machine's speed/accuracy tradeoff
- Requires an active StreamSave subscription license to run transcription jobs

## Support

Questions or issues: `support@streamsave.youriahn.com`

---

## 한국어 안내

StreamSave 구독자 전용 무료 데스크톱 앱 — 로컬 PC에서 오디오/비디오 파일의 자막을 생성하고
번역합니다(Windows/macOS/Linux). 어디에도 업로드되지 않고 whisper.cpp로 전부 기기 안에서
처리됩니다.

**이 저장소는 설치파일만 배포합니다.** 소스코드는 별도의 비공개 저장소에 있고, 이 저장소는
다운로드만 공개하기 위해 따로 만들어졌습니다.

### 다운로드
위 표의 링크는 항상 최신 버전을 가리킵니다. 버전별 변경 내역은 [Releases 페이지](https://github.com/youriahn-streamsave/streamsave-stt-releases/releases)에서 확인하세요.

### 최초 실행 안내
아직 코드서명이 안 된 상태(v0.1)라 처음 실행할 때 각 OS가 "알 수 없는 게시자" 경고를
띄웁니다 — 정상적인 현상입니다.

- **Windows**: SmartScreen 경고가 뜨면 **추가 정보 → 실행**을 클릭하세요.
- **macOS**: 최신 macOS(Sequoia 이후)는 우클릭 열기가 안 먹힐 수 있어 **시스템 설정 → 개인정보
  보호 및 보안**에서 스크롤을 내려 StreamSaveSTT 항목 옆 **열기**를 눌러 승인하세요.
- **Linux**: `chmod +x StreamSaveSTT.AppImage` 후 바로 실행하면 됩니다(설치 불필요).

### 문의
`support@streamsave.youriahn.com`
