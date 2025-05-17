# Chapter 06: Manage, Optimize, and Troubleshoot The Network (Theory)

## 1. VPC Flow Logs

- VPC, 서브넷, 네트워크 인터페이스의 트래픽 정보를 캡처하는 로그 서비스
- 네트워크 트래픽 분석, 보안 감사, 문제 해결에 활용

---

## 2. 네트워크 ACL과 보안 그룹

- **보안 그룹(Security Group):** 인스턴스 단위, 상태 저장(Stateless)
- **네트워크 ACL(Network ACL):** 서브넷 단위, 상태 비저장(Stateless)
- **Flow Logs와 연계하여 접근 제어 및 트래픽 분석 가능**

---

## 3. 네트워크 비용 관리 및 최적화

- **비용 모니터링:** AWS Cost Explorer, CloudWatch 등 활용
- **최적화 전략:** 데이터 전송 최소화, 리소스 통합, 캐싱, 리전/가용영역 선택 등

---

## 4. Enhanced Networking

- **ENA(Elastic Network Adapter), SR-IOV 등 고성능 네트워킹 지원**
- 대용량 트래픽, 저지연 네트워크 환경에 적합

---

## 5. Placement Group

- **Placement Group:** EC2 인스턴스의 물리적 배치 전략
  - **Cluster:** 저지연, 고대역폭 통신
  - **Spread:** 장애 도메인 분산
  - **Partition:** 대규모 워크로드 분산
- **제약사항:** 인스턴스 유형, 리전/가용영역 등

---

## 6. 네트워크 문제 해결

- **Flow Logs, CloudWatch, VPC Reachability Analyzer 등 활용**
- 보안 그룹/NACL/라우팅 테이블/네트워크 경로 점검

---

## 7. 마인드맵 및 연습문제

```
네트워크 관리/최적화/문제해결
│
├─ VPC Flow Logs
├─ 보안 그룹/NACL
├─ 비용 관리/최적화
├─ Enhanced Networking
├─ Placement Group
└─ 문제 해결 도구
----------------------------

연습문제

1. VPC Flow Logs의 주요 활용 사례를 2가지 이상 서술하시오.
2. 보안 그룹과 NACL의 차이점을 설명하시오.
3. Enhanced Networking이 필요한 상황을 예시로 설명하시오.
4. Placement Group의 유형과 각각의 특징을 설명하시오.
```
