# Chapter 04: Design and Implement Hybrid Networks at Scale (Theory)

## 1. 하이브리드 네트워크란?

- 온프레미스(내부 데이터센터)와 AWS 클라우드를 연결하여 하나의 네트워크처럼 사용하는 구조
- 보안, 확장성, 유연성, 재해복구 등 다양한 목적

---

## 2. 하이브리드 네트워크의 필요성

- **Reactive Reasons:** 장애 복구, 데이터 마이그레이션, 임시 확장 등
- **Pro-active Reasons:** 비용 최적화, 글로벌 서비스 확장, 규제 준수 등

---

## 3. AWS 하이브리드 네트워크 서비스

- **VPN (Virtual Private Network):** 인터넷을 통한 암호화된 연결
- **Direct Connect:** 전용선 기반의 고속, 안정적 연결
- **CloudHub:** 여러 사이트를 AWS와 연결하는 허브 구조
- **QinQ-VLAN Stacking:** 복수 VLAN 태깅을 통한 네트워크 분리

---

## 4. VPN의 종류와 특징

### 4.1 소프트웨어 VPN
- 소프트웨어 기반 VPN 서버/클라이언트 사용
- 장점: 저비용, 빠른 구축
- 단점: 성능, 확장성 한계

### 4.2 하드웨어 VPN (VPC VPN)
- 전용 장비를 통한 VPN 연결
- 장점: 고성능, 안정성
- 단점: 비용, 구축 복잡성

---

## 5. Direct Connect (DX)

- AWS와 온프레미스 간 전용선 연결
- 높은 대역폭, 낮은 지연, 안정적 네트워크 품질
- Private VIF, Public VIF 등 다양한 연결 방식

---

## 6. CloudHub 아키텍처

- 여러 지사/사이트를 AWS와 연결하는 허브-스포크 구조
- VPN, Direct Connect 혼합 가능

---

## 7. 하이브리드 네트워크의 고가용성/복원력

- 이중화, 다중 경로, 자동 장애 조치 설계 필요
- AWS 리전/가용영역, 온프레미스 장비 이중화 등

---

## 8. 마인드맵 및 연습문제

```
하이브리드 네트워크
│
├─ 필요성
│   ├─ Reactive
│   └─ Pro-active
├─ AWS 서비스
│   ├─ VPN
│   ├─ Direct Connect
│   ├─ CloudHub
│   └─ QinQ-VLAN
├─ VPN 종류
│   ├─ 소프트웨어 VPN
│   └─ 하드웨어 VPN
├─ Direct Connect
├─ CloudHub 아키텍처
└─ 고가용성/복원력
----------------------------

연습문제

1. 하이브리드 네트워크의 대표적인 활용 사례를 2가지 서술하시오.
2. 소프트웨어 VPN과 하드웨어 VPN의 차이점을 설명하시오.
3. Direct Connect의 장점 2가지를 적으시오.
4. CloudHub 아키텍처의 특징을 설명하시오.
```
