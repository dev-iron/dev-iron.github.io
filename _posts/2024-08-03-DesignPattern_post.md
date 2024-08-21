---
title: 디자인 패턴 (Design Pattern) 이란?
date: 2024-08-03 20:00:00 +09:00
categories: [소프트웨어 공학]
tags: [cs, design pattern, se]     # TAG names should always be lowercase
---

안녕하세요. 오늘은 디자인 패턴에 대해 정보를 기록해보겠습니다.

## 디자인 패턴이란?
- - -
디자인 패턴(Design Pattern)은 소프트웨어 설계에서 반복적으로 나타나는 문제를 해결하기 위한 일종의 템플릿입니다. 이는 객체 지향 프로그래밍의 특성을 최대한 활용하여 효율적이고 재사용 가능한 소프트웨어를 설계하기 위한 방법론을 제공합니다.

디자인 패턴은 오랜 시간 동안 축적된 경험과 지식을 바탕으로 특정 문제를 해결하기 위한 검증된 방법론입니다. 소프트웨어 개발에서 디자인 패턴은 반복적으로 발생하는 문제에 대한 해결책을 제공하는 검증된 접근 방법을 제공합니다. 다양한 상황에서 효과적으로 문제를 해결하기 위해, 패턴은 그 해결책을 문서화하여 개발자들이 매번 새로운 방법을 고민하지 않고도 효율적으로 문제를 해결할 수 있게 돕습니다. 즉,  디자인 패턴은 과거의 경험과 노하우를 바탕으로 동일한 문제를 해결하는 데 도움을 주는 설계의 '검증된 해법'이라 할 수 있습니다.   

<br>  

## 디자인 패턴의 목적
- - - 
디자인 패턴의 목적은 소프트웨어 설계에서 반복적으로 발생하는 문제를 검증된 방법으로 해결하고, 코드의 재사용성과 유지보수성을 높이며, 설계의 유연성을 제공하는 것입니다.  

- 재사용성 증대 : 코드를 재사용 가능하게 하여 개발 시간을 줄이고 유지 보수를 쉽게 합니다.  
- 표준화 : 개발 팀 간에 공통의 용어와 이해를 형성하여 커뮤니케이션을 원활하게 합니다.  
- 유연성 증가 : 설계의 유연성을 높여 변경에 더 쉽게 대응할 수 있도록 합니다.  
- 효율성 향상 : 검증된 설계 방식을 사용하여 개발 프로세스를 최적화합니다.  

<br>  

**디자인 패턴의 특징**
- - -
재사용 가능성: 패턴은 다양한 상황에서 재사용할 수 있습니다.
캡슐화: 특정 설계 문제를 해결하는 데 필요한 구현을 캡슐화합니다.
유연성: 코드의 구조를 유연하게 설계할 수 있도록 도와줍니다.
확장성: 새로운 요구사항에 맞게 쉽게 확장할 수 있습니다.

<br>  

## 객체 지향의 특성과 설계 원칙 그리고 디자인 패턴
- - -
**객체 지향 프로그래밍의 주요 특성**
- 캡슐화: 데이터와 메소드를 하나의 객체로 묶고, 외부에서는 이를 접근할 수 있는 공개 인터페이스만을 제공합니다.
- 상속: 기존 클래스의 속성과 메소드를 확장하여 새로운 클래스를 생성합니다.
- 다형성: 동일한 인터페이스를 통해 서로 다른 구현을 사용할 수 있습니다.
- 추상화: 구체적인 구현보다는 인터페이스나 추상 클래스를 통해 설계합니다.


**설계 원칙**
- SOLID 원칙: 단일 책임 원칙(SRP), 개방-폐쇄 원칙(OCP), 리스코프 치환 원칙(LSP), 인터페이스 분리 원칙(ISP), 의존성 역전 원칙(DIP)
- DRY 원칙: 중복을 피하고 코드의 재사용성을 높입니다.
- KISS 원칙: 설계를 간단하고 명확하게 유지합니다.

<br>  

## GoF 디자인 패턴
- - -
GoF(Gang of Four)는 디자인 패턴의 클래식인 23가지 패턴을 정의한 네 명의 저자를 의미합니다. 이 패턴들은 다음 세 가지 범주로 나뉩니다  

