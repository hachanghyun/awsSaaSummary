# awsSaaSummary

    IAM = Identity and Access Management, Global service
    인바운드 규칙은 외부에서 Ec2 인스턴스로 연결할 수 있게 해주는 규칙
    SSH는 터미널이나 명령줄을 이용해서 원격 머신이나 서버를 제어할 수 있게 해줌
    EC2 인스턴스 connect ssh와 같은 방식으로 웹에서 빠르게 연결가능한 connect

##### Q.EC2 인스턴스에 고성능 컴퓨팅(HPC) 애플리케이션을 배포하려 합니다. 다음 중 어떤 EC2 인스턴스 유형을 선택해야 할까요?
    A.컴퓨팅 최적화 EC2 인스턴스는 고성능 프로세서(예: 배치 처리, 미디어 트랜스코딩, 고성능 컴퓨팅, 과학적 모델링 및 머신 러닝, 전용 게이밍 서버 등)가 필요한 집중 컴퓨팅 워크로드에 적합합니다.

##### Q.1년 간 지속적으로 서버를 운영할 계획인 애플리케이션의 경우에는 다음 중 어떤 EC2 구매 옵션을 사용해야 할까요?
    A.예약 인스턴스는 장기적인 워크로드에 적합합니다. EC2 인스턴스는 1년, 혹은 3년의 기간으로 예약할 수 있습니다.

##### Q.일련의 EC2 인스턴스에 호스팅 될 애플리케이션을 실행하려 합니다. 이 애플리케이션에는 소프트웨어 설치가 필요하며, 최초 실행 중에 일부 OS 패키지를 업데이트해야 합니다. EC2 인스턴스를 실행하려는 경우, 이를 위한 최적의 방식은 무엇일까요?
    A.EC2 사용자 데이터는 bash 스크립트를 사용해 EC2 인스턴스를 부트스트랩 할 경우에 사용됩니다. 이 스크립트에는 소프트웨어/패키지 설치, 인터넷에서 파일 다운로드 등, 여러분이 원하는 작업을 수행하기 위한 명령어를 포함시킬 수 있습니다.

##### Q.인메모리 데이터베이스를 사용하는 중요 애플리케이션을 위해서는 다음 중 어떤 EC2 인스턴스 유형을 선택해야 할까요?
    A.메모리 최적화 EC2 인스턴스는 메모리에 대규모 데이터 세트가 필요한 워크로드에 적합합니다.

##### Q.온프레미스에 호스팅된 OLTP 데이터베이스를 갖춘 전자 상거래 애플리케이션이 있습니다. 이 애플리케이션은 인기가 좋아, 데이터베이스가 초당 수천 개의 요청을 지니게 됩니다. 여러분은 데이터베이스를 EC2 인스턴스로 이전하려 합니다. 이렇게 높은 빈도를 보이는 OLTP 데이터베이스를 처리하기 위해서는 어떤 EC2 인스턴스 유형을 선택해야 할까요?
    A.스토리지 최적화 EC2 인스턴스는 로컬 스토리지의 대규모 데이터 세트에 대해 높은 수준의, 그리고 순차적인 읽기/쓰기 액세스 권한이 필요한 워크로드에 적합합니다.

##### (참/거짓) 보안 그룹은 오직 하나의 EC2 인스턴스에만 연결될 수 있습니다. (X)

##### Q.온프레미스 애플리케이션을 AWS로 이전하려 합니다. 여러분의 기업에는 애플리케이션을 전용 서버에서 실행해야 한다는 엄격한 규정이 있습니다. 또한 비용 절감을 위해 전용 서버 바운드 소프트웨어 라이선스를 사용해야 합니다. 이 경우, 다음 중 어떤 EC2 구매 옵션이 적합할까요?
    A.전용 호스트는 높은 수준의 규정 준수가 필요한 기업, 혹은 복잡한 라이선스 모델을 가진 소프트웨어에 적합합니다. 이는 가장 비싼 EC2 구매 옵션입니다.

##### Q.데이터베이스 기술을 EC2 인스턴스에 배포하려 합니다. 공급 업체 라이선스는 물리적 코어 및 기반 네크워크 소켓 가시성를 기반으로 비용을 책정합니다. 이 경우, 어떤 EC2 구매 옵션을 사용해야 가시성을 확보할 수 있을까요?
    A.전용호스트

##### Q.EC2 인스턴스 플릿에서 대규모의 데이터 분석을 수행하는 애플리케이션이 있습니다. 여러분은 EC2 인스턴스들이 서로 소통하면서도 가장 높은 수준의 네트워킹 성능을 유지했으면 합니다. 이런 경우, 다음 중 어떤 EC2 배치 그룹을 선택해야 할까요?
    A.클러스터 배치 그룹을 사용하면 EC2 인스턴스들이 나란히 위치하게 되어 고성능의 컴퓨팅 및 네크워킹 성능을 제공하게 됩니다.

##### Q.EC2 인스턴스 플릿에 호스팅된 중요 애플리케이션이 있습니다. 이 애플리케이션에서 AZ 실패가 일어난 경우, 최대 가용성을 달성했으면 합니다. 이런 경우, 다음 중 어떤 EC2 배치 그룹을 선택해야 할까요?
    A.분산 배치 그룹은 EC2 인스턴스를 여러 AZ에 걸쳐 서로 다른 물리적 하드웨어에 배치합니다.

##### Q.탄력적 네트워크 인터페이스(ENI)는 다른 AZ에 있는 EC2 인스턴스와 연결될 수 있습니다. (x) 


Access
IAM ( Identity and Access Management ) ⭐️⭐️⭐️⭐️⭐️
📌
인증 및 권한 관리 서비스
Roles
📌
사용자, 서비스에 대한 액세스 권한 관리 Policy의 집합
Policy
📌
사용자, 서비스에 대한 권한 부여
Group
📌
여러 사람에게 동일한 액세스 권한 부여 및 관리
User
📌
말 그대로 AWS 계정 하나하나
Cognito 
📌
사용자 인증 및 권한 부여를 위한 서비스
웹 및 모바일 애플리케이션에서 사용자 인증과 권한 부여를 쉽게 구현 가능
완전 관리형 서비스
사용자 계정 관리, 인증, 권한 부여 및 동기화를 위한 API와 SDK를 제공
SAML 및 OAuth와 같은 표준 기반 프로토콜 지원
MFA, 사용자별 패스워드 정책, 비밀번호 해시와 같은 보안 기능 제공
Amazon Cognito User Pools 및 Amazon Cognito Identity Pools 두 가지 유형 제공
Directory Service
📌
AWS에서 제공하는 관리형 디렉터리 서비스
온프레미스와 AWS 클라우드 리소스간의 하이브리드 환경에서 Microsoft Active Directory를 호스팅
관리형 AD ( Active Directory )
AWS에서 AD 관리와 유지보수를 대신해줌
AWS Managed Microsoft AD, AD Connector, Simple AD 3가지 타입으로 제공
Control Tower
📌
AWS 계정, VPC 및 계정 중앙화 서비스를 자동화하고 통합하여 AWS 최적화를 지원하는 서비스
 멀티 계정 환경에서 AWS 리소스를 안전하게 설정하고 준수 규정을 준수할 수 있습니다.
멀티 AWS 계정 구성
AWS 리소스의 보안 구성
AWS 리소스 준수 규정 준수
계정 모니터링 및 보안 관리
