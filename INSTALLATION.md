# 📦 OMC 모드팩 설치 가이드

이 가이드는 친구들이 쉽게 모드팩을 설치할 수 있도록 단계별로 설명합니다.

## 🎯 시작하기 전에

### 필수 요구사항 체크리스트

- [ ] **Minecraft Java Edition** 정품 계정
- [ ] **Java 21** 이상 설치
- [ ] 최소 **8GB RAM** (6GB 이상 할당)
- [ ] 약 **3GB** 여유 저장공간

## 🚀 방법 1: Prism Launcher (가장 쉬움, 추천!)

### 1단계: Prism Launcher 다운로드

1. [Prism Launcher 공식 사이트](https://prismlauncher.org/) 접속
2. 자신의 운영체제에 맞는 버전 다운로드
   - Windows: `.exe` 파일
   - Mac: `.dmg` 파일
   - Linux: AppImage 또는 패키지
3. 설치 및 실행

### 2단계: Java 설정

1. Prism Launcher 실행
2. 상단 메뉴 **Settings** 클릭
3. **Java** 탭 선택
4. **Auto-detect** 버튼 클릭하여 Java 21 선택
5. **Maximum memory allocation** 을 **6144 MB** 이상으로 설정

### 3단계: 모드팩 설치

1. [Releases 페이지](../../releases/latest)에서 최신 `.mrpack` 파일 다운로드
   - 파일명: `OMC-Modpack-vX.X.X-Client.mrpack`
2. Prism Launcher 창에 `.mrpack` 파일을 **드래그 & 드롭**
3. 인스턴스 이름 확인 후 **OK** 클릭
4. 자동으로 모든 모드와 설정 다운로드 (2~5분 소요)

### 4단계: 게임 실행

1. 설치된 인스턴스를 더블클릭
2. Minecraft 로그인
3. 메인 메뉴가 뜨면 설치 완료! ✅

---

## 🎮 방법 2: Modrinth App

### 1단계: Modrinth App 설치

1. [Modrinth App](https://modrinth.com/app) 다운로드
2. 설치 및 실행
3. Minecraft 계정 로그인

### 2단계: 모드팩 추가

1. 좌측 메뉴에서 **Browse** 클릭
2. 우측 상단 **Import** 버튼 클릭
3. 다운로드한 `.mrpack` 파일 선택
4. **Create** 클릭

### 3단계: 메모리 설정

1. 생성된 프로필 우클릭
2. **Edit** → **Settings**
3. **Java memory** 를 **6GB** 이상으로 설정
4. **Save** 클릭

### 4단계: 플레이

1. 프로필 선택
2. **Play** 버튼 클릭

---

## 🔧 방법 3: 수동 설치 (고급)

### 1단계: NeoForge 설치

1. [NeoForge 다운로드 페이지](https://neoforged.net/) 접속
2. **1.21.1** 버전 선택
3. **21.1.209** Installer 다운로드
4. `.jar` 파일 실행
5. **Install client** 선택 후 **OK**

### 2단계: 모드 다운로드

**옵션 A: PackWiz로 설치 (자동)**
```bash
# packwiz 설치 필요
packwiz refresh
```

**옵션 B: 수동 다운로드**
1. `.mrpack` 파일을 `.zip`으로 확장자 변경
2. 압축 해제
3. `overrides` 폴더 내용을 `.minecraft` 폴더에 복사

### 3단계: 프로필 설정

1. Minecraft Launcher 실행
2. **Installations** → **New installation**
3. Name: `OMC Modpack`
4. Version: `neoforge-21.1.209`
5. **More Options** → JVM Arguments 수정:
   ```
   -Xmx6G -Xms6G
   ```
6. **Create** 클릭

### 4단계: 실행

1. 프로필 선택 후 **Play**

---

## 🌐 서버 접속하기

### 서버 정보
```
서버 이름: OMC 서버
서버 주소: dshs-omc.duckdns.org:38472
버전: 1.21.1 NeoForge 21.1.209
```

### 접속 방법

1. 게임 실행 후 **Multiplayer** 클릭
2. **Add Server** 클릭
3. 서버 정보 입력:
   - Server Name: `OMC 서버`
   - Server Address: `dshs-omc.duckdns.org:38472`
4. **Done** 클릭
5. 서버 선택 후 **Join Server**

---

## ❓ 자주 묻는 질문 (FAQ)

### Q1. Java 21을 어디서 다운로드하나요?
**A:** [Adoptium](https://adoptium.net/)에서 Eclipse Temurin 21을 다운로드하세요.

### Q2. 게임이 크래시되어요
**A:** 다음을 확인하세요:
1. Java 버전이 21 이상인지
2. RAM 할당이 6GB 이상인지
3. 그래픽 드라이버가 최신인지
4. `.mrpack` 파일을 정확히 사용했는지

### Q3. "Incompatible mod set!" 오류가 나요
**A:** 서버와 클라이언트의 모드팩 버전이 일치하지 않습니다. 최신 버전을 다시 다운로드하세요.

### Q4. FPS가 너무 낮아요
**A:** 
1. 비디오 설정에서 렌더 거리를 줄이세요 (10 청크 권장)
2. 그래픽 품질을 낮추세요
3. Embeddium 설정에서 성능 모드를 활성화하세요

### Q5. 음성 채팅이 안 들려요
**A:**
1. 게임 내에서 `V` 키를 눌러 음성 설정을 여세요
2. 마이크와 스피커 설정을 확인하세요
3. `M` 키로 음소거 상태를 확인하세요

### Q6. 임의로 모드를 추가해도 되나요?
**A:** ❌ 권장하지 않습니다. 서버와의 호환성 문제가 발생할 수 있습니다.

### Q7. Mac에서 설치할 수 있나요?
**A:** ✅ 네! Prism Launcher 또는 Modrinth App을 사용하면 Mac에서도 동일하게 설치 가능합니다.

---

## 🆘 문제 해결

### 로그 파일 찾기

문제가 발생하면 로그 파일을 확인하세요:

**Prism Launcher:**
1. 인스턴스 우클릭
2. **Edit Instance** → **Other Logs**
3. `latest.log` 확인

**일반 런처:**
- Windows: `%appdata%\.minecraft\logs\latest.log`
- Mac: `~/Library/Application Support/minecraft/logs/latest.log`
- Linux: `~/.minecraft/logs/latest.log`

### 흔한 오류 해결

#### "Java 17 required" 오류
→ Java 21을 설치하고 런처 설정에서 Java 경로를 변경하세요.

#### "Out of memory" 오류
→ 런처 설정에서 RAM 할당을 늘리세요 (최소 6GB).

#### 모드 로딩 실패
→ `.minecraft/mods` 폴더를 삭제하고 모드팩을 재설치하세요.

---

## 📞 도움 요청

그래도 문제가 해결되지 않나요?

1. [GitHub Issues](../../issues)에 문제를 등록하세요
2. 디스코드 서버에 문의하세요
3. 로그 파일을 함께 첨부해주세요

---

**설치 과정에서 문제가 있으면 언제든 물어보세요!** 😊