- 생성(Creational) 패턴: 객체 생성과 관련된 패턴
    - 예: 싱글톤, 팩토리 메서드, 추상 팩토리, 빌더, 프로토타입

- 구조(Structural) 패턴: 객체나 클래스를 조합하여 더 큰 구조를 만드는 패턴
    - 예: 어댑터, 브리지, 컴포지트, 데코레이터, 퍼사드, 플라이웨이트, 프록시

- 행동(Behavioral) 패턴: 객체 간의 상호작용 및 책임 분배와 관련된 패턴
  - 예: 책임 연쇄, 커맨드, 인터프리터, 반복자, 중재자, 메멘토, 옵서버, 상태, 전략, 템플릿 메서드, 방문자

<br>  

## 디자인 패턴 특징 



# 생성 패턴 (Creational Patterns)   
특징: 객체 생성의 복잡성을 관리하고, 객체 생성을 유연하게 조정할 수 있도록 돕습니다.
- - -

    싱글톤 패턴 (Singleton Pattern)  
    - 특징: 인스턴스가 오직 하나만 생성되고, 전역적으로 접근할 수 있도록 보장합니다.  
    - 예시: 데이터베이스 연결 객체, 설정 관리 클래스.  


    팩토리 메서드 패턴 (Factory Method Pattern)   
    - 특징: 객체 생성 코드를 서브클래스에서 구현하도록 하여 객체 생성 과정을 클라이언트 코드와 분리합니다.  
    - 예시: 다양한 유형의 버튼을 생성하는 GUI 라이브러리, 다양한 문서 형식을 지원하는 텍스트 편집기.  


    추상 팩토리 패턴 (Abstract Factory Pattern)  
    - 특징: 관련 객체들의 가족을 생성할 수 있는 인터페이스를 제공하고, 구현 클래스를 숨깁니다.  
    - 예시: 플랫폼별 UI 구성 요소를 생성하는 시스템(Windows와 macOS의 버튼, 텍스트 박스 등).  


    빌더 패턴 (Builder Pattern)  
    - 특징: 복잡한 객체를 단계별로 생성할 수 있도록 하고, 생성 과정을 분리하여 가독성을 높입니다.  
    - 예시: 복잡한 HTML 문서를 생성하는 웹 페이지 빌더, 복잡한 자동차 조립.  


    프로토타입 패턴 (Prototype Pattern)  
    - 특징: 기존 객체를 복제하여 새로운 객체를 생성합니다. 객체 생성 비용이 클 때 유용합니다.  
    - 예시: 그래픽 편집기에서 도형 복사, 복제 가능한 객체들(문서 편집기에서 복제된 문서). 
    
<br>
<br>

# 구조 패턴 (Structural Patterns)   
특징 : 클래스와 객체 간의 관계를 정의하고, 구조를 조정하여 더 큰 시스템을 효율적으로 구성합니다.  
- - -

    어댑터 패턴 (Adapter Pattern)   
    - 특징: 서로 호환되지 않는 인터페이스를 연결하여 사용할 수 있도록 합니다.  
    - 예시: 전원 플러그 어댑터, 다양한 파일 포맷을 읽는 프로그램에서의 변환기.   


    브리지 패턴 (Bridge Pattern)   
    - 특징: 구현과 추상화를 분리하여, 둘을 독립적으로 변경할 수 있게 합니다.  
    - 예시: 다양한 형태의 장치와 그 장치에서 사용할 수 있는 기능을 분리한 원격 제어 시스템.  


    컴포지트 패턴 (Composite Pattern)   
    - 특징: 객체를 트리 구조로 구성하여, 부분-전체 계층을 표현하고 통일된 방식으로 처리합니다.  
    - 예시: 파일 시스템의 폴더와 파일, 그래픽 사용자 인터페이스의 복합적인 구성 요소.  


    데코레이터 패턴 (Decorator Pattern)   
    - 특징: 객체에 동적으로 추가적인 기능을 부여하고, 기존 객체의 기능을 확장합니다.  
    예시: GUI 컴포넌트에 추가 기능(스크롤바, 테두리 등)을 추가하는 경우, 파일 객체에 압축 기능 추가.  


    퍼사드 패턴 (Facade Pattern)   
    - 특징: 복잡한 서브시스템에 대해 단순화된 인터페이스를 제공하여 사용하기 쉽게 합니다.  
    - 예시: 복잡한 서브시스템을 단순화하여 사용자에게 제공하는 통합 관리 시스템, 복잡한 오디오 시스템의 단순화된 컨트롤.  


    플라이웨이트 패턴 (Flyweight Pattern)   
    - 특징: 많은 객체를 공유하여 메모리를 절약하고 성능을 향상시킵니다.  
    - 예시: 그래픽 렌더링에서 공통 요소를 공유하여 성능을 최적화하는 경우, 문서 편집기의 문자 객체.  


    프록시 패턴 (Proxy Pattern)   
    - 특징: 접근 제어, 로깅 등의 목적으로 대리 객체를 사용하여 실제 객체에 대한 접근을 제어합니다.  
    - 예시: 이미지 로딩을 지연시키는 프록시, 네트워크 접근 제어를 위한 대리 객체.  

