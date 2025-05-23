# Chapter 02: Networking Refresher (Theory)

## 1. 네트워킹 기초

### 1.1 OSI 7계층 모델
OSI 7계층 모델은 네트워크 통신을 7개의 계층으로 나누어 각 계층이 담당하는 역할을 정의합니다.

| 계층 | 이름             | 주요 역할 및 예시                |
|------|------------------|----------------------------------|
| 7    | 응용 (Application) | 사용자와 직접 상호작용, HTTP, FTP |
| 6    | 표현 (Presentation) | 데이터 형식 변환, 암호화, 압축    |
| 5    | 세션 (Session)     | 세션 관리, RPC, NetBIOS         |
| 4    | 전송 (Transport)   | 신뢰성, 흐름제어, TCP/UDP        |
| 3    | 네트워크 (Network) | 라우팅, IP, ICMP                 |
| 2    | 데이터링크 (Data Link) | MAC, 스위치, 이더넷           |
| 1    | 물리 (Physical)    | 케이블, 허브, 전기적 신호        |

---

### 1.2 IPv4와 서브넷팅

- **IPv4 주소:** 32비트, 4개의 옥텟(예: 192.168.0.1)
- **서브넷팅:** 네트워크를 더 작은 단위로 분할하여 효율적 관리 및 보안 강화
- **서브넷 마스크:** 네트워크/호스트 구분 (예: 255.255.255.0)

#### 주요 개념
- **Public IP:** 인터넷에서 사용 가능한 주소
- **Private IP:** 내부 네트워크에서만 사용 (예: 10.0.0.0/8, 192.168.0.0/16)
- **NAT:** 사설 IP를 공인 IP로 변환

---

### 1.3 VLAN, 트렁크, VPN

- **VLAN:** 논리적으로 네트워크를 분리 (보안, 트래픽 분리)
- **트렁크:** 여러 VLAN의 트래픽을 한 링크로 전달
- **VPN:** 인터넷을 통한 사설 네트워크 연결 (IPSec 등)

---

### 1.4 DNS와 BGP

- **DNS:** 도메인 이름을 IP 주소로 변환
- **BGP:** 인터넷의 라우팅 프로토콜, 경로 선택

---

### 1.5 네트워크 실무 용어

- **DHCP:** IP 자동 할당
- **라우팅:** 패킷의 경로 결정
- **서브넷:** 네트워크 분할 단위

---

## 2. 마인드맵 및 연습문제

```
네트워킹 기초
│
├─ OSI 7계층
│   ├─ 응용
│   ├─ 표현
│   ├─ 세션
│   ├─ 전송
│   ├─ 네트워크
│   ├─ 데이터링크
│   └─ 물리
├─ IP/서브넷
│   ├─ Public/Private
│   ├─ NAT
│   └─ 서브넷 마스크
├─ VLAN/트렁크/VPN
├─ DNS/BGP
└─ DHCP/라우팅/서브넷
----------------------------

연습문제

1. OSI 7계층의 각 계층 이름과 역할을 간단히 설명하시오.
2. Public IP와 Private IP의 차이점을 설명하시오.
3. 서브넷팅의 장점 2가지를 적으시오.
4. VLAN과 VPN의 차이점을 설명하시오.
```
