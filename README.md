<img width="2621" height="551" alt="logo" src="https://github.com/user-attachments/assets/8ddb1b3d-2bed-410e-b68d-abec2c59ce6e" />

<img width="2162" height="982" alt="image" src="https://github.com/user-attachments/assets/d1c8a922-9cfc-4501-ac20-e366b81e4b9a" />
<img width="2088" height="932" alt="image" src="https://github.com/user-attachments/assets/2708a5a8-03f6-4ce1-8216-c6e9bb5588e1" />




---
## ☔ About Project
- UNICORN 해커톤 참여 <img width="19.2" height="25.8" alt="korea-logo" src="https://github.com/user-attachments/assets/b29e9d4b-fff7-41eb-928e-9321dd35a557" />
- 2025.07.20 ~ 2025.08.31
- PM(1) · Designer(2) · Full Stack(2) 
- (✅)를 통해 저의 개발 기여를 확인하실 수 있습니다.
---
## 🛠 Tech Stack
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)

| Type | Tech Stack <img width = 690> |
| :---: | --- |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white) |
| **Auth** | ![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white) |
| **Feature** | ![QR Code](https://img.shields.io/badge/QR_Code-000000?style=flat) ![Jimp](https://img.shields.io/badge/Jimp-4B32C3?style=flat) ![Resend](https://img.shields.io/badge/Resend-000000?style=flat&logo=resend&logoColor=white) ![Nodemailer](https://img.shields.io/badge/Nodemailer-22B573?style=flat) |
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
