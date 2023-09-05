<img src="https://companieslogo.com/img/orig/MDB_BIG-ad812c6c.png?t=1648915248" width="50%" title="Github_Logo"/> <br>


# MongoDB Atlas Handson Workshop for LGU Plus

### Pre Work

#### Login to Atlas
주어진 계정으로 Atlas에 로그인을 합니다.
최초 MFA 설정 화면이 나오며 Remind me later를 클릭 합니다.

<img src="/00.pre-work/images/images10.png" width="90%" height="90%">  

로그인 완료 후 계정 정보를 클릭 합니다. 계정 정보에 Invitations가 1개 도착 된 것을 볼 수 있으며 이를 클릭 하여 줍니다.    

<img src="/00.pre-work/images/images11.png" width="90%" height="90%">  

Invitation 을 Accept 하여 줍니다.     

<img src="/00.pre-work/images/images12.png" width="90%" height="90%">  

이후 All cluster를 클릭 하면 demo 클러스터가 배포 된 것을 확인 할 수 있습니다.   

<img src="/00.pre-work/images/images13.png" width="90%" height="90%">  


#### Database Account 생성
Atlas 데이터베이스 클러스터를 접근하기 위한 계정 생성으로 Security 메뉴에 Database Access를 클릭 하여 계정을 생성 할 수 있습니다.    
Hands-on에서는 Id/password를 이용하는 방식의 데이터베이스 계정을 생성 합니다.   
<img src="/00.pre-work/images/images08.png" width="90%" height="90%">  
계정은 atlas-account로 하여 생성 합니다. Built-in Role 은 편의상 Read and Write to any database 를 선택합니다.

#### Network Access 생성
데이터 베이스 접근 테스트를 위해서 접근 하려는 컴퓨터의 IP 주소를 방화벽에 허용 해 주어야 합니다.    
Security의 Network Access메뉴를 선택 합니다.
<img src="/00.pre-work/images/images05.png" width="80%" height="80%">  
Add IP Address를 클릭하고 Add IP Access List Entry 에서 Add current IP Address를 클릭하하고 Confirm을 선택 합니다.   
방화벽 설정은 1분 가량의 시간이 소요 됩니다.


#### 초기 데이터 로드
생성된 데이터 베이스 클러스터에 초기 샘플 데이터를 적재하여 Hands on을 진행 합니다.   
<img src="/00.pre-work/images/images06.png" width="90%" height="90%">     


Database 메뉴를 클릭 하면 생성된 데이터 베이스 클러스터를 볼 수 있습니다. 최초에는 데이터가 없음으로 클러스터 메뉴 버튼을 "..."을 클릭 하면 추가 메뉴 중 Load Sample Dataset 을 선택 합니다.   
생성이 완료된 후 Browse Collections를 클릭하먄 데이터를 볼 수 있습니다.
생성된 데이터 베이스는 sample_airbnb외 8개의 데이터베이스가 생성 되고 최소 1개 이상의 컬렉션(테이블)이 생성되게 됩니다.
<img src="/00.pre-work/images/images07.png" width="90%" height="90%"> 


#### 기타 필요한 소프트웨어
클라이언트 애플리케이션 테스트를 위한 Nodejs 필요합니다.
MongoDB에 접속하고 데이터를 조회 하는 GUI Tool (Compass)를 다운로드 합니다.

Nodejs : 
https://nodejs.org/en/download/

Compass :   
https://www.mongodb.com/products/compass

Mongosh :
https://www.mongodb.com/docs/mongodb-shell/install/

