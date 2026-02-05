# 🧩 heemo-web

Heemo 서비스의 사용자용 웹 애플리케이션입니다.
Next.js 기반으로 구축되며, 확장성과 유지보수성을 고려한 구조를 목표로 개발되었습니다.

---

## 📌 Overview

본 프로젝트는 **Feature-Sliced Design(FSD)** 아키텍처를 기반으로 구성되어
기능 단위로 구조를 분리하고, 재사용성과 확장성을 높이는 것을 목표로 합니다.

---

## 🚀 Tech Stack

### Core

* Next.js (App Router)
* React
* TypeScript

### Styling

* Tailwind CSS

### State & Data

* React Query (Planned)
* Zustand (Planned)

### Tooling

* pnpm
* Turbopack

### Architecture

* Feature-Sliced Design (FSD)

---

## 📱 Key Features

* 사용자 중심 UI/UX 설계
* 반응형 웹 지원
* PWA 지원 예정
* 확장 가능한 프론트엔드 아키텍처

---

## 🧱 Architecture

본 프로젝트는 **Feature-Sliced Design(FSD)** 구조를 따릅니다.

```
src/
 ┣ app/
 ┣ pages/
 ┣ widgets/
 ┣ features/
 ┣ entities/
 ┣ shared/
```

### app

* Next.js 라우팅 및 전역 설정
* Layout, Provider, Routing 관리

### pages

* 페이지 단위 구성
* 여러 widgets 및 features 조합

### widgets

* 독립적인 UI 블록
* 페이지 구성 단위

### features

* 사용자 행동 단위 기능
* 예: 인증, 검색, 필터링 등

### entities

* 비즈니스 도메인 모델
* API 모델 및 상태 로직 관리

### shared

* 전역 공통 모듈
* UI 컴포넌트
* 유틸 함수
* 디자인 시스템
* 공통 Hooks

---

## 📦 Installation

### 1. pnpm 설치

```
npm install -g pnpm
```

### 2. 의존성 설치

```
pnpm install
```

---

## 💻 Development

```
pnpm dev
```

Application runs at:

```
http://localhost:3000
```

---

## 🏗 Build

```
pnpm build
```

---

## ▶ Production Run

```
pnpm start
```

---

## 🌐 Environment Variables

`.env.local` 파일을 생성하여 환경 변수를 설정합니다.

```
NEXT_PUBLIC_API_URL=
```

---

## 🎨 Styling Guide

본 프로젝트는 **Tailwind CSS** 기반으로 스타일을 관리합니다.

* Utility-first 방식
* 디자인 토큰 확장 예정
* 반응형 UI 지원

---

## 📱 PWA

서비스 확장을 고려하여
Progressive Web App 지원을 계획하고 있습니다.

---

## 📏 Code Convention

### Commit Message Convention

```
feat: 새로운 기능 추가
fix: 버그 수정
refactor: 코드 리팩토링
style: UI 스타일 변경
chore: 설정 및 환경 변경
docs: 문서 수정
```

### Naming Convention

| 대상        | 규칙         |
| --------- | ---------- |
| Folder    | kebab-case |
| Component | PascalCase |

---

## 🧪 Testing (Planned)

* Unit Test → Vitest or Jest
* E2E Test → Playwright

---

## 📦 Future Improvements

* 상태 관리 구조 고도화
* 디자인 시스템 구축
* PWA 기능 확장
* 테스트 환경 구축
