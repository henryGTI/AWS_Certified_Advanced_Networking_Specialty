# Chapter 03: Design and Implement AWS Networks (Theory)

## 1. AWS 글로벌 인프라 구조

- **리전(Region):** AWS의 물리적 데이터센터 집합(예: ap-northeast-2, 서울)
- **가용 영역(Availability Zone, AZ):** 한 리전 내 여러 개의 독립된 데이터센터
- **엣지 로케이션(Edge Location):** CDN, 캐시 등 엣지 서비스 제공

---

## 2. VPC와 기본 네트워킹 설계

- **VPC(Virtual Private Cloud):** AWS 내에서 논리적으로 분리된 네트워크
- **서브넷(Subnet):** VPC 내에서 IP 대역을 분할한 네트워크
- **라우팅 테이블:** 서브넷 간, 인터넷 간 트래픽 경로 지정
- **인터넷 게이트웨이(IGW):** VPC를 인터넷에 연결

---

## 3. VPC 라우터(Deep Dive)

- VPC 내 트래픽 라우팅 담당
- 라우팅 테이블을 통해 서브넷별 트래픽 경로 지정

---

## 4. ENI, EIP, IGW (Deep Dive)

- **ENI(Elastic Network Interface):** EC2 인스턴스에 부착 가능한 네트워크 인터페이스
- **EIP(Elastic IP):** 고정 공인 IP, 필요시 인스턴스에 할당
- **IGW(Internet Gateway):** VPC와 인터넷을 연결

---

## 5. 보안 그룹과 NACL (Deep Dive)

- **보안 그룹(Security Group):** 인스턴스 단위 방화벽, 상태 저장(Stateless)
- **NACL(Network ACL):** 서브넷 단위 방화벽, 상태 비저장(Stateless)

---

## 6. NAT, VGW, VPC Peering, VPC Endpoint

- **NAT Gateway/Instance:** 프라이빗 서브넷에서 인터넷 접근 허용
- **VGW(Virtual Private Gateway):** 온프레미스와 VPC 간 VPN 연결
- **VPC Peering:** VPC 간 프라이빗 네트워크 연결
- **VPC Endpoint:** VPC 내에서 AWS 서비스에 프라이빗하게 접근

---

## 7. 멀티 VPC 아키텍처

- 여러 VPC를 조합하여 대규모 네트워크 설계
- Peering, Transit Gateway, Endpoint 등 활용

---

## 8. 마인드맵 및 연습문제

```
AWS 네트워크 설계
│
├─ 글로벌 인프라
│   ├─ 리전
│   ├─ AZ
│   └─ 엣지 로케이션
├─ VPC
│   ├─ 서브넷
│   ├─ 라우팅 테이블
│   ├─ IGW
│   ├─ ENI/EIP
│   ├─ 보안 그룹/NACL
│   ├─ NAT/VGW
│   ├─ VPC Peering
│   └─ VPC Endpoint
└─ 멀티 VPC 아키텍처
----------------------------

연습문제

1. VPC와 서브넷의 차이점을 설명하시오.
2. 보안 그룹과 NACL의 차이점을 서술하시오.
3. NAT Gateway의 역할을 설명하시오.
4. VPC Peering과 VPC Endpoint의 차이점을 설명하시오.
```
