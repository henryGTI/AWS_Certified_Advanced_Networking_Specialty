# Chapter 05: Configure Network Integration with Application Services (Theory)

## 1. Route 53

- AWS의 관리형 DNS(도메인 네임 시스템) 서비스
- 도메인 이름을 IP 주소로 변환
- 다양한 라우팅 정책(단순, 가중치, 지연 시간, 장애 조치 등) 지원

---

## 2. 하이브리드 DNS

- 온프레미스와 AWS 간 DNS 연동
- Split View(내부/외부 DNS 분리), Private Hosted Zone 활용

---

## 3. VPC DHCP

- VPC 내 인스턴스에 자동으로 IP, DNS 등 네트워크 정보 할당

---

## 4. Elastic Load Balancer (ELB)

- 여러 EC2 인스턴스에 트래픽을 분산
- **Classic Load Balancer:** L4/L7 지원, 구형
- **Application Load Balancer:** L7(HTTP/HTTPS) 트래픽 분산
- **Network Load Balancer:** L4(TCP/UDP) 고성능 분산

---

## 5. S3와 CloudFront

- **S3:** 객체 스토리지 서비스, 정적 웹 호스팅 가능
- **CloudFront:** 글로벌 CDN, S3/EC2/온프레미스 등 다양한 오리진 지원
- **GeoRestriction:** 지역별 접근 제한
- **SSL, 캐싱, 최적화 등 다양한 기능 제공**

---

## 6. 로컬/글로벌 복원력 전략

- 여러 리전/가용영역에 걸친 서비스 배포
- 장애 발생 시 자동 장애 조치, 데이터 복제 등

---

## 7. AWS WorkSpaces

- 클라우드 기반 가상 데스크톱 서비스
- 보안, 확장성, 관리 편의성 제공

---

## 8. 마인드맵 및 연습문제

```
네트워크와 애플리케이션 통합
│
├─ Route 53
│   ├─ 라우팅 정책
│   └─ 하이브리드 DNS
├─ VPC DHCP
├─ ELB
│   ├─ Classic
│   ├─ Application
│   └─ Network
├─ S3/CloudFront
│   ├─ CDN
│   ├─ GeoRestriction
│   └─ 최적화/보안
├─ 복원력 전략
└─ WorkSpaces
----------------------------

연습문제

1. Route 53의 주요 기능을 2가지 이상 서술하시오.
2. Application Load Balancer와 Network Load Balancer의 차이점을 설명하시오.
3. S3와 CloudFront의 차이점과 연동 시 장점을 설명하시오.
4. 하이브리드 DNS란 무엇이며, 어떤 상황에서 사용하는지 설명하시오.
```
