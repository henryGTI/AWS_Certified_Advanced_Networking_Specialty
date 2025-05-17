# Chapter 04: Design and Implement Hybrid Networks at Scale (Practice)

## 실습 1: AWS Site-to-Site VPN 연결 구성

1. AWS Management Console에서 "VPN 연결" 생성
2. 가상 프라이빗 게이트웨이(VGW) 생성 및 VPC에 연결
3. 고객 게이트웨이(Customer Gateway) 정보 입력(온프레미스 라우터의 공인 IP)
4. VPN 연결 생성 및 터널 정보 확인
5. 온프레미스 라우터에 터널 정보 적용

---

## 실습 2: Direct Connect 연결 시나리오

1. AWS Direct Connect 콘솔에서 "Direct Connect 연결" 요청
2. 파트너사 또는 통신사와 물리적 회선 연결
3. 가상 인터페이스(VIF) 생성(Private/Public)
4. 라우팅(BGP) 설정 및 테스트

---

## 실습 3: CloudHub 아키텍처 실습

1. 여러 고객 게이트웨이(Customer Gateway) 등록
2. 각각의 VPN 연결을 CloudHub로 구성
3. 각 지사/사이트 간 통신 테스트

---

## 실습 4: 하이브리드 네트워크 고가용성 설계

1. 이중 VPN 터널 구성
2. Direct Connect와 VPN 백업 경로 동시 구성
3. 장애 발생 시 자동 장애 조치 테스트

---

## 실습 결과 캡처/정리

- 각 실습 단계별로 캡처 이미지, 명령어, 결과 등을 추가로 정리하세요.
