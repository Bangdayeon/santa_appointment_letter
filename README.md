# 🎅 산타 임명장 🎅
- 친구에게 어울리는 산타를 선택하고 메시지와 함께 **산타 임명장**을 수여할 수 있는 웹 서비스입니다.  
- 로그인을 통해 개인 작업실을 생성하고, 친구들에게 공유하여 임명장을 주고받을 수 있어요.
- 간단한 **성격 테스트**를 통해 친구에게 어울리는 산타를 골라 임명장을 보내요.

## 🔗 링크

- **Service**: https://www.iamsanta.site
- **Notion (기획/문서)**: https://www.notion.so/2c0add99c04280c08879d1810dd4eebb


## 🛠 기술 스택

### Frontend
- **Framework**: Next.js (App Router)
- **Language**: TypeScript
- **Styling**: TailwindCSS

### Backend
- **API**: Next.js API Routes
- **Database**: Supabase

### Authentication
- **OAuth**: Kakao Login

### Analytics
- **Google Analytics**
- **Google Tag Manager**

### Development Tools
- **Package Manager**: pnpm
- **Lint & Formatter**: ESLint, Prettier

### Deployment
- **Vercel** (Custom Domain 연결)

## ✨ 주요 기능

- 카카오 OAuth 로그인
- 개인 작업실 생성 및 공유
- 성격 테스트 기반 산타 추천
- 친구에게 메시지와 함께 산타 임명장 전달

## 🔧 구현 포인트

- Next.js App Router 기반 SSR/CSR 구조
- Supabase를 활용한 인증 및 데이터 관리
- API Route를 통한 서버 로직 처리
- Google Analytics / GTM을 통한 사용자 행동 분석

## 🚀 시작하기
### 1. 클론 & 설치
```
# 저장소 클론
git clone https://github.com/Bangdayeon/santa_appointment_letter.git

# 의존성 설치
pnpm install
```
### 2. 개발 모드 실행
```
pnpm run dev
```
브라우저에서 http://localhost:3000 열기

### 3. 빌드 & 프로덕션 모드
```
# 프로덕션 빌드
pnpm run build

# 프로덕션 서버 실행
pnpm run start
```

## 📜 사용 가능한 스크립트
- `pnpm run dev` - 개발 서버 실행
- `pnpm run build` – 프로덕션 빌드 생성
- `pnpm run start` – 프로덕션 서버 실행
- `pnpm run lint` – ESLint 실행
- `pnpm run format` – Prettier 포맷 실행
- `pnpm run lint:staged` – lint-staged로 변경된 파일 린트 및 포맷

## 📂 폴더 구조

```
└── src
    ├── app/             # App Router 페이지 & 레이아웃 & next.js api route
    ├── assets/          # icon svg 파일
    ├── components/      # 재사용 가능한 React 컴포넌트
    ├── contexts/        # context
    ├── hooks/           # 공용 훅
    ├── lib/             # Supabase 설정, 상수 데이터, 공통 유틸리티 등을 관리하는 모듈
    ├── styles/          # 공용 스타일링 css 파일
    ├── types/           # 타입 정의
    └── utils/           # 서버 요청 처리, Supabase 연동, 날짜 포맷 등 공통 유틸리티 함수
```
