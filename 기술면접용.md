# JAVA

Collection<br><br>

List <br>
- 1. ArrayList : 배열로 구현된 리스트<br> 
- 2. LinkedList : 다음 노드 주소를 기억하고 있는 리스트(탐색 느림)<br>

Map <br>
- 1. HashMap : Key,Value / 중복없음 순서없음<br>
- 2. TreeMap : Tree구조 Map / 순서 보장<br>
- 3. LinkedHashMap : LinkedList로 구현된 HashMap / 순서 보장, 랜덤 접근 느림<br>

Set <br>
- 1. HashSet : Key값이 없는 집합 / 중복없음 순서없음<br>
- 2. TreeSet : Red-Black Tree Set<br>
- 3. LinkedHashSet : LinkedList로 구현된 HashSet / 순서 보장<br>
     
Stack
- 1. LIFO / Push , Pop <br>
- 2. 배열로 만드는게 유리<br>
- 3. 스택 클래스 생성후 사용<br>

Queue<br>
- 1. FIFO / Poll , Remove<br>
- 2. 링크드 리스트로 만드는게 유리<br>
- 3. 자바에서는 인터페이스(객체 생성 불가)

OOP<br>
- 필요 데이터 추상화 -> 행위를 가진 객체화<br>
- 장점 : 코드 재사용율 높음, 유지보수 간단, 대형 안건에 적합<br>
- 단점 : 느림, 용량이 큼, 설계 힘듬<br>
- 1. 클래스 : 객체 추상화, 메소드로 정의한 것<br>
- 2. 인스턴스 : 실제 메모리에 할당한 클래스 데이터<br>
- 3. 추상화 : 클래스의 중요 정보만 정의하여 표현<br>
- 4. 캡슐화 : 코드 수정 없이 재활용을 목적하여 묶는 것<br>
- 5. 은닉화 : 캡슐 내부를 볼 수 없음<br>
- 6. 상속 : 속성, 메소드를 물려받음<br>
- 7. 다형성 : 변수, 함수명이 상황에 따라 다르게 해석(오버로딩, 오버라이딩)<br>

SOLID<br>
- 1. Single Responsibility Principle 단일 책임 법칙<br>
- 2. Open Close Principle 개방 폐쇄 법칙<br>
- 3. Liskov Substitusion Principle 리스코프 치환 법칙<br>
- 4. Interface Segreation Principle 인터페이스 분리 법칙<br>
- 5. Dependency Inversion Principle 의존성 역전 법칙<br>

AOP<br>
FP<br>
Stream API<br>

# MVC

- 1. Model : 처리되는 데이터, 내부 알고리즘 로직 처리를 수행<br>
- 2. View : 사용자 인터페이스<br>
- 3. Controller : 모델과 뷰를 연결, 사용자 입출력 받음<br>

컴포넌트 <br>

View - JSP, Controller - Java Class, Model - Java Bean<br>

컨테이너 <br>

프레임워크 안에서 인스턴스들의 생명주기 관리, 추가 기능 부여 <br>
의존성 주입을 통해 구성 컴포넌트를 관리함<br>

Dependency Injection<br>

Bean 객체 생성시 수행<br>
흐름<br>
- 요청 URL을 Dispatcher-servlet에 전달 <br>
- Handler Mapping 후 컨트롤러에 전달 <br>
- 컨트롤러가 로직 처리 <br>
- 결과를 ModelAndView 객체 생성 후 담아 Dispatcher-servlet에 전달 <br>
- 전달받을 View 검색을 위해 ViewResolver로 전송 <br>
- 검사후 View로 이동 <br>
- Model 정보로 View를 그린후 Dispatcher-servlet에 전달 <br>
- 클라이언트에게 전송<br>

VO<br>

ReadOnly<br>
DB 레코드에 대응되는 자바 클래스 <br>
불변 <br>
Network Traffic 이 감소함 <br>

DTO<br>

전송용 객체 <br>
VO와 거의 동일? 차이점에 대해 설명이 어렵네 ㅇㄴ <br>

DAO<br>

데이터 접근용 객체 <br>
CRUD 처리 <br>
DB나 매커니즘에 추상 인터페이스를 제공 <br>
인터페이스 -> DAO -> 구현객체 반환 <br>
트랜잭션 간의 오버헤드 감소 <br>