<br>
<br>


# 행동 패턴 (Behavioral Patterns)  
특징 : 객체 간의 상호작용과 책임 분배를 정의하여, 복잡한 동작을 관리하고 유연성을 제공합니다.  
- - -

     책임 연쇄 패턴 (Chain of Responsibility Pattern)   
    - 특징: 요청을 처리할 수 있는 객체들을 연결하여 요청을 처리하고, 요청이 처리될 때까지 계속 전달합니다.  
    - 예시: 로깅 시스템에서 다양한 로거 객체를 체인으로 연결하여 로그를 기록하는 경우.  
<br>

     커맨드 패턴 (Command Pattern)   
    - 특징: 요청을 객체로 캡슐화하여 호출자와 수신자를 분리하고, 요청을 저장하거나 되돌릴 수 있습니다.  
    - 예시: 원격 제어 시스템에서 다양한 명령을 객체로 캡슐화하여 실행, 취소, 재실행을 지원하는 경우.  
<br>

     인터프리터 패턴 (Interpreter Pattern)   
    - 특징: 특정 언어의 문법을 정의하고 해석하여, 문장을 실행하거나 평가합니다.  
    - 예시: 수학 식이나 명령어를 해석하고 실행하는 해석기, DSL(Domain-Specific Language) 구현.  
<br>

     반복자 패턴 (Iterator Pattern)   
    특징: 집합체의 내부 요소를 순회할 수 있는 방법을 제공하여, 집합체의 내부 구조를 노출하지 않고 순회할 수 있게 합니다.  
    - 예시: 배열, 리스트, 컬렉션의 요소를 순회하는 반복자 구현.  
<br>

     중재자 패턴 (Mediator Pattern)   
    - 특징: 객체 간의 상호작용을 중앙에서 관리하여, 객체 간의 직접적인 의존성을 줄이고 복잡성을 감소시킵니다.  
    - 예시: UI 컴포넌트 간의 상호작용을 조정하는 중앙 제어 객체, 다양한 시스템 간의 메시지 전달 조정.  
<br>

     메멘토 패턴 (Memento Pattern)   
    - 특징: 객체의 상태를 저장하고, 이후에 저장된 상태로 복원할 수 있도록 합니다.  
    - 예시: 텍스트 편집기에서 undo/redo 기능을 지원하는 경우, 게임에서 저장된 상태로 복원하는 기능.  
<br>

     옵서버 패턴 (Observer Pattern)   
    - 특징: 객체의 상태 변화 시, 이를 관찰하는 다른 객체들에게 알림을 전달합니다.  
    - 예시: 뉴스 구독 시스템에서 뉴스 기사의 업데이트 시 구독자에게 알림을 보내는 경우.  
<br>

     상태 패턴 (State Pattern)   
    - 특징: 객체의 상태에 따라 행동을 변경하고, 상태 전이를 관리합니다.  
    - 예시: 게임 캐릭터의 상태에 따라 행동을 달리하는 경우, 상태 기반의 UI 상태 관리.  
<br>

     전략 패턴 (Strategy Pattern)   
    - 특징: 알고리즘을 캡슐화하여 서로 교환할 수 있게 하고, 클라이언트에서 알고리즘을 선택할 수 있도록 합니다.  
    - 예시: 다양한 정렬 알고리즘을 제공하는 정렬기, 다양한 전략을 사용하는 게임 AI.  
