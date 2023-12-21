# awsSaaSummary

## IAM 및 AWS CLI
## EC2 기초
## EC2 솔루션스 아키텍트 어소시에이트 레벨
## EC2 인스턴스 스토리지
## 고가용성 및 스케일링성 ELB 및 ASG
## AWS 기초 RDS + Aurora + Elasticashe
## Route 53
## 클래식 솔루션 아키텍처 토론
## Amazon S3 소개
## 고급 Amazon S3
## 아마존 S3 보안
## CloudFront 및 AWS 글로벌 엑셀러레이터
## AWS 스토리지 추가 기능
## 디커플링 애플리케이션 SQS, SNS, Kinesis, Active MQ
## AWS의 컨테이너 ECS, Fargate, ECR 및 EKS
## 솔루션 설계자 관점의 서버리스 개요
## 서버리스 솔루션 아키텍처 토론
## AWS의 데이터베이스
## 데이터 & 분석
## 머신러닝
## AWS모니터링 및 감사 CloudWatch, CloudTrail 및 Config
## Identity and Access Management (IAM) 고급
## AWS보안 및 암호화 KMS, SSM Parameter Store, CloudHSM, Shield, WAF
## 네트워캉- VPC
## 재해 복구 및 마이그레이션
## 더 많은 솔루션 아키텍처
## 기타 서비스
## 백서 및 아키텍처 - AWS공인 솔루션스 아키텍트 어소시에이트

### IAM = Identity and Access Management, Global service

### 인바운드 규칙은 외부에서 Ec2 인스턴스로 연결할 수 있게 해주는 규칙

### SSH는 터미널이나 명령줄을 이용해서 원격 머신이나 서버를 제어할 수 있게 해줌

### EC2 인스턴스 connect ssh와 같은 방식으로 웹에서 빠르게 연결가능한 connect

### Q.EC2 인스턴스에 고성능 컴퓨팅(HPC) 애플리케이션을 배포하려 합니다. 다음 중 어떤 EC2 인스턴스 유형을 선택해야 할까요?
                   A.컴퓨팅 최적화 EC2 인스턴스는 고성능 프로세서(예: 배치 처리, 미디어 트랜스코딩, 고성능 컴퓨팅, 과학적 모델링 및 머신 러닝, 전용 게이밍 서버 등)가 필요한 집중 컴퓨팅 워크로드에 적합합니다.

### Q.1년 간 지속적으로 서버를 운영할 계획인 애플리케이션의 경우에는 다음 중 어떤 EC2 구매 옵션을 사용해야 할까요?
### A.예약 인스턴스는 장기적인 워크로드에 적합합니다. EC2 인스턴스는 1년, 혹은 3년의 기간으로 예약할 수 있습니다.

### Q.일련의 EC2 인스턴스에 호스팅 될 애플리케이션을 실행하려 합니다. 이 애플리케이션에는 소프트웨어 설치가 필요하며, 최초 실행 중에 일부 OS 패키지를 업데이트해야 합니다. EC2 인스턴스를 실행하려는 경우, 이를 위한 최적의 방식은 무엇일까요?
### A.EC2 사용자 데이터는 bash 스크립트를 사용해 EC2 인스턴스를 부트스트랩 할 경우에 사용됩니다. 이 스크립트에는 소프트웨어/패키지 설치, 인터넷에서 파일 다운로드 등, 여러분이 원하는 작업을 수행하기 위한 명령어를 포함시킬 수 있습니다.

### Q.인메모리 데이터베이스를 사용하는 중요 애플리케이션을 위해서는 다음 중 어떤 EC2 인스턴스 유형을 선택해야 할까요?
### A.메모리 최적화 EC2 인스턴스는 메모리에 대규모 데이터 세트가 필요한 워크로드에 적합합니다.

### Q.온프레미스에 호스팅된 OLTP 데이터베이스를 갖춘 전자 상거래 애플리케이션이 있습니다. 이 애플리케이션은 인기가 좋아, 데이터베이스가 초당 수천 개의 요청을 지니게 됩니다. 여러분은 데이터베이스를 EC2 인스턴스로 이전하려 합니다. 이렇게 높은 빈도를 보이는 OLTP 데이터베이스를 처리하기 위해서는 어떤 EC2 인스턴스 유형을 선택해야 할까요?
### A.스토리지 최적화 EC2 인스턴스는 로컬 스토리지의 대규모 데이터 세트에 대해 높은 수준의, 그리고 순차적인 읽기/쓰기 액세스 권한이 필요한 워크로드에 적합합니다.

### (참/거짓) 보안 그룹은 오직 하나의 EC2 인스턴스에만 연결될 수 있습니다. (X)

### Q.온프레미스 애플리케이션을 AWS로 이전하려 합니다. 여러분의 기업에는 애플리케이션을 전용 서버에서 실행해야 한다는 엄격한 규정이 있습니다. 또한 비용 절감을 위해 전용 서버 바운드 소프트웨어 라이선스를 사용해야 합니다. 이 경우, 다음 중 어떤 EC2 구매 옵션이 적합할까요?
### A.전용 호스트는 높은 수준의 규정 준수가 필요한 기업, 혹은 복잡한 라이선스 모델을 가진 소프트웨어에 적합합니다. 이는 가장 비싼 EC2 구매 옵션입니다.

### Q.데이터베이스 기술을 EC2 인스턴스에 배포하려 합니다. 공급 업체 라이선스는 물리적 코어 및 기반 네크워크 소켓 가시성를 기반으로 비용을 책정합니다. 이 경우, 어떤 EC2 구매 옵션을 사용해야 가시성을 확보할 수 있을까요?
### A.전용호스트

