# Frontend Development Plan

이 문서는 Gosu Drive 관리자 사이트의 프런트엔드 개발을 위한 초기 계획입니다.

## 1. 베이스 템플릿 구성
- Tailwind CSS, Flowbite, HTMX, Alpine.js CDN 로드
- 공통 레이아웃: 상단 네비게이션 바와 사이드바 슬롯 마련

## 2. 모달 파셜 제작
- 예약 생성 모달 (`booking_create_modal.html`)
- 회원 잔여시간 조정 모달 (`member_balance_adjust_modal.html`)
- 폼 오류 표시 파셜 (`partials/_form_errors.html`)

## 3. 캘린더 페이지
- FullCalendar 통합
- 모달과 이벤트 연동 (예약 생성/취소 시 리프레시)

## 4. 리스트 페이지 및 레이아웃
- 네비게이션 바와 사이드바 파셜 추가
- 회원 목록 템플릿 (`members/index.html`)과 잔여시간 조정 모달 연동
- 예약 목록 템플릿 (`bookings/index.html`)과 예약 생성/취소 버튼
- 예약/ledger 테이블 파셜화 (`partials/_booking_table.html`, `partials/_ledger_table.html`)
- 회원 상세 템플릿 (`members/detail.html`)에 HTMX 기반 부분 갱신 연결

## 5. 향후 작업 항목
- 상품 리스트 페이지 템플릿화
- 네비게이션, 사이드바 컴포넌트 반응형 세분화
- 다크 모드 및 반응형 최적화
- 대시보드와 리포트 초기 레이아웃 스케치

진행 상황에 따라 추가 세부 계획을 보완할 예정입니다.
