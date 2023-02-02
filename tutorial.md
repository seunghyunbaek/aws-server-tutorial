# AWS Tutorial : 서버 만들기

### 서버 만드는 방법
AWS 계정 생성 및 로그인하기
  
  
### 지역을 아시아 태평양(서울) 로 설정하기  
 사는 지역과 가까울수록 속도가 더 빠르다.  
  
  
### EC2 서비스: 인스턴스 생성하기  
 EC2 서비스를 찾아준다. EC2는 클라우드 상의 가상 서버다.  
 인스턴스 시작 누르면 프리티어 가능 서버들 중에 고르면 되는데 여기서는 우분투 18.04 LTS를 선택했다.  
 인스턴스 유형은 t2.micro 를 선택하고 키페어를 생성하고 저장했다. 키페어는 서버에 접속할 때 사용한다.  
 인스턴스 시작하면 상태가 pending으로 나오는데 이는 aws에서 가상으로 서버를 만드는 중임을 나타낸다. 기다리면 running 상태로 변경된다.  
 서버가 만들어지면 이름을 설정해줄 수 있다.  
 
 
### 서버에 접속하기   
 인스턴스 선택 후 연결을 누르면 연결하는 방법에 대해 알려준다.  
 [Putty를 이용하여 연결하는 방법](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/putty.html)  
 

### Putty 간단 설명
 PuttyGen 을 실행 - load 선택 후 .pem 선택 - save private key 누르면 .ppk 파일 생성  
 putty 실행 - Honst Name 입력: ec2 인스턴스의 퍼블릭 IPv4 주소 or 퍼블릭 IPv4 DNS 를 입력 -  Connection > SSH > Auth > Credentials 에서 private key file 에 .ppk 파일 선택 후 Open 하면 실행된다.  
 
