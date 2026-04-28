# ☁️ KOSA-Team1-Gooroomees Organization

우리 팀의 효율적인 협업과 안정적인 코드 관리를 위한 공통 가이드라인입니다. 모든 팀원은 아래 규칙을 준수하여 프로젝트를 진행해 주세요.

---

## 🌳 Branch Strategy: main - develop - feature
짧은 기간 내 효율적인 관리를 위해 **GitHub-flow** 기반의 간소화된 전략을 사용합니다.

- **`main`**: 최종 배포용 브랜치. 언제든 즉시 서비스 가능한 상태를 유지합니다.
- **`develop`**: 개발 통합 브랜치. 모든 `feature` 작업이 모이는 기준점입니다.
- **`feature`**: 기능 구현 브랜치. `develop`에서 분기하며, 작업 완료 후 `develop`으로 PR을 보냅니다.
  - **네이밍 규칙**: `[Prefix]/#이슈번호` (예: `feat/#1`, `fix/#5`)

### 🔄 Workflow
1. `develop` 브랜치에서 본인의 작업 브랜치(`feat/#번호`)를 생성합니다.
2. 기능 구현 후 원격 저장소에 Push합니다.
3. **develop** 브랜치를 대상으로 **PR**을 생성합니다.
4. 리뷰 및 승인 절차를 거쳐 `develop`에 병합합니다.
5. 검증된 `develop` 코드는 마일스톤에 맞춰 `main`으로 최종 병합됩니다.

---

## 📝 Commit Convention
모든 커밋 메시지는 아래 양식을 엄격히 준수합니다.

### 1. 양식 및 예시
- **양식**: `[Prefix]#(이슈번호) - (해당 작업에 대한 내용)`
- **예시**: `Feature#1 - 사용자 로그인 API 구현`

### 2. 접두어(Prefix) 종류
| Prefix | 내용 |
| :--- | :--- |
| **Feature** | 새로운 기능 구현 |
| **Fix** | 버그 해결, 오류 수정 및 코드 보정 |
| **Design** | UI 레이아웃 조정 및 디자인 요소 변경 |
| **Merge** | 브랜치 병합 및 충돌 해결 |
| **Refactor** | 코드 구조 개선 (기능 변화 없음) |
| **Docs** | 문서 추가 및 개정 (README, WIKI 등) |
| **Chore** | 빌드/패키지 설정 등 프로덕션 코드 외 작업 |
| **Setting** | 프로젝트 초기 세팅 및 환경 구축 |
| **Rename** | 파일/폴더명 수정 또는 위치 이동 |
| **Remove** | 파일 삭제 작업만 수행하는 경우 |
| **Comment** | 주석 추가 및 변경 |

---

## 🛠 Organization Tools
- **Issue/PR Templates**: 새 이슈 및 PR 생성 시 자동으로 양식이 적용됩니다.
- **Repository Rulesets**: `main`, `develop` 브랜치에 대한 직접 Push가 제한되며, PR 승인이 권장됩니다.

---
*문의사항은 팀 내 Git Manager(@tls427wodnr)에게 문의해 주세요.*
