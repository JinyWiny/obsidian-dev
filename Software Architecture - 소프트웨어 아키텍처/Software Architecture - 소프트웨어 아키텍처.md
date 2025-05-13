
<h2>개념</h2>
"시스템의 기본 구조로서, 시스템을 구성하는 요소들과 그들 간의 관계 및 외부 환경과의 상호작용을 정의한 것"

-  시스템 구성 및 동작 원리
-  구성 요소 간의 관계 + 시스템 외부 환경과의 관계

<h2> 원칙</h2>
소프트웨어의 설계 및 구현 과정에서 발생하는 <b>"복잡성 관리"</b>하고, <b>"유지 보수와 확장 용이"</b>하게 해주는 지침

<h4>일반 원칙</h4>
><b>Separation of Concerns - 관심사(책임) 분리</b>
  
  시스템의 각 부분을 독립적으로 관리할 수 있도록, 서로 다른 책임을 가진 모듈로 나누는 원칙
  재사용성과 유지보수성 향상

> Modularity - 모듈화

  시스템을 작은 독립된 단위(모듈)로 나누어, 각 모듈이 고유한 기능을 수행하도록 구성하는 원칙
  재사용성과 유지보수성 향상

> Abstraction - 추상화

  시스템을 구성하는 복잡한 요소를 간단하게 표현하는 방법으로, 핵심적인 부분에만 집중하고 불필요한 세부사항은 숨기는 원칙
  직관적인 코드 및 구현의 복잡성 감소

> Encapsulation - 캡슐화

  객체 내부의 상태와 동작을 외부에서 직접 접근할 수 없게 감추고, 필요한 기능만을 공개하여 시스템의 안전성을 높이는 원칙
  데이터 일관성 류지 및 시스템 복잡성 감소

> DRY(Don't Repeat Yourself) - 중복 제거

  코드에서 중복을 피하고, 동일한 로직이나 데이터를 여러 곳에서 사용하지 않도록 만드는 원칙
  간결한 코드 및 수정 시 대상이 적어 유지보수성 향상

> KISS(Keep It Simple, Stupid) - 단순하고 명확하게

  불필요한 복잡함을 피하고, 간단하고 이해하기 쉽게 만드는 원칙
  가독성 향상

> YAGNI(You Aren't Gonna Need It) - 필요 없는 건 미리 만들지 않기

  현재 요구 사항에 필요하지 않은 기능을 미리 구현하지 않는 원칙
  시스템 설계 초기 단계에서부터 필요한 기능만 구현함으로써, 불필요한 코드와 복잡성 감소

<h4>SOLID</h4>
> SRP(Single Responsibility Principle) - 단일 책임 원칙

  클래스나 모듈은 하나의 책임만 가져야 한다는 원칙
  각 클래스가 하나의 기능만 수행하게 하여, 클래스가 변경될 이유가 하나만 있게 만들어 변경에 강한 구조

> OCP(Open-Closed Principle) - 개방-폐쇄 원칙

  시스템은 **확장에는 열려 있어야** 하고, **수정에는 닫혀 있어야** 한다는 원칙
  새로운 기능을 추가할 때 기존 코드를 변경하지 않고, 기존 코드에 영향을 미치지 않도록 새로운 클래스를 추가하는 방식

> LSP(Liskov Substitution Principle) - 리스코프 치환 원칙

  자식 클래스는 부모 클래스를 대체할 수 있어야 한다는 원칙
  자식 클래스가 부모 클래스를 확장할 때 부모 클래스의 기능을 변경하지 않도록 하여, 상속 관계에서의 예측 가능한 동작을 보장

> ISP(Interface Segregation Principle) - 인터페이스 분리 원칙

  한 번에 많은 기능을 제공하는 인터페이스보다는, 클라이언트가 필요로 하는 기능만을 제공하는 작은 인터페이스로 분리해야 한다는 원칙
  불필요한 기능을 가진 인터페이스를 구현하지 않게 되어 간결한 코드

> DIP(Dependency Inversion Principle) - 의존성 역전 원칙

  상위 모듈이 하위 모듈에 의존하는 것이 아니라, **상위 모듈은 추상화된 인터페이스에 의존하고**, **하위 모듈은 그 인터페이스의 구현에 의존해야 한다**는 원칙
  시스템의 의존성을 줄이고, 구현 변경이 시스템에 미치는 영향을 최소화

<h2>종류</h2>
<h4>구조 중심</h4>
- [[Clean(Clean Architecture) - 클린]]
- [[Hexagonal(Ports and Adapters) - 포트-어댑터 패턴]]
- [[Onion(Onion Architecture) - 어니언]]
- [[Layered(Layered Architecture) - 계층형]]
- [[Monolithic(Monolithic Architecture) - 단일체]]
- [[Microkernel(Microkernel Architecture) - 마이크로 커널]]

<h4>분산/서비스 중심</h4>
- [[MSA(Microservice Architecture) - 마이크로 서비스]]
- [[SOA(Service-Oriented Architecture) - 서비스 지향]]
- [[Serverless(Serverless Architecture) - 서버리스]]

<h4>동작/행위 중심</h4>
- [[EDA(Event-Driven Architecture) - 이벤트 기반]]
- [[CQRS(Command Query Responsibility Segregation) - 명령-조회 책임 분리]]

<h4>UI 패턴</h4>
- [[MVC(Model-View-Controller) - 모델-뷰-컨트롤러]]
- [[MVVM(Model-View-ViewModel) - 모델-뷰-뷰모델]]
- [[MVP(Model-View-Presenter) - 모델-뷰-프레젠테이션]]

<h4>도메인 중심</h4>
아키텍처라기보단 설계 철학으로 볼 수 있다.
- [[DDD(Domain-Driven Design) - 도메인 주도]]