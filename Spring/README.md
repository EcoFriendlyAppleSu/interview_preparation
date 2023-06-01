# Spring Framework

<details>
<summary style="font-size:20px">@SpringBootTest vs @DataJpaTest</summary>
<div markdown="1">
<br></br>
<h3>@SpringBootTest vs @DataJpaTest</h3>

- SpringBootTest는 통합 테스트 시 사용되며 Application Context를 로드하고 테스트 실행에 필요한 설정을 제공합니다.

- DataJpaTest는 Spring Data JPA Repository의 단위 테스트를 작성할 때 사용되는 Annotation입니다. 통합 테스트처럼 모든 Context를 등록하는 것이 아닌 필요한 Repository의 Bean만 등록해 사용하기 때문에 Test Slicing이 가능합니다.

<h3>❓ 둘은 무슨 차이가 있나요?</h3>

✅ SpringbootTest : @Transactional이 존재하지 않아, 매 번 롤백시켜주지 않고 각 테스트의 영향이 다른 테스트에 끼칠 수 있습니다.

✅ DataJpaTest : @Transcational이 존재해 매 번 테스트가 실행될 때마다 Rollback이 실행됩니다.

<h3>❓ 그렇다면 @SpringBootTest와 @Transactional을 같이 사용하면 되는거 아닌가요?</h3>

✅ 사용해도 되는데 그렇게된다면 Product Code Level에서 Transactional 경계가 설정된 것처럼 보입니다. 이것은 코드스멜을 야기할 수 있습니다. 따라서, 정확히 알고 사용해야합니다.
</div>
</details>


<details>
<summary style="font-size:20px">@Transactional</summary>
<div markdown="1">
<br></br>
<h3>SpringFramework @Transactional vs Javax @Transactional</h3>

- 크게 적용 범위와 관리 범위의 차이를 갖고 있습니다.

<h3>✅ Spring Framework @Transactional</h3>

- 적용 범위 : 클래스 수준과 메서드 수준에서 사용할 수 있습니다. 클래스 수준에서 사용할 경우 모든 메서드에 적용됩니다.

- 관리 범위 : Spring의 Transaction 관리자와 통합되어 작동합니다. Spring은 Runtime에 Proxy를 생성하여 Transaction 관리를 수행합니다.

<h3>✅ Javax @Transactional</h3>

- 적용 범위 : 메서드 수준에서만 사용할 수 있습니다.

- 관리 범위 : Java EE Container의 Transaction 관리자와 통합되어 작동합니다. Java EE Container는 Transaction 관리를 수행하고 메서드 실행 전후에 필요한 Transcation 처리를 수행합니다.


<br></br>

<h3>Spring Framework를 사용하면 Framework에서 제공하는 Annotation을 사용하는 것이 유리하다는 것을 알았습니다.</h3>

<br></br>


<h3>❓ JPA와 함께 사용됐을 때 어떻게 동작하나요?</h3>

- JPA 최초 조회 시 원본 데이터 SnapShot을 갖고 Persistence Context에 저장합니다.

- @Transaction이 걸린 Method에선 Entity의 변경이 이뤄질 때마다 Dirty Checking이 발생하게 됩니다.

- 끝으로 Transaction이 정상적으로 종료되면 최종적으로 값이 변경되고 그렇지 않다면 Rollback이 됩니다.

<h3>❓ Transactional(readOnly = true or false)는 무엇인가요? </h3>

- readOnly가 true라면 읽기 전용으로 인식되고 CUD 동작을 하지 않고 조회만 가능합니다.

- 위와같이 사용하면 **조회만 진행하기 때문에 1차 캐시에 저장해야 할 SnapShot을 하지 않아도 되어 성능이 향상**되는 이점을 가질 수 있습니다.

  - 추가로, CQRS Pattern에 적용해 사용할 수 있습니다. 
  - readOnly 조건을 잘 사용한다면 Command 용 Service와 Query 용 Service로 책임을 분리할 수 있습니다.
    - 나아가, DB에 대한 End Point를 구분할 수 있습니다. Master DB(CUD) - Slave DB(Read) -> **장애격리를 할 수 있는 좋은 포인트**가 됩니다.

<h3>🙏🏻 Tip</h3>

- Method 전체에 Transactional를 두고 관리한다면 Human Error가 발생할 수 있습니다.
  
- 때문에 Class 위해서 readOnly = true 선언 후 CUD 작업에선 Transactional을 추가적으로 작업하는 것이 좋습니다.

</div>
</details>

<details>
<summary style="font-size:20px">@WebMvcTest</summary>
<div markdown="1">
<br/>
<h3>WebMvcTest란</h3>

- '@WebMvcTest'는 스프링 MVC Controller의 단위 테스트를 위해 사용됩니다. 이 Annotation을 사용하면 Web 계층에 집중된 테스트를 수행할 수 있습니다.

- '@WebMvcTest'는 Controller의 동작을 테스트하고, Controller와 관련된 Bean들만 로드됩니다. 따라서, Controller의 요청 처리, 응답 상태 코드, View와 Model의 검증 등과 같은 Web 계층에 특화된 테스트를 작성할 수 있습니다.

<h3>❓ WebMvcTest를 사용해서 얻을 수 있는 이점이 있나요?</h3>

- Presentation 계층에서의 테스트를 위해 필요한 최소한의 구성 요소만 로드되어 테스트 시간이 짧고 외부 의존성이 없으므로 테스트 범위가 좁아집니다.
</div>
</details>