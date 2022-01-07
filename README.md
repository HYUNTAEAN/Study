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

#MVC

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

