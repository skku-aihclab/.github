# AI-Healthcare Lab GitHub Onboarding README

## 0) TL;DR (필수 체크리스트)

* [ ] 개인 GitHub 계정 생성 및 **2FA(2단계 인증) 활성화**
* [ ] `skku-aihclab` Organization 초대 수락
* [ ] **실명 프로필**(학번/학위 단계 표기 권장), 연구 분야/관심 태그 입력
* [ ] 연구 과제별 저장소 접근 권한 요청

---

## 1) 조직(Organization) 개요

* 명칭: **skku-aihclab** (연구실 공식 GitHub 조직)
* 관리(Owner): PI 및 지정 관리자 계정
* 기본 목적: 코드/문서/실험 관리, 연구 산출물 공개/비공개 운영
* 플랜: Education 혜택 적용 시 private repo 무제한 사용 가능

> ⚠️ Organization은 로그인 계정이 아닙니다. 개인 계정으로 로그인 후 조직을 이용합니다.

---

## 2) 보안 및 계정 정책

* 액세스 토큰: 필요 최소 범위(scope)로 발급, 노출 금지
* 팀 권한: Maintainer/Developer/Reader 등 최소권한 원칙(least privilege)
* 탈퇴·졸업 시: Owner/Maintainer에 통보 → 권한 회수 → 필요한 저장소 이관

---

## 3) 저장소(Repository) 운영 표준

### 3.1 네이밍 규칙(예시)

* 연구: `proj<year>-<topic>-<short/detailed topic>` → 예) `proj25-samsung-exercise_classification`
* 데이터: `data<year>-<source>-<privacy>` → 예) `data25-samsung_1st-internal`
* 패키지/라이브러리: `lib-<name>`
* 문서/강의: `docs-<course>-<year>`

### 3.2 가시성 & 권한

* 기본 비공개(private), 공개 필요 시 Owner 승인
* **Repository deletion/transfer**: 기본 **Owner만 허용(권장)**
* **Private forking**: 기본 **비활성화(권장)**. 필요 시 이슈로 요청
* GitHub Pages: 외부 공개용은 Public, 내부용은 Education Team 적용 후 Private 사용

### 3.3 Jupyter Notebook 규칙

* 업로드 전 반드시 **커널을 Restart & Run All** 하여 셀 번호가 1부터 끝까지 순서대로 이어지도록 할 것.
* 실행 결과(plots, metrics, logs)는 그대로 남겨두어 재현성 보장.
* 불필요한 셀(디버깅용 출력, 임시 코드)은 정리 후 업로드.
* 데이터/결과물은 직접 업로드하지 말고 외부 스토리지 링크로 연결. 사용한 데이터에 대해서는 반드시 README나 별도 문서에 설명을 포함할 것(데이터 출처, 다운로드 방법, 접근 권한, 저장 위치 등).

---

## 4) 개발 환경

* Python: `conda`/`mamba` 환경 권장, `environment.yml` 제공
* CUDA/TensorFlow/PyTorch 버전 호환 표기(README에 명시)



