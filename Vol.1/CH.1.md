# CH.1 | 오브젝트와 의존관계

### 스프링 오프젝트의 설계와 구현, 동작원리
---

**DAO:** DB를 사용해 데이터를 다루기 위한 오브젝트  
- **관심사의 분리:** 유지보수의 용이성을 위해 객체의 각 기능을 분리하는 것
  - 중복된 코드를 추출하여 **(extract method)** 독립적인 메소드로 선언


- **template method pattern:** 추상 메소드나 오버라이딩이 가능한 protected 메소드를 사용하여 서브클래스에서 구체적으로 구현하는 **(factory method pattern)**  방법
  - 자바는 클래스의 다중상속을 허용하지 않으므로 사용에 주의
  - 슈퍼클래스를 수정할 경우, 모든 서브클래스의 수정이 필요할 수 있음
  - 기본적인 기능의 메소드를 하나의 DAO 클래스에 한해서만 사용할 수 있어 매 DAO 클래스마다 중복되는 문제가 있음  



### References
---
- https://www.oracle.com/java/technologies/javase/javabeans-spec.html
- https://dololak.tistory.com/133

