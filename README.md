# 🎮 Minecraft NeoForge 1.21.1 모드팩

이 모드팩은 **NeoForge 1.21.1** 기반의 서바이벌 + PvE 중심 모드팩입니다.

## 📋 서버 정보

- **서버 주소**: `dshs-omc.duckdns.org:38472`
- **보이스챗 포트**: `24454`
- **마인크래프트 버전**: 1.21.1
- **모드로더**: NeoForge 21.1.209

## 🚀 클라이언트 설치 방법

### 방법 1: Prism Launcher (권장)

1. **Prism Launcher 다운로드 및 설치**
   - [Prism Launcher 공식 사이트](https://prismlauncher.org/)에서 다운로드

2. **새 인스턴스 생성**
   - `Add Instance` 클릭
   - 버전: `1.21.1` 선택
   - Mod Loader: `NeoForge` 선택 (버전: 21.1.209)

3. **Packwiz 설치**
   - 생성한 인스턴스를 우클릭 → `Edit` 선택
   - 왼쪽 메뉴에서 `Settings` 클릭
   - `Custom commands` 체크
   - `Pre-launch command`에 다음 입력:
     ```
     "$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/CheshireOverLap/minecraft-modpack/main/pack.toml
     ```

4. **Packwiz 부트스트랩 다운로드**
   - [Packwiz Installer Bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap/releases) 다운로드
   - `packwiz-installer-bootstrap.jar` 파일을 인스턴스 폴더에 저장
   - (인스턴스 폴더 경로: 인스턴스 우클릭 → `Folder` → `Minecraft` 선택)

5. **게임 실행**
   - 인스턴스를 실행하면 자동으로 모든 모드가 다운로드됩니다
   - 첫 실행 시 모드 다운로드에 시간이 걸릴 수 있습니다

### 방법 2: MultiMC

MultiMC도 Prism Launcher와 동일한 방식으로 설정할 수 있습니다.

### 방법 3: 수동 설치

1. **NeoForge 1.21.1 설치**
   - [NeoForge 공식 사이트](https://neoforged.net/)에서 버전 21.1.209 다운로드 및 설치

2. **Packwiz Installer 다운로드**
   - [Packwiz Installer Bootstrap](https://github.com/packwiz/packwiz-installer-bootstrap/releases) 다운로드

3. **모드 다운로드**
   - 터미널/명령 프롬프트에서 `.minecraft` 폴더로 이동
   - 다음 명령어 실행:
     ```bash
     java -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/CheshireOverLap/minecraft-modpack/main/pack.toml
     ```

4. **셰이더팩 & 리소스팩 복사 (선택사항)**
   - `shaderpacks` 폴더의 셰이더를 `.minecraft/shaderpacks/`에 복사
   - `resourcepacks` 폴더의 리소스팩을 `.minecraft/resourcepacks/`에 복사

## 📦 포함된 모드 (32개)

### ⚔️ 콘텐츠 & 보스
- **L_Ender's Cataclysm** - 고난이도 보스 및 던전 추가

### 🛠️ 유틸리티 & API
- Architectury API
- Cloth Config API
- Curios API
- YUNG's API
- Lionfish API
- Placebo

### ⚡ 성능 최적화
- **Embeddium** - 렌더링 최적화 (Sodium 포크)
- **FerriteCore** - 메모리 사용량 감소
- **ModernFix** - 로딩 속도 및 성능 개선
- **FastSuite** - 레시피 최적화
- **Entity Culling** - 보이지 않는 엔티티 렌더링 제거
- **More Culling** - 추가 컬링 최적화
- **AllTheLeaks** - 메모리 누수 수정

### 🎨 그래픽 & 비주얼
- **NeOculus** - 셰이더 지원 (Oculus 포크)
- **Continuity** - 연결된 텍스처 지원
- **Entity Texture Features** - 엔티티 텍스처 커스터마이징
- **Yes Steve Model** - 플레이어 모델 개선
- **Complementary Reimagined 셰이더** (포함)
- **Stoneborn 리소스팩** (포함)

### 🗺️ UI & 편의성
- **JEI** (Just Enough Items) - 아이템/레시피 검색
- **Xaero's Minimap** - 미니맵
- **Xaero's World Map** - 월드맵
- **AppleSkin** - 음식 정보 표시
- **Clumps** - 경험치 오브 최적화
- **Inventory Profiles Next** - 인벤토리 정리
- **libIPN** - IPN 라이브러리

### 💀 사망 시스템
- **You're in Grave Danger** - 사망 시 무덤 생성

### 🗣️ 커뮤니케이션
- **Simple Voice Chat** - 근거리 음성 채팅

### 🔧 월드 편집
- **WorldEdit** - 월드 편집 도구

### 🔌 호환성
- **Sinytra Connector** - Fabric 모드 지원
- **Forgified Fabric API** - Fabric API 호환
- **Kotlin for Forge** - Kotlin 언어 지원
- **Euphoria Patches** - Optifine 리소스팩 지원

## 🎮 게임 플레이 팁

### 셰이더 설정
1. 게임 실행 후 `옵션` → `비디오 설정` → `셰이더팩`
2. `ComplementaryReimagined_r5.5.1.zip` 선택
3. 성능이 낮다면 셰이더 설정에서 품질 조정

### 보이스챗 사용
- `V` 키를 눌러 음성 채팅 활성화
- 근거리에 있는 플레이어와 대화 가능

### JEI 사용법
- 아이템 검색: 검색창에 아이템 이름 입력
- 레시피 확인: `R` 키
- 사용처 확인: `U` 키

## 🔄 모드 업데이트

모드팩이 업데이트되면 Prism Launcher를 실행할 때 자동으로 감지되고 업데이트됩니다.

수동 설치의 경우:
```bash
java -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/CheshireOverLap/minecraft-modpack/main/pack.toml
```

## ❓ 문제 해결

### 모드가 다운로드되지 않을 때
1. 인터넷 연결 확인
2. Packwiz 명령어 재실행
3. `.minecraft/packwiz.json` 파일 삭제 후 재시도

### 게임이 크래시될 때
1. Java 버전 확인 (Java 21 이상 권장)
2. 할당 메모리 증가 (최소 4GB, 권장 6-8GB)
3. 그래픽 드라이버 업데이트

### 셰이더가 작동하지 않을 때
1. NeOculus 모드가 설치되어 있는지 확인
2. 셰이더팩이 `shaderpacks` 폴더에 있는지 확인
3. 성능 문제 시 셰이더를 끄거나 다른 셰이더 사용

## 📞 문의

- **서버 관리자**: CheshireOverLap
- **GitHub**: https://github.com/CheshireOverLap/minecraft-modpack

## 📜 라이선스

이 모드팩에 포함된 모든 모드는 각 모드 제작자의 라이선스를 따릅니다.
