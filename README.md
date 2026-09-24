<img width="2621" height="551" alt="logo" src="https://github.com/user-attachments/assets/8ddb1b3d-2bed-410e-b68d-abec2c59ce6e" />

<img width="2162" height="982" alt="image" src="https://github.com/user-attachments/assets/d1c8a922-9cfc-4501-ac20-e366b81e4b9a" />
<img width="2088" height="932" alt="image" src="https://github.com/user-attachments/assets/2708a5a8-03f6-4ce1-8216-c6e9bb5588e1" />




---
## ☔ About Project

### 📌 Project

- UNICORN 해커톤 참여 <img width="19.2" height="25.8" alt="korea-logo" src="https://github.com/user-attachments/assets/b29e9d4b-fff7-41eb-928e-9321dd35a557" />
- 2025.07.20 ~ 2025.08.31
- PM(1) · Designer(2) · Full Stack(2)

### 👩🏻‍💻 My Role

- `Prisma` 기반 `MySQL` 연동 및 DB 스키마 설계
- `MyPage`/`QR`/`QR Scan` 도메인 API 구현
- `Resend`를 활용한 회원가입 이메일 인증 구현 (인증 토큰 링크 발송 및 검증)
- `Railway`를 이용한 Backend Server 및 MySQL DB 배포

---
## 📡 API

| Domain | Method | Endpoint | Description |
| :---: | :---: | --- | --- |
| **User** | POST | `/user/signup` | 회원가입 및 인증 메일 발송 |
| | GET | `/user/email-verify` | 이메일 인증 처리 |
| | POST | `/user/login` | 로그인 (JWT 발급) |
| | GET | `/user/:id` | 사용자 정보 조회 |
| **MyPage** | GET | `/mypage?userId={id}` | 마이페이지 정보 조회 |
| **QR** | GET | `/qr/png?text={text}` | QR 코드 PNG 생성 |
| | GET | `/qr/dataurl?text={text}` | QR 코드 Data URL 생성 |
| | POST | `/qr/png` | QR 코드 PNG 생성 (Body) |
| **QR Scan** | POST | `/qr-scan/scan` | QR 스캔으로 우산 대여/반납 처리 |
| | GET | `/qr-scan/umbrella/:id` | 우산 정보 조회 |
| **Store** | GET | `/store/initialmap` | 지도 초기 진입 시 가게 마커 조회 |
| | POST | `/store/search` | 가게명으로 검색 |
| | GET | `/store/hashtag/:tagName` | 해시태그(날씨 키워드)별 가게 조회 |
| **Place** | POST | `/search-place` | 네이버 지역 검색 API 기반 장소 검색 |
| **Weather** | GET | `/weather/current?lat={lat}&lon={lon}` | 현재 위치 날씨 조회 |

---
## 🛠 Tech Stack
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white) ![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat&logo=railway&logoColor=white)

| Type | Tech Stack <img width = 680> |
| :---: | --- |
| **Database** |![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white) |
| **Auth** | ![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white) |
| **Feature** | ![QR Code](https://img.shields.io/badge/QR_Code-000000?style=flat) ![Jimp](https://img.shields.io/badge/Jimp-4B32C3?style=flat) ![Resend](https://img.shields.io/badge/Resend-000000?style=flat&logo=resend&logoColor=white) |
| **Logging & Test** | ![Winston](https://img.shields.io/badge/Winston-5A5A5A?style=flat) ![Jest](https://img.shields.io/badge/Jest-C21325?style=flat&logo=jest&logoColor=white) |
---
## 📂 File Structure

```
📦 project
├── db/                     # DB 초기화 스크립트 및 설정
├── prisma/                 # Prisma 스키마, 마이그레이션, 시드 데이터
|
└── src/
    ├── auth/               # 로그인, 회원가입, JWT 인증
    ├── config/             # 환경 변수 및 앱 설정
    ├── email/              # 이메일 발송 (인증 메일 등)
    ├── logger/             # Winston 기반 로깅
    ├── mypage/             # 마이페이지 (내 정보, 리워드 내역 등)
    ├── qr/                 # QR 코드 생성
    ├── qr-scan/            # QR 스캔 처리 (우산 대여/반납)
    ├── search-place/       # 장소 검색
    ├── store/              # 제휴 가게 정보 및 추천
    ├── user/               # 사용자 정보 관리
    ├── user_qr/            # 사용자별 QR 정보 관리
    ├── utils/
    │   └── decorators/     # 커스텀 데코레이터
    └── weather/            # 날씨 API 연동 
```
