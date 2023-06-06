<details>
<summary style="font-size:20px">Transactional이란</summary>
<div markdown="1">
<br/>
<h3>🤔 Transactional은 무엇을 하나요?</h3>

- Transactional은 **하나의 논리적 작업 단위로 수행되는 일련의 작업**을 이야기합니다.
<br/>

<h3>🤔 Transactional 특성은 어떤 것이 있나요?</h3>

- Transactiona이 가져야 하는 특성에는 ACID이 있습니다.

✅ Atomicity: 원자성은 트랜잭션과 관련된 작업들이 부분적으로 실행되다가 중단되지 않는 것을 보장하는 능력이다. 예를 들어, 자금 이체는 성공할 수도 실패할 수도 있지만 보내는 쪽에서 돈을 빼 오는 작업만 성공하고 받는 쪽에 돈을 넣는 작업을 실패해서는 안된다. 원자성은 이와 같이 중간 단계까지 실행되고 실패하는 일이 없도록 하는 것이다.

✅ Consistency: 일관성은 트랜잭션이 실행을 성공적으로 완료하면 언제나 일관성 있는 데이터베이스 상태로 유지하는 것을 의미한다. 무결성 제약이 모든 계좌는 잔고가 있어야 한다면 이를 위반하는 트랜잭션은 중단된다.

✅ Isolation: 고립성은 트랜잭션을 수행 시 다른 트랜잭션의 연산 작업이 끼어들지 못하도록 보장하는 것을 의미한다. 이것은 트랜잭션 밖에 있는 어떤 연산도 중간 단계의 데이터를 볼 수 없음을 의미한다. 은행 관리자는 이체 작업을 하는 도중에 쿼리를 실행하더라도 특정 계좌간 이체하는 양 쪽을 볼 수 없다. 공식적으로 고립성은 트랜잭션 실행내역은 연속적이어야 함을 의미한다. 성능관련 이유로 인해 이 특성은 가장 유연성 있는 제약 조건이다. 자세한 내용은 관련 문서를 참조해야 한다.

✅ Durability: 지속성은 성공적으로 수행된 트랜잭션은 영원히 반영되어야 함을 의미한다. 시스템 문제, DB 일관성 체크 등을 하더라도 유지되어야 함을 의미한다. 전형적으로 모든 트랜잭션은 로그로 남고 시스템 장애 발생 전 상태로 되돌릴 수 있다. 트랜잭션은 로그에 모든 것이 저장된 후에만 commit 상태로 간주될 수 있다.

<h3>❓ Spring Project에서 @Transactional은 어떻게 동작하나요?</h3>

- @Transactional를 통해 DB와의 상호작용이 Transactional으로 묶일 수 있습니다.

1. 메서드가 호출되면 Spring은 Transactional을 시작합니다.
2. 메서드 내에서 수행되는 DB 작업은 Transactional 내에서 실행됩니다. 이러한 작업은 일련의 데이터 변경 작업이 포함될 수 있습니다.
3. 메서드가 성공적으로 완료되면, Spring은 Transaction을 Commit하여 DB의 변경 사항을 영구적으로 반영합니다.
4. 메서드 실행 도중 예외가 발생하면, Spring은 Transaction을 롤백하고 이전 상태로 DB를 되돌립니다. 이는 메서드 내에서 발생한 모든 변경 사항을 취소합니다.

<h3>❓ Transactional을 사용할 때, DataSource 이야기가 많이 나오는데 어떤 상관관계가 존재하나요?</h3>

- DataSource는 Spring에서 DB와의 연결을 관리하는 Interface입니다. Spring은 DataSource Interface를 사용하여 DB ConnectionPool을 구성하고, DB 연결을 관리하며, DB와의 상호작용을 처리합니다.

- DataSource는 DB 연결 설정 및 Transaction 관리 등을 제공합니다. @Transactional 어노테이션과 함께 사용될 때 데이터베이스 연결과 트랜잭션 관리를 담당하는 주요한 요소입니다.

</div>
</details>