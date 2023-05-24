# JPA

<details>
<summary style="font-size:20px">@EnableJpaAuditing</summary>
<div markdown="1">
@EnableJpaAuditing은 어디에 사용되나요?

- '@EnableJpaAuditing'은 Spring Data JPA에서 제공하는 어노테이션으로, JPA 감사(Auditing) 기능을 활성화하는 데 사용됩니다. 이 어노테이션을 사용하면 Entity의 생성일자와 수정일자를 자동으로 관리할 수 있습니다.

@EnableJpaAuditing을 사용했을 때 왜 “JPA metamodel must not be empty!” Message를 내뱉는 것일까요?

- Auditing Annotation을 @SpringBootApplication에 등록해놓고 JPA를 사용하지 않는 Slice Test를 진행할 경우 에러가 발생합니다.

- 이유는 Spring Container를 요구하는 가장 기본이되는 --Application 클래스가 항상 로드 됩니다. Auditing Annotation이 등록되어있다면 모든 테스트들이 항상 JPA관련 Bean들을 필요로 합니다.

- @SpringBootTest를 사용할 때는 전체 Context를 로드하고 JPA를 포함한 모든 Bean을 주입 받기 때문에 에러가 발생하지 않지만, **@WebMvcTest 같은 Slice Test는 JPA관련 Bean들을 로드하지 않기 때문에 에러가 발생**합니다.
</div>
</details>