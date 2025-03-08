# 할 일 관리 서비스
업무 효율을 높이기 위해 프로젝트와 세부적인 업무 관리를 지원하는 서비스

<br />


## 프로젝트 개요
본 서비스는 다양한 기능과 직관적인 UI/UX를 통해 할 일을 효율적으로 관리할 수 있도록 도모하는 서비스입니다.

주요 정책은 ‘공간 정책’과 ‘역할 정책’을 중심으로 구성되어 있습니다.
첫 번째, 공간정책으로는 워크스페이스와 프로젝트, 보드, 할 일로 분리합니다.
워크스페이스는 여러 개의 프로젝트를 포함하며, 각 프로젝트는 다수의 보드와 할일을 가질 수 있습니다. 
두 번째, 역할정책으로는 워크스페이스 관리자와 프로젝트 관리자, 일반 참여자로 분리합니다.
워크스페이스 관리자는 워크스페이스에 사람을 초대할 권한을 가지고 있으며, 프로젝트 관리자는 해당 프로젝트를 총괄하여 업무의 진행상황을 파악할 수 있습니다.

주요 기능으로는 실시간 알림, 쪽지, 드래그 앤 드롭(DND)을 기반으로 한 칸반뷰와 목록뷰가 있으며, 업무 변경내역 파악하기 위한 히스토리 기능과 업무에 대한 피드백이 가능한 댓글 기능 등이 추가로 포함되어 있습니다. 
워크스페이스 메인페이지에는 할 일을 보다 효율적으로 관리할 수 있도록 다양한 서비스를 제공하며, 그에 대한 종류로는 공지사항, 구성원 목록, 타임라인뷰, 할 일 D-3이 있습니다.
이를 통해 사용자는 할일의 현황과 일정을 직관적으로 파악할 수 있습니다.

<br />

## 기대효과
1. 개인 업무와 그룹 업무를 분리하여, 프라이빗한 할 일 관리 가능
2. 타임라인과 진행상황 칸반보드로, 직관적인 업무 현황 파악 가능
3. 실시간 알림과 쪽지, 댓글 기능을 통한 그룹 간의 소통 향상
4. 분업화된 권한으로, 체계적인 업무 환경 조성
5. 프로젝트로 분리되어 그룹 내 다양한 업무 환경 조성 
<br />


## 사용기술
- 개발환경 : Oracle Linux Server 8.6
- 백엔드 : Java 11, Spring Boot 2.7.4, Spring Security, Spring Data Jpa, QueryDsl, Spring Mail
- 프론트 : Typescript, React.js, Zustand, MUI
- DB : Postgresql, Redis
- 인프라 : AWS(EC2, S3, CLOUDFRONT, ROUTE53, ELB, RDS), Docker
<br />


## 시스템 아키텍처
![daon_arch](https://github.com/user-attachments/assets/a05ab038-0d9c-4401-98cb-0055ab654408)
<br />


## ERD
- TODO ERD 이미지 업로드
<br />


## 역할
### 김성은
- 서비스 내 페이지 이동 관리
- 전체 화면 구성 및 UI 구조 설계
- LNB 개발
- 할 일 관리 UI 개발
- 할 일 칸반보드 드래그 앤 드롭 기능 개발
- 공지사항 기능 및 UI 개발

### 김재윤
- 워크스페이스/프로젝트/보드/초대장/쪽지 기능 개발
- SSE 실시간 처리 시스템 개발
- 가입 인증 메일 송신 및 처리 시스템 개발
- 역할별 권한 분리 및 기능 세분화

### 유하영
- 프론트엔드, 백엔드 개발환경 구축 및 인프라 환경 구축
- 테스트, 빌드 배포 자동화 파이프라인 구축
- 시큐리티 인증 처리, JWT 인증 처리, 로그인 토큰 발급
- 히스토리 기능 및 UI 개발
- SSE 기능 이용 실시간 알림 처리 개발

### 조수연
- 랜딩 페이지 개발
- 회원가입 기능 및 UI 개발
- 로그인 UI 개발
- 할 일 생성 및 관리, 댓글 기능 개발
<br />


## 주요 화면
### 회원가입 페이지
![01](https://github.com/user-attachments/assets/f4ae8870-1505-452e-8e43-c96bf8ef329c)

### 워크스페이스 메인 페이지
![02](https://github.com/user-attachments/assets/2066acf3-f4c5-47d3-a0ff-b68de03b1208)

### 할 일 목록 페이지
![03](https://github.com/user-attachments/assets/3a47218f-eff1-482b-8675-dab64d8a501e)

### 할 일 상세 모달
![04](https://github.com/user-attachments/assets/bba2b4bd-8d6e-4321-9e49-05f1df3160ae)

### 할 일 생성 모달
![05](https://github.com/user-attachments/assets/6f2bf133-4d96-4d54-8fd8-5114c624abd5)

### 프로젝트 생성 모달
![06](https://github.com/user-attachments/assets/92e0e073-eba4-4585-8903-44d5c1e82132)

### 프로젝트 설정
![07](https://github.com/user-attachments/assets/a8e7fbcb-36a6-4351-8b20-e92b1e25f40b)

### 워크스페이스 생성 모달
![08](https://github.com/user-attachments/assets/4583164d-1f24-4b65-bdb6-8e642a03225f)

### 워크스페이스 설정 모달
![09](https://github.com/user-attachments/assets/d747911d-a80d-47c4-91cf-7a68a1e53614)

### 알림 모달
![10](https://github.com/user-attachments/assets/1937f454-479e-43ea-96a7-08d4627116c5)

### 검색 모달
![11](https://github.com/user-attachments/assets/999d9ed6-987a-4cac-b4a0-6fc32491a3e4)

