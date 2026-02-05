# Heemo Web App 🌸

Couple Healing & Date Course Service Frontend
자주 다투는 연인을 위한 화해 솔루션 및 스마트 데이트 코스 추천 서비스

**Next.js · TypeScript · Tailwind CSS · pnpm · FSD (Feature-Sliced Design)**
**PWA (Planned) · Playwright (Planned) · Vitest (Planned)**

---

## 📖 Project Overview

**Heemo(희모)**는 연인 간의 건강한 관계 회복과 즐거운 데이트 경험을 돕기 위해 설계된 웹 애플리케이션의 **프론트엔드**입니다.
단순한 화면 구현을 넘어, **사용자 감정 흐름(갈등 → 중재 → 회복)**을 자연스럽게 이어주는 UX를 목표로 합니다.

본 프로젝트는 **확장성과 유지보수성**을 우선으로 고려하여 **Feature-Sliced Design(FSD)** 아키텍처를 기반으로 구성되었으며,
도메인/기능 단위로 UI, 상태, 비즈니스 로직을 분리하여 장기적으로 안정적인 개발을 지향합니다.

---

## 🚀 Key Features

### Relationship Recovery (Healing)

* 갈등 상황 입력 기반의 중재 플로우 UI
* 감정 분석 결과 요약 및 회복 액션 가이드 화면 (Planned)
* ‘백기(White Flag)’ 알림 수신 및 상태 반영 UI (Planned)

### Smart Date Planner

* 위치 기반 데이트 코스 탐색 UI (Planned)
* 코스 동선/시간 구성 화면 (Planned)
* 코스 저장 및 공유 기능 (Planned)

### Couple Todo (Shared)

* 커플 공유 투두리스트 UI (Planned)
* 실시간 반영(동기화) UX (Planned)

### Gamification

* 활동 기여도(Relationship Point) 기반 캐릭터 성장 UI (Planned)
* 미션/보상 획득 및 히스토리 화면 (Planned)

---

## 🛠 Tech Stack & Decision Making

### Frontend

* **Framework**: Next.js (App Router)

  * 라우팅/레이아웃 구조화를 단순화하고, 확장 가능한 페이지 구성을 위해 선택
* **Language**: TypeScript

  * 안정적인 타입 기반 개발 및 유지보수성 강화
* **Styling**: Tailwind CSS

  * 빠른 UI 구현과 일관된 스타일 시스템 운영을 위해 선택
* **Architecture**: Feature-Sliced Design (FSD)

  * 기능/도메인 단위로 책임을 분리해 확장성과 재사용성 강화
* **Package Manager**: pnpm

  * 빠른 설치 속도 및 의존성 관리 효율성(특히 확장 시)을 위해 선택
* **Bundler**: Turbopack (Next dev)

  * 개발 경험(속도) 개선

### State & Data (Planned)

* **Server State**: React Query
* **Client State**: Zustand

### Testing (Planned)

* **Unit/Integration**: Vitest + Testing Library
* **E2E**: Playwright

---

## 🏗 Architecture (Feature-Sliced Design)

본 프로젝트는 **FSD** 구조를 따르며,
UI 조합 단위(Widgets) → 기능(Features) → 도메인(Entities) → 공통(Shared) 레이어로 책임을 분리합니다.

```
src/
├── app/        // Next.js 라우팅, Layout, Provider, 전역 설정
├── pages/      // 페이지 단위 구성(여러 widgets/features 조합)
├── widgets/    // 독립 UI 블록(페이지 구성 요소)
├── features/   // 사용자 행동 단위 기능(예: 로그인, 검색, 필터링)
├── entities/   // 도메인 모델(예: couple, datecourse, healing)
└── shared/     // 공통 UI/유틸/디자인 토큰/hooks/api 클라이언트
```

---

## ⚙️ Getting Started

### Prerequisites

* Node.js 22.x (권장)
* pnpm

### Install

```bash
pnpm install
```

### Run (Development)

```bash
pnpm dev
```

App: [http://localhost:3000](http://localhost:3000)

### Build

```bash
pnpm build
```

### Start (Production)

```bash
pnpm start
```

---

## 🌐 Environment Variables

`.env.local` 파일을 생성하여 환경 변수를 설정합니다.

```env
NEXT_PUBLIC_API_URL=
```

---

## 📱 PWA (Planned)

서비스 확장을 고려하여 **Progressive Web App** 환경을 지원할 예정입니다.

* Web App Manifest 구성
* Service Worker 적용
* 오프라인 캐싱 전략 (Planned)

---

## 🧪 Testing (Planned)

* UI/도메인 로직 단위 테스트(Vitest)
* 핵심 사용자 시나리오 E2E 테스트(Playwright)

---

## 📏 Code Convention

### Commit Message Convention

```
feat: 기능 추가
fix: 버그 수정
refactor: 리팩토링
style: UI 변경
chore: 설정/환경 변경
docs: 문서 수정
```

### Naming Convention

* Folder: `kebab-case`
* Component: `PascalCase`

---

## 📦 Future Improvements

* 상태 관리 구조 고도화 (React Query + Zustand)
* 디자인 시스템/토큰 정리
* PWA 기능 확장
* 테스트 커버리지 확장 (unit + e2e)
