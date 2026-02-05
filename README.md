# 🧩 heemo-web

---

# 📌 Overview

본 프로젝트는 **Feature-Sliced Design(FSD)** 아키텍처를 기반으로 구성되어
유지보수성과 확장성을 강화하였습니다.

---

# 🚀 Tech Stack

## Core

- Next.js (App Router)
- React
- TypeScript

## Styling

- Tailwind CSS

## State / Data

- React Query (예정)
- Zustand (예정)

## Package Manager

- pnpm

## Bundler

- Turbopack

## Architecture

- Feature-Sliced Design (FSD)

---

# 📱 Features

- 사용자 중심 UI/UX 설계
- 반응형 웹 지원
- PWA 지원 예정
- 확장 가능한 아키텍처 구조

---

# 🧱 Architecture - Feature Sliced Design

본 프로젝트는 **FSD 구조**를 기반으로 설계되었습니다.

```
src/
 ┣ app/
 ┣ pages/
 ┣ widgets/
 ┣ features/
 ┣ entities/
 ┣ shared/
```

---

## 📂 Layer 설명

### 🔹 app

- Next.js 라우팅 및 전역 설정
- 레이아웃, Provider, Routing 관리

---

### 🔹 pages

- 실제 페이지 단위 구성
- 여러 위젯과 기능 조합

---

### 🔹 widgets

- UI 블록 단위 구성
- 페이지를 구성하는 독립적인 영역

---

### 🔹 features

- 사용자 행동 단위 기능
- 예: 로그인, 검색, 필터링 등

---

### 🔹 entities

- 비즈니스 도메인 모델
- API 모델, 타입, 상태 로직 포함

---

### 🔹 shared

- 전역 공통 모듈
- UI 컴포넌트
- 유틸 함수
- 디자인 시스템
- 공통 hooks

---

# 📦 Installation

## 1. pnpm 설치

```
npm install -g pnpm
```

---

## 2. 의존성 설치

```
pnpm install
```

---

# 💻 Development

```
pnpm dev
```

기본 실행 주소:

```
http://localhost:3000
```

---

# 🏗 Build

```
pnpm build
```

---

# ▶ Production Run

```
pnpm start
```

---

# 🌐 Environment Variables

`.env.local` 파일을 생성하여 환경 변수를 설정합니다.

```
NEXT_PUBLIC_API_URL=
```

---

# 🎨 Styling Guide

본 프로젝트는 **Tailwind CSS** 기반으로 스타일을 관리합니다.

- Utility First 구조
- 디자인 토큰 확장 예정
- 반응형 UI 지원

---

# 📱 PWA

향후 서비스 확장을 위해
Progressive Web App 환경을 지원할 예정입니다.

---

# 📏 Code Convention

## Commit Message Convention

```
feat: 기능 추가
fix: 버그 수정
refactor: 리팩토링
style: UI 변경
chore: 설정 변경
docs: 문서 수정
```

---

## Folder Naming

```
kebab-case
```

---

## Component Naming

```
PascalCase
```

---

# 🧪 Testing (예정)

- Unit → Vitest or Jest
- E2E → Playwright

---

# 📦 Future Improvements

- 상태 관리 구조 고도화
- 디자인 시스템 구축
- PWA 기능 확장
- 테스트 환경 구축