Restful <br>

웹 자원을 HTTP를 통해 직관적으로 전달하기 위한 인터페이스<br>
JSON형식이나 XML형식을 HTTP 프로토콜위에서 통신함 <br>
법칙 <br>
- 1. 자원<br>
- 2. 메소드 (GET POST PUT DELETE만으로 표현)<br>
- 3. 명사만<br>
- 4. 확장자 미포함<br>

AJAX<br>

비동기적 통신 기술 <br>
HTTP 요청시 XMLHttpRequest라는 객체를 생성하여 수행 <br>
1 : open()<br>
2 : send()<br>
3 : recv()<br>
4 : Done<br>

# 운영체제

프로세스 <br>

실행중인 프로그램, 디스크에서 메모리로 적재되어 CPU 자원을 할당받음 <br>
스택, 힙, 데이터, 코드영역 <br>

PCB<br>

프로세스 제어 블록 <br>
주기억장치에 유지 <br>
PCB에 현재 상태 저장 (PID, 상태, 다음 명령어 주소)<br>

PC<br>

프로그램 카운터 <br>
다음 실행될 명령어 주소 저장 레지스터 <br>

캐시 메모리 <br>

CPU 레지스터 <-> 메모리<br>
사이에서 캐싱을 통해 병목현상을 완화시킴 <br>

쓰레드 <br>

프로세스의 작업 실행 단위 <br>
프로세스의 주소, 자원 공유 가능 <br>
스레드 ID , PC, 레지스터 집합, 스택 으로 구성 <br>
각각 스택, PC 레지스터를 받음 <br>
멀티 쓰레드 사용시, 힙 영역 공유로 자원 사용시 동기화 필요 <br>
동기화를 위해 과도한 Lock 사용시 병목현상 <br>

Lock <br>

하드웨어 기반 처리, 임계영역 진입을 위한 증명서 개념 <br>

임계영역 공유 전제 조건 <br>

- 1. 상호배제 
- 2. 진행 (크리티컬 섹션 체크)
- 3. 한정된 대기 (진입횟수 제한)

교착상태 발생 조건 4가지 <br>

- 1. 상호 배제
- 2. 점유 대기
- 3. 비선점
- 4. 순환대기


# 네트워크

HTTP 요청 흐름 <br>

브라우저 -> URL 값 파싱 요청 메세지 생성 -> 웹서버로 전송 <br>
-> OS가 DNS 서버 조회하여 Host이름을 IP주소로 변환<br>
-> 어댑터에서 수신, 패킷속에 저장 -> LAN 어댑터에게 전송 <br>
-> 전기신호로 변환, LAN 케이블로 송출 -> 라우터에서 수신 <br>
-> ISP에게 전달 -> 인터넷으로 들어감 -> 목적지 LAN에 도착 <br>
-> 방화벽 검사 -> 캐시 서버에서 검사 -> 물리적 웹 서버 도착<br>
-> 패킷 추출, 메세지 복원 -> 어플리케이션으로 전송 -> 클라이언트 <br>

Http<br>

평문 통신, TCP/IP 특성상 도청 가능, 통신 상대 미확인 <br>

Https (+SSL)<br>

Http <-> SSL, TLS <-> TCP <br>
대칭키, 공개키 방식 <br>
랜덤 데이터 조합으로 대칭키 생성<br>
공개키로 대칭키를 암호화하여 서버에 전송함 <br>
서버는 비밀키를 통해 복호화<br>

CORS <br>

Cross Origin Resource Sharing <br>
도메인간의 자원 공유 <br>

HTTP Header	Description<br>
Access-Control-Allow-Origin	접근 가능한 URL 설정<br>
Access-Control-Allow-Credentials	접근 가능한 쿠키 설정 (true, false)<br>
Access-Control-Allow-Headers	접근 가능한 헤더 설정<br>
Access-Control-Allow-Methods	접근 가능한 메서드 설정<br>

OSI7 <br>

통신 접속 -> 완료까지의 과정을 7단계로 정의한 국제 통신 표준 규약 <br>

TCP/IP 4계층 <br>

통신에 실제 사용되는 계층 <br>
링크, 네트워크, 트랜스포트, 어플리케이션 <br>
과정을 단계별로 파악하여 문제 발생시 트러블슈팅에 용이 <br>

