# Photo Organizer — macOS

[Windows · English](../README.md) | [Windows · 한국어](README_KR.md) | [macOS · English](README_mac.md) | **macOS · 한국어**

Photo Organizer는 필름 사진과 디지털 사진을 정리하고, 메타데이터·파일 시간 관리, LUT 적용, 폴더 분류 및 각종 도구 기능을 제공하는 데스크톱 프로그램입니다.

> 현재 macOS 빌드: **v2.0.0**  
> 아키텍처: **Apple Silicon (arm64)**

---

## 주요 기능

### 필름 사진
- 버튼 또는 마우스 드래그로 사진 순서 변경
- 연속 촬영시간 / 정확한 촬영시간 적용
- EXIF `DateTimeOriginal` 기록
- 카메라 / 렌즈 / 필름 메타데이터 지원
- 고정렌즈 카메라 보조 데이터베이스
- 메타데이터 일괄 적용

### 디지털 사진
- `.cube` LUT 적용
- LUT 강도 조절
- 원본 / 적용 결과 미리보기
- 이전 / 다음 사진 이동
- 같은 위치에 `*_LUT` 폴더로 저장
- 다른 이름으로 저장
- JPEG / PNG / TIFF 출력 지원
- LUT 라이브러리: `Documents/Photo Organizer/LUTs`

### 폴더 분류
- 파일을 폴더별로 정리
- 관련 RAW 파일 매칭 지원
- 파일명 충돌 방지 처리

### 파일 시간
- 파일의 날짜 및 시간 정보를 일괄 수정

### 도구
- SHA-256 기반 중복 파일 확인
- 초기화 / 프로그램 정보

### 지원 언어
- 한국어
- English
- 日本語
- 简体中文
- Français
- Español
- Deutsch
- Русский

---
### Gatekeeper 안내

현재 무료 macOS 빌드는 **ad-hoc 코드 서명**을 사용하며 Apple Developer ID 공증(notarization)은 적용하지 않았습니다.

따라서 처음 실행할 때 macOS가 앱 실행을 차단할 수 있습니다.

그 경우:

1. `Photo Organizer.app`을 한 번 실행합니다.
2. 차단 경고가 나타나면 창을 닫습니다.
3. `시스템 설정 → 개인정보 보호 및 보안`으로 이동합니다.
4. 화면 아래쪽의 보안 항목에서 `Photo Organizer`에 대해 **그래도 열기**를 선택합니다.
5. 다시 나타나는 확인창에서 **열기**를 선택합니다.

이 허용 과정은 일반적으로 **최초 1회만 필요**합니다.

같은 빌드의 동일한 `Photo Organizer.app`을 계속 사용하는 경우, 이후에는 일반 앱처럼 바로 실행할 수 있습니다.

다만 아래와 같은 경우에는 macOS가 다시 허용을 요구할 수 있습니다.

- 새 버전으로 업데이트한 경우
- 앱 파일 또는 코드 서명이 변경된 경우
- ZIP 파일을 다시 다운로드하여 새 앱으로 인식된 경우

---

## macOS 요구 사항

- **Apple Silicon Mac**
- 현재 arm64 빌드는 M1 / M2 / M3 / M4 계열용
- Intel Mac용 빌드는 현재 제공하지 않음

현재 macOS 빌드는 다음 구성요소를 사용합니다.

- Python 3.14.7
- Tcl/Tk 9.0.x
- CustomTkinter 6.0.0
- Pillow
- piexif
- tkinterdnd2
- SUIT 글꼴

---

## 설치 방법

macOS 배포본이 공개될 경우:

1. macOS arm64 ZIP 파일을 다운로드합니다.
2. ZIP 압축을 해제합니다.
3. `Photo Organizer.app`을 `응용 프로그램(Applications)` 폴더로 옮기는 것을 권장합니다.
4. 앱을 실행합니다.

### Gatekeeper 안내

현재 무료 macOS 빌드는 **ad-hoc 코드 서명**을 사용하며 Apple Developer ID 공증(notarization)은 적용하지 않았습니다.

따라서 처음 실행할 때 macOS가 앱 실행을 차단할 수 있습니다.

그 경우:

1. Finder에서 `Photo Organizer.app`을 Control-클릭 또는 우클릭합니다.
2. **열기**를 선택합니다.
3. 다시 **열기**를 선택합니다.

macOS 버전에 따라 다음 위치에서 허용해야 할 수도 있습니다.

`시스템 설정 → 개인정보 보호 및 보안`

---

## 코드 서명

macOS v2.0.0 arm64 빌드는 로컬에서 다음 명령으로 검증을 통과했습니다.

```bash
codesign --verify --deep --strict
```

즉, 앱 번들의 코드 서명 무결성은 정상입니다.

다만 Apple Developer ID 인증서로 서명하지 않았고 Apple 공증도 받지 않았기 때문에, 다른 Mac에서 다운로드한 앱을 처음 실행할 때 Gatekeeper 경고가 나타날 수 있습니다.

---

## 제3자 라이선스

- [macOS 제3자 라이선스](../THIRD_PARTY_LICENSES_mac.md)
- [SUIT Open Font License](../licenses/SUIT_OFL.txt)
- [Photo Organizer 라이선스](../LICENSE.txt)

---

## 라이선스

Photo Organizer는 독점 무료 소프트웨어(Proprietary Freeware)입니다.

개인적·비상업적 용도에서는 프로젝트 라이선스 조건에 따라 무료로 사용할 수 있습니다.

상업적 이용, 재배포, 상업 제품 또는 서비스에 포함하는 행위 등 라이선스에서 명시적으로 허용하지 않은 권리는 별도 허가가 필요합니다.

자세한 내용:

[LICENSE.txt](../LICENSE.txt)

---

## 저작권

Copyright © 2026 Arti3479. All rights reserved.
