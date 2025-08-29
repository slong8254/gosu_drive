# Gosu Drive

Gosu Drive는 운전 연습 학원의 회원 관리와 수업 예약을 위한 Django 기반 웹서비스입니다.

## 주요 기능 (MVP)
- **회원 관리**: 프로필, 잔여시간, 예약 및 결제 이력 관리
- **수업 상품**: 강사와 기간을 포함한 상품 관리, 기본 차감 시간 설정
- **예약 & 시간 차감**: 회원이 상품과 시간을 선택해 예약하면 잔여 시간이 차감되며, 취소 시 100% 복구
- **캘린더 뷰**: FullCalendar로 월/주/일 단위 예약 현황 확인
- **잔여시간 조정**: 관리자 권한으로 회원 잔여시간을 직접 증감
- **HTMX 부분 갱신**: 예약 생성·취소 및 잔여시간 조정 시 관련 테이블과 배지가 자동 갱신
- **관리자 로그인**: Django 인증 기반 관리자/강사 계정 관리

## 기술 스택
- Python 3.11+, Django 5.x
- 프런트엔드: Django Template + Tailwind CSS(Play CDN) + Flowbite(CDN) + HTMX + Alpine.js
- 데이터베이스: SQLite (개발) / PostgreSQL (운영 권장)

## 개발 목표
1. 빠르게 동작하는 관리자 전용 백오피스 구축
2. 예약·취소 시 일관된 시간 차감과 복구 처리
3. 향후 분석, 정산, 알림 기능으로 확장 가능한 구조 유지

## 로컬 개발
```bash
# 가상환경 및 의존성 설치 (예시)
python -m venv .venv
source .venv/bin/activate
pip install django

# 프로젝트 실행
python manage.py runserver
```

현재 저장소에는 기본 레이아웃, 모달 파셜, 캘린더·회원·예약 리스트 등 프런트엔드 UI 스켈레톤이 포함되어 있으며, 세부 기능은 진행 중입니다.

프런트엔드 작업 계획은 `FRONTEND_PLAN.md` 파일을 참고하세요.
전체 프로젝트 개요와 세부 로드맵은 `PROJECT_PLAN.md`에서 확인할 수 있습니다.