<br>

     템플릿 메서드 패턴 (Template Method Pattern)   
    - 특징: 알고리즘의 골격을 정의하고, 서브클래스에서 세부 구현을 담당하도록 합니다.  
    - 예시: 데이터 처리의 기본 절차를 정의하고, 구체적인 처리 방식은 서브클래스에서 구현하는 경우.  
<br>

     방문자 패턴 (Visitor Pattern)   
    - 특징: 객체 구조를 변경하지 않고 새로운 기능을 추가할 수 있도록 합니다.  
    - 예시: 객체 구조를 탐색하며 각 객체에 특정 작업을 수행하는 경우, 문서의 다양한 요소에 대한 처리 기능 추가.  


<br> 

## 소프트웨어 설계 과정에서의 디자인 패턴
- - - 

**이 부분은 필자가 디자인 패턴을 공부할 때, 소프트웨어 설계에서 디자인 패턴이 실제로 어떤 단계에서 적용되는지 파악하는 데 어려움을 겪었기에, 이를 명확히 하고자 글을 기록합니다. 디자인 패턴의 정의와 종류, 특징을 배우는 것도 중요하지만, 많은 사람들이 디자인 패턴이 소프트웨어 설계의 각 단계에서 어떻게 적용되는지 이해하는 데 어려움을 겪고 있습니다. 따라서, 전체 설계 과정과 디자인 패턴의 실제 적용 방법을 구체적으로 정리하여 보다 명확한 이해를 돕고자 합니다.**

<br>

**다음은 소프트웨어 설계 과정에서 디자인 패턴이 적용되는 단계와 그 역할에 대한 설명입니다.**

1. **요구사항 분석** : 시스템의 요구사항을 수집하고 분석합니다. 이 단계에서는 디자인 패턴의 필요성을 미리 파악하기 위해 문제의 본질과 요구되는 기능을 명확히 정의합니다.

2. **시스템 설계** : 시스템의 전체 아키텍처와 주요 컴포넌트를 설계합니다. 이 단계에서는 시스템의 구조를 정의하고, 각 컴포넌트 간의 관계를 설정합니다. 디자인 패턴은 시스템의 아키텍처 설계에 필요한 다양한 패턴을 도입하여 시스템의 복잡성을 관리합니다.

3. **객체 설계** : 객체 간의 관계와 상호작용을 설계합니다. 이 단계에서 디자인 패턴은 객체의 책임과 역할을 명확히 하고, 객체 간의 상호작용을 효율적으로 설계하는 데 도움을 줍니다. 특히 객체 간의 협력과 상호작용을 정의하는 데 중요한 역할을 합니다.

4. **디자인 패턴 적용** : 반복적으로 발생하는 설계 문제를 해결하기 위해 적절한 디자인 패턴을 적용합니다. 이 단계에서는 구체적인 설계 문제를 해결하기 위해 다양한 디자인 패턴을 적용하여 설계의 유연성과 재사용성을 높입니다. 패턴은 특정 문제에 대한 검증된 해결책을 제공하며, 코드의 품질과 유지보수성을 향상시킵니다.

5. **구현** : 설계를 바탕으로 코드를 작성합니다. 이 단계에서 디자인 패턴의 적용이 잘못된 경우, 코드가 복잡해지거나 유지보수가 어려워질 수 있으므로, 설계 단계에서의 패턴 적용이 중요합니다.

6. **테스트** : 코드의 기능을 검증하고 오류를 수정합니다. 디자인 패턴을 사용하면 설계가 잘 구조화되어 있으므로, 테스트 단계에서의 오류를 식별하고 수정하는 과정이 효율적입니다.

7. **유지보수** : 소프트웨어를 운영하면서 발생하는 문제를 수정하고 개선합니다. 디자인 패턴은 설계의 유연성을 높여, 변경 사항에 쉽게 대응할 수 있도록 하며, 유지보수 단계에서의 작업을 더 수월하게 합니다.

**정리**  
**디자인 패턴은 주로 객체 설계 단계에서 적용되지만, 시스템 설계와 구현 단계에서도 중요한 역할을 합니다. 패턴을 통해 설계 문제를 사전에 해결하고, 이후 단계에서의 효율적인 작업을 지원하며, 소프트웨어의 전반적인 품질을 높이는 데 기여합니다.**