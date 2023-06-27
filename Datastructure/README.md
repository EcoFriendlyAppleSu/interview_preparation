<details>
<summary style="font-size:20px">시간 복잡도와 공간 복잡도</summary>
<div markdown="1">
<br/>
<h2>🤔 시간복잡도와 공간복잡도에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 시간 복잡도와 공간 복잡도는 모두 성능 측정에 요인이 되는 측정값입니다.

- 시간 복잡도는 프로세스 실행 시 소요되는 시간을 의미하며 공간 복잡도는 프로세스 실행 시 사용하는 메모리의 양을 의미합니다.

<h3>GPT의 대답</h3>

- 시간 복잡도와 공간 복잡도는 알고리즘의 효율성을 측정하는 두 가지 주요 방법입니다.

- 시간 복잡도는 알고리즘이 문제를 해결하는 데 걸리는 시간을 측정합니다. 이는 일반적으로 입력 데이터의 크기에 따라 결정되며, 이를 통해 알고리즘이 큰 데이터 세트에 대해 얼마나 잘 확장되는지를 판단할 수 있습니다. 

- 공간 복잡도는 알고리즘이 문제를 해결하는 데 필요한 메모리 양을 측정합니다. 일부 알고리즘은 매우 빠르지만 많은 양의 메모리를 사용할 수 있으며, 이는 제한된 메모리 리소스를 가진 시스템에서는 문제가 될 수 있습니다.

<br/>
<h2>🤔 Big-O, Big-Theta, Big-Omega 에 대해 설명해 주세요.</h2>

<h3>GPT의 대답</h3>

✅ Big-O (O) : 이 표기법은 알고리즘의 최악의 경우의 실행 시간을 표현합니다. 즉, 입력 크기에 따른 알고리즘의 실행 시간의 상한을 나타냅니다.

✅ Big-Theta (Θ) : 이 표기법은 알고리즘의 평균 혹은 일반적인 경우의 실행 시간을 나타냅니다. 즉, 입력 크기에 따른 알고리즘의 실행 시간의 상한과 하한을 모두 만족시키는 경우를 의미합니다.

✅ Big-Omega (Ω) : 이 표기법은 알고리즘의 최선의 경우의 실행 시간을 나타냅니다. 즉, 입력 크기에 따른 알고리즘의 실행 시간의 하한을 나타냅니다.

<br/>
<h2>🤔 다른 것을 사용하지 않고, Big-O를 사용하는 이유가 있을까요?</h2>

<h3>📝 나의 대답</h3>

- 최악의 실행 시간을 표현함으로써 풀고자하는 문제에 적합함을 알 수 있기 때문입니다.

<h3>GPT의 대답</h3>

- Big-O 표기법은 알고리즘의 최악의 경우의 실행 시간을 나타냄으로써, 특정 문제에 대해 알고리즘이 어떻게 수행될 수 있는지에 대한 가장 보수적인 추정을 제공합니다. 이는 **최악의 경우에도 시스템이 어떻게 수행될지 이해하는 것이 중요한 많은 실제 상황에서 유용**합니다.

<br/>
<h2>🤔 O(1)은 O(N^2) 보다 무조건적으로 빠른가요?</h2>

<h3>📝 나의 대답</h3>

- 아니요. 어떤 메모리를 사용하는지가 두 Big-O 결과에 영향을 끼칠 수 있습니다. 만약 알고리즘을 해결할 때 O(1)에서 메모리 스위칭 비용이 많이 O(N^2)보다 많이 발생하게 된다면 O(1)이 더 느릴 수도 있습니다.

<h3>GPT의 대답</h3>

- 아니요, O(1)이 O(N^2)보다 무조건적으로 빠르다고 말할 수 없습니다. Big-O 표기법은 입력 크기에 따른 알고리즘의 실행 시간의 상한을 나타내는 것으로, 입력 크기가 커질수록 O(N^2)은 O(1)보다 더 많은 시간이 소요될 것입니다.

- 그러나 이것은 '항상'이라는 말이 아닙니다. 실제 실행 시간은 알고리즘의 구현, 하드웨어, 데이터 분포 등 많은 다른 요인들에 의해 결정됩니다. 예를 들어, O(1)의 알고리즘이 상당히 큰 상수 시간을 가지거나, O(N^2)의 알고리즘이 매우 작은 입력 크기에 대해 사용될 경우, 실제로는 O(N^2)의 알고리즘이 더 빠를 수 있습니다.

- 또한, 당신이 언급한 것처럼, 메모리 스위칭, 캐시 히트 등의 하드웨어 요인도 실행 시간에 영향을 줄 수 있습니다. 이러한 모든 요인을 고려하면, Big-O 표기법만으로는 실제 실행 시간을 완벽하게 예측할 수 없습니다.

</div>
</details>

<details>
<summary style="font-size:20px">링크드 리스트</summary>
<div markdown="1">
<br/>
<h2>🤔 링크드 리스트에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 링크드 리스트는 자료구조의 하나로 노드의 연결로 구성되어 있습니다. 단일 링크드 리스트, 양방향 링크드 리스트로 구성할 수 있으며 노드 안엔 데이터와 다음 노드의 위치를 담아 연결을 맺습니다.

<h3>GPT의 대답</h3>

- 링크드 리스트의 주요 장점 중 하나는 요소의 삽입과 삭제가 배열에 비해 상대적으로 간단하다는 것입니다. 배열에서는 요소를 삽입하거나 삭제할 때마다 다른 요소들을 이동시켜야 하지만, 링크드 리스트에서는 단순히 몇 개의 포인터를 수정하면 됩니다.

- 그러나, 이런 유연성 때문에 링크드 리스트는 포인터를 통한 노드 접근이 필요하므로, 임의 접근(random access)가 불가능하며, 이는 배열과 비교했을 때의 단점으로 볼 수 있습니다.

<br/>
<h2>🤔 일반 배열과, 링크드 리스트를 비교해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 일반 배열은 메모리에 연속적으로 존재하지만 링크드 리스트는 그렇지 않습니다. 데이터 조회 속도는 일반 배열이 링크드 리스트보다 좋습니다. 이유는 일반 배열의 경우엔 데이터가 연속으로 존재하기 때문입니다. 하지만 중간에 데이터를 삽입, 삭제 시 일반 배열의 경우 삽입, 삭제 기준으로 데이터를 이동시켜야 하기 때문에 링크드 리스트보다 리소스가 많이 소모됩니다.

<h3>GPT의 대답</h3>

- 일반 배열은 메모리의 연속적인 영역에 데이터를 저장합니다. 이로 인해 배열은 인덱스를 통해 임의의 요소에 빠르게 접근할 수 있는 장점이 있습니다. 그러나, 배열의 크기는 선언 시점에서 결정되며, 이후에는 크기를 변경할 수 없습니다. 또한, 배열의 중간에 요소를 삽입하거나 삭제하려면 다른 요소들을 이동시켜야 하므로, 이러한 작업은 비효율적입니다.

- 반면에 링크드 리스트는 메모리의 비연속적인 영역에 데이터를 저장하며, 각 노드가 다음 노드를 가리키는 방식으로 연결됩니다. 이로 인해 링크드 리스트는 동적으로 크기를 조정할 수 있으며, 중간에 요소를 삽입하거나 삭제하는 것이 상대적으로 간단합니다.

- 단지 연결을 끊고 새로 연결하는 것만으로도 가능하기 때문입니다. 그러나 이는 링크드 리스트가 임의 접근을 지원하지 않는다는 단점을 가지고 있습니다. 링크드 리스트에서 특정 요소에 접근하려면 처음부터 순차적으로 접근해야 합니다.

<br/>
<h2>🤔 링크드 리스트를 사용해서 구현할 수 있는 다른 자료구조에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 링크드 리스트로 다양한 자료구조를 구현할 수 있습니다. 스택, 큐, 그래프 등 만들 수 있습니다.

<br/>
<h2>🤔 Array와 LinkedList 장/단점</h2>

<h3>📝 나의 대답</h3>

- Array :  RandomAccess가 가능해 속도가 빠르다는 장점이 있습니다. 하지만 삽입 또는 삭제의 과정에서 각 원소들을 shift 해줘야 하는 비용이 생겨 이 경우 시간 복잡도는 O(n)이 된다는 단점이 있습니다.
  
- 각각의 원소들은 자기 자신 다음에 어떤 원소인지만을 기억하고 있기 때문에 이 부분만 다른 값으로 바꿔주면 삽입과 삭제를 O(1)로 해결할 수 있습니다.
하지만LinkedList는 원하는 위치에 한 번에 접근할 수 없다는 단점이 있습니다. 원하는 위치에 삽입을 하고자 하면 원하는 위치를 Search 과정에 있어서 첫번째 원소부터 다 확인해봐야 합니다.
</div>
</details>

<details>
<summary style="font-size:20px">Stack, Queue</summary>
<div markdown="1">
<br/>
<h2>🤔 스택과 큐에 대해서 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 스택과 큐는 선형 자료구조이며 컴퓨터의 많은 부분에서 사용됩니다. Stack은 LIFO 형태를 갖고 데이터를 처리하며 Queue는 FIFO으로 데이터를 처리합니다.

- 위의 특징 때문에 Stack은 실행 취소, 히스토리 관리, 함수 호출 등의 다양한 알고리즘에서 사용됩니다. Queue는 작업 스케줄링, 이벤트 처리, 캐싱 등의 다양한 알고리즘에서 사용됩니다.

<br/>
<h2>🤔 스택 2개로 큐를, 큐 2개로 스택을 만드는 방법과, 그 시간복잡도에 대해 설명해 주세요.</h2>

<h3>GPT의 대답</h3>

✅ Stack 2개로 Queue를 만드는 방법

1. 2개의 스택을 가지고 하나는 '입력 스택'으로 사용하고, 다른 하나는 '출력 스택'으로 사용합니다.

2. 새로운 요소를 추가할 때는 '입력 스택'에 'push'합니다.

3. 요소를 제거할 때는 '출력 스택'에서 'pop'합니다. 만약 '출력 스택'이 비어 있다면, '입력 스택'의 모든 요소를 '출력 스택'으로 이동시킨 후에 '출력 스택'에서 'pop'합니다.

- 이 방법의 시간 복잡도는 일반적으로 O(1)입니다. 그러나 '출력 스택'이 비어 있을 때 '입력 스택'의 모든 요소를 '출력 스택'으로 이동시키는 연산은 O(N)입니다. 하지만 이런 연산은 각 요소당 한 번만 발생하므로, 각 연산에 대한 평균 시간 복잡도는 여전히 O(1)입니다.

✅ Queue 2개로 Stack을 만드는 방법

1. 2개의 큐를 가지고 하나는 '주 큐', 다른 하나는 '보조 큐'로 사용합니다.
새로운 요소를 추가할 때는 '주 큐'에 'enqueue'합니다.

2. 요소를 제거할 때는 '주 큐'의 요소를 '보조 큐'로 이동시키되, '주 큐'에 마지막으로 남아 있는 요소를 제외하고 모두 이동시킵니다. 그리고 '주 큐'의 마지막 요소를 제거하고, '주 큐'와 '보조 큐'의 역할을 바꿉니다.

- 이 방법의 시간 복잡도는 요소를 추가하는 것은 O(1)이지만, 요소를 제거하는 것은 O(N)입니다. 이는 요소를 제거할 때마다 '주 큐'의 거의 모든 요소를 '보조 큐'로 이동시켜야 하기 때문입니다. 따라서, 이 방법은 스택의 'pop' 연산을 자주 수행해야 하는 경우에는 비효율적일 수 있습니다.

<br/>
<h2>🤔 시간복잡도를 유지하면서, 배열로 스택과 큐를 구현할 수 있을까요.</h2>

<h3>📝 나의 대답</h3>

- 배열로 Stack을 구성한다면 시간복잡도를 유지하면서 구현할 수 있지만 큐를 구현하게 된다면 요소의 삭제 시 O(N)의 배열 원소 이동이 발생하게 되어 시간복잡도를 유지할 수 없습니다.

<h3>GPT의 대답</h3>

- 원형 큐 또는 deque를 사용하면 큐 연산의 시간 복잡도를 O(1)로 유지할 수 있습니다.

<br/>
<h2>🤔 Prefix, Infix, Postfix 에 대해 설명하고, 이를 스택을 활용해서 계산/하는 방법에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Prefix, Infix, Postfix는 전위 처리, 중위 처리, 후위 처리를 이야기하며 전위 처리는 그래프의 왼쪽 먼저 계산을 하고 중위 처리는 하나의 부모 노드 아래 있는 자식 노드를 먼저 처리합니다. 후위 처리는 오른쪽 계산을 먼저 처리하는 것을 의미합니다. 모든 처리 방법에 스택을 사용할 수 있고 연산자를 만나게되면 피연산자를 Pop하여 계산합니다.

<h3>GPT의 대답</h3>

- Prefix, Infix, Postfix는 연산자의 위치에 따라 수식을 표현하는 방법을 나타냅니다. 또한, 그래프 처리와는 관련이 없으며, 스택은 이들 표현을 계산할 때 유용하게 사용됩니다.

- Infix 표현은 흔히 우리가 사용하는 방식으로, 연산자를 피연산자들 사이에 두는 방식입니다. 예를 들어, 2 + 3이라는 식은 Infix 표현입니다.

- Prefix 표현(전위 표기법)은 연산자를 피연산자들 앞에 두는 방식입니다. 위의 예를 Prefix로 바꾸면, + 2 3이 됩니다.

- Postfix 표현(후위 표기법)은 연산자를 피연산자들 뒤에 두는 방식입니다. 위의 예를 Postfix로 바꾸면, 2 3 +이 됩니다.

- Prefix 계산: 우측에서 좌측으로 읽으면서 피연산자를 만나면 스택에 push하고, 연산자를 만나면 스택에서 두 개의 피연산자를 pop하여 연산한 후 결과를 다시 스택에 push합니다. 마지막에 스택에 남는 값이 수식의 결과입니다.

- Postfix 계산: 좌측에서 우측으로 읽으면서 피연산자를 만나면 스택에 push하고, 연산자를 만나면 스택에서 두 개의 피연산자를 pop하여 연산한 후 결과를 다시 스택에 push합니다. 마지막에 스택에 남는 값이 수식의 결과입니다.

<br/>
<h2>🤔 Deque는 어떻게 구현할 수 있을까요.</h2>

<h3>📝 나의 대답</h3>

- Deque는 양방향으로 요소를 넣고 뺄 수 있는 자료구조를 의미합니다.

- Deque는 Linked List로 구현할 수 있습니다.

<h3>GPT의 대답</h3>

- Deque(Double-Ended Queue)는 양쪽 끝에서 삽입과 삭제가 모두 가능한 자료구조를 말합니다. 이를 구현하는 방법은 여러 가지가 있지만, 대표적으로는 Doubly Linked List 또는 동적 배열(Dynamic Array)를 사용할 수 있습니다.
</div>
</details>

<details>
<summary style="font-size:20px">Hash</summary>
<div markdown="1">
<br/>
<h2>🤔 해시 자료구조에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Hash는 Hash Table에 값을 저장하는 자료구조이며 Hash 알고리즘을 통해 Hashing을 수행하고 처리된 값을 key-value로 저장합니다. Hash를 통해 Indexing을 할 수 있어 조회 성능을 높일 수 있고 데이터를 보호해 저장할 수도 있습니다.

<h3>GPT의 대답</h3>

- 해시(Hash)는 임의 크기의 데이터를 고정된 크기의 데이터로 매핑하는 함수입니다. 이를 활용하여 구현한 '해시 테이블'은 키(Key)를 값(Value)에 매핑하는 자료구조를 말합니다.

- 해시 함수는 키를 받아서 고정된 범위의 정수를 반환하며, 이 반환값을 해시 코드, 해시값 혹은 간단하게 해시라고 부르기도 합니다. 이 해시값을 배열의 인덱스로 사용하여 값을 저장하고 검색합니다. 이 과정을 '해싱'이라고 합니다.

- 해시 테이블의 주된 장점은 데이터의 검색(조회) 속도가 빠르다는 점입니다. 이론적으로는 해시 함수와 해시 테이블 크기가 적절하면 O(1)의 시간 복잡도로 데이터를 조회할 수 있습니다. 하지만 해시 충돌(두 개 이상의 키가 같은 해시값을 가질 때 발생)을 해결하는 메커니즘이 필요합니다. 일반적인 해시 충돌 해결 방법에는 '체이닝(Chaining)'과 '오픈 어드레싱(Open Addressing)' 등이 있습니다.

<br/>
<h2>🤔 값이 주어졌을 때, 어떻게 하면 충돌이 최대한 적은 해시 함수를 설계할 수 있을까요.</h2>

<h3>📝 나의 대답</h3>

- Hash Table의 사이즈를 늘리거나 해시 함수의 로직을 통해 다양한 해시 값을 얻을 수 있다면 충돌이 최대한 적은 해시를 만들 수 있습니다.

<br/>
<h2>🤔 해시값이 충돌했을 때, 어떤 방식으로 처리할 수 있을까요.</h2>

<h3>📝 나의 대답</h3>

- 해시 값이 충돌했을 때, 체이닝과 오픈 어드레싱을 통해 해시 충돌을 처리할 수 있습니다. 체이닝은 링그드 리스트 자료구조를 사용해 같은 해시 값을 갖는 데이터를 연결해 해시 충돌을 해결합니다. 오픈 어드레싱은 충돌이 일어나면 다음 주소의 Hash Table에 Hash를 저장하는 방법으로 충돌을 해결합니다.

<h3>GPT의 대답</h3>

- 오픈 어드레싱은 충돌이 발생했을 경우 빈 공간을 찾아 데이터를 저장하는 방법입니다. 이를 위해 선형 탐색, 이차 탐색, 이중 해시 등의 방법이 사용됩니다. 

- 이 방법은 추가적인 메모리 공간 없이 해시 테이블 내에서 충돌을 처리할 수 있다는 장점이 있습니다. 하지만 해시 테이블의 **로딩 팩터(저장된 요소의 수 / 테이블의 크기)**가 커지면 충돌이 빈번하게 발생할 수 있으므로, 이에 따른 재해시(rehashing) 과정이 필요할 수 있습니다.

<br/>
<h2>🤔 본인이 사용하는 언어에서는, 어떤 방식으로 해시 충돌을 처리하나요.</h2>

<h3>📝 나의 대답</h3>

- Java에서는 해시 충돌을 체이닝을 통해 처리합니다. 특정 임계값에 도달하면 Red-Black Tree를 만들어 Hash Value를 관리합니다. 이러한 이유는 링크드 리스트로 만들어진 체이닝은 조회 시 O(N)을 따르게 됩니다. Red-Black Tree로 변경함으로서 O(N)을 O(logN)으로 변경할 수 있습니다.

<br/>
<h2>🤔 Double Hashing 의 장점과 단점에 대해서 설명하고, 단점을 어떻게 해결할 수 있을지 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 이중 해싱을 사용하면 Hashing을 두 번 거쳐 Hash Value를 구하는 것을 이야기합니다. Hashing을 두 번 거치게 된다면 다양한 Hash 값을 구할 수 있어 충돌 횟수가 줄어들 순 있지만 계산이 한 번 더 수행되어 조회 시 성능이 떨어질 수 있습니다.

<h3>GPT의 대답</h3>

- 이중 해싱(Double Hashing)의 장점은 해시 충돌이 발생했을 때, 두 번째 해시 함수를 사용해 새로운 주소를 찾는다는 점입니다. 이 방법은 해시 테이블에서 빈 공간을 보다 효율적으로 활용할 수 있게 해줍니다.

- 그러나 이중 해싱의 단점은 해시 함수를 두 번 계산해야 하므로 연산 비용이 늘어난다는 점입니다. 또한, 잘못 설계된 두 번째 해시 함수는 해시 테이블의 일부 공간만을 사용하게 만들어 테이블의 공간 효율성을 떨어뜨릴 수 있습니다.
</div>
</details>
 
<details>
<summary style="font-size:20px">Tree</summary>
<div markdown="1">
<br/>
<h2>🤔 트리와 이진트리, 이진탐색트리에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 트리 자료구조는 부모 노드와 자식 노드로 이뤄진 자료구조입니다. 이진트리는 하나의 부모 노드 아래에 두 개의 자식만 존재하는 자료구조이며 이진 트리에 완전 이진트리, 편향 이진트리가 존재합니다.

- 이진 탐색트리는 부모 노드보다 값이 작다면 왼쪽에 값을 채우고 크다면 오른쪽에 값을 채워 조회 성능을 높일 수 있는 자료구조입니다.

<br/>
<h2>🤔 그래프와 트리의 차이가 무엇인가요?</h2>

<h3>📝 나의 대답</h3>

- 그래프와 트리 모두 노드를 사용해 각 노드의 연결을 통해 구현할 수 있는 자료구조입니다.

- 그래프는 노드 사이 상하 관계가 존재하지 않고 연경을 중점을 두고 트리는 부모 노드, 자식 노드를 갖습니다.

<h3>GPT의 대답</h3>

- 그래프는 순환이 가능하며 모든 노드는 양방향으로 이동할 수 있습니다. 또한 그래프에는 루트 노드라는 개념이 없습니다.

- 트리는 그래프의 한 종류로, 순환을 허용하지 않고, 모든 노드는 한 방향(부모에서 자식으로)으로만 이동합니다. 트리에는 루트 노드가 있고, 모든 노드는 루트 노드에서 출발한 경로를 통해 도달할 수 있습니다.

<br/>
<h2>🤔 이진탐색트리에서 중위 탐색을 하게 되면, 그 결과는 어떤 의미를 가지나요.</h2>

<h3>📝 나의 대답</h3>

- 중위 탐색을 수행하면 이분탐색 결과와 같습니다. 부모 노드를 기준으로 좌측을 작은 값, 우측을 큰 값을 저장했다고 가정했을 때, 한 쪽을 선택하면 반대 쪽 조회를 수행하지 않아도 됩니다.

<h3>GPT의 대답</h3>

- 이진 탐색 트리의 중위 순회는 오름차순으로 노드를 방문합니다. 즉, 중위 순회를 사용하면 이진 탐색 트리의 모든 요소를 오름차순으로 얻을 수 있습니다.

<br/>
<h2>🤔 이진탐색트리의 주요 연산에 대한 시간복잡도를 설명하고, 왜 그런 시간복잡도가 도출되는지 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 이진 탐색 트리는 탐색 시 기본적으로 O(logN)의 성능을 갖습니다. 하지만 주어진 값들이 한쪽으로만 편향된 트리를 갖는다면 이는 조회 시 O(N)의 성능을 갖게 됩니다.

<h3>GPT의 대답</h3>

- 탐색(Search): 이진 탐색 트리에서 특정 노드를 탐색하는 데 필요한 시간 복잡도는 O(logN)입니다. 이는 트리가 균형 잡힌 경우를 가정했을 때입니다. 이진 탐색 트리는 각 노드의 왼쪽 하위 트리에는 노드보다 작은 값들이, 오른쪽 하위 트리에는 노드보다 큰 값들이 저장되는 구조이므로, 탐색할 값과 노드의 값을 비교하여 탐색 방향을 결정할 수 있습니다. 이러한 과정을 통해 탐색 범위를 반으로 줄여나가므로 logN의 시간 복잡도가 나옵니다.

- 삽입(Insertion) 및 삭제(Deletion): 삽입 및 삭제 연산 또한 이진 탐색 트리에서는 O(logN)의 시간 복잡도를 가집니다. 삽입의 경우, 삽입할 위치를 찾는 것이 탐색 과정과 같으므로 logN의 시간 복잡도를 가지며, 삭제의 경우에도 삭제할 노드를 찾는 과정이 탐색과 동일하기 때문입니다. 다만, 삭제할 노드가 두 개의 자식 노드를 가지는 경우, 삭제 후 트리의 속성을 유지하기 위해 추가적인 작업이 필요하며, 이 작업에는 최악의 경우 O(logN)의 시간이 소요됩니다.

- 하지만, 주어진 트리가 균형 잡혀있지 않고 한쪽으로 편향되어 있다면 위의 연산들은 모두 O(N)의 시간 복잡도를 가지게 됩니다. 트리가 한쪽으로 편향되어 있다면 각 연산마다 거의 모든 노드를 방문해야 할 수 있기 때문입니다. 이를 해결하기 위해 균형 이진 탐색 트리(AVL 트리, Red-Black Tree 등)와 같은 자료구조를 사용하기도 합니다.

<br/>
<h2>🤔 이진탐색트리의 한계점에 대해 설명해주세요.</h2>

<h3>📝 나의 대답</h3>

- 편향된 탐색 그래프를 그릴 땐 기대한 O(logN)의 성능이 아닌 O(N)의 성능을 보여주기 때문입니다.

<br/>
<h2>🤔 이진탐색트리의 값 삽입, 삭제 방법에 대해 설명하고, 어떤식으로 값을 삽입하면 편향이 발생할까요.</h2>

<h3>📝 나의 대답</h3>

- 이진 탐색 트리에 값을 삽입, 삭제를 할 땐, 해당 값을 조회 후 삽입 혹은 삭제할 위치를 찾습니다. 데이터를 삽입 혹은 삭제 후 자식 노드가 존재한다면 정렬을 수행하게 되는데 이 때 O(logN)의 실행 복잡도를 갖습니다.

<h3>GPT의 대답</h3>

- 트리가 편향되는 경우는 주로 입력 **데이터가 이미 정렬되어 있거나 거의 정렬되어 있는 경우**입니다. 이런 경우에는 모든 값이 한쪽 방향으로만 삽입되어 트리가 한 방향으로만 길게 늘어나게 되며, 이는 결국 트리가 편향되게 됩니다. 이 경우 BST의 효율성이 크게 떨어지며, 이를 피하기 위해 균형 이진 탐색 트리를 사용합니다.

</div>
</details>

<details>
<summary style="font-size:20px">Heap</summary>
<div markdown="1">
<br/>
<h2>🤔 힙에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Heap은 우선순위큐를 구현한 구현체이며 우선순위큐는 Heap의 ADT입니다. 우선순위큐는 루트 노드에 최대값 혹은 최소값을 가지며 완전 이진 트리를 구성합니다.

<h3>GPT의 대답</h3>

- Heap은 우선순위 큐를 구현하는 하나의 데이터 구조입니다. 따라서 Heap은 우선순위 큐를 구현하기 위한 방법 중 하나입니다.

- 우선순위 큐는 요소들에 우선순위를 부여하고, 가장 높은 우선순위를 가진 요소에 빠르게 접근할 수 있는 추상 자료형(ADT)입니다. 이때 Heap은 이러한 우선순위 큐를 구현하는 데 사용되는 자료 구조입니다.

- Heap은 완전 이진 트리의 형태를 가지며, 힙 속성을 만족해야 합니다. 최대 힙(Max Heap)의 경우, 루트 노드는 항상 자식 노드들보다 크거나 같은 값을 갖고 있습니다. 최소 힙(Min Heap)의 경우, 루트 노드는 항상 자식 노드들보다 작거나 같은 값을 갖고 있습니다.

- 힙은 일반적으로 배열로 구현되며, 이진 트리의 형태를 배열에 저장하여 공간을 절약합니다. 배열 인덱스를 사용하여 노드 간의 관계를 나타냅니다.

<br/>
<h2>🤔 힙을 배열로 구현한다고 가정하면, 어떻게 값을 저장할 수 있을까요?
</h2>

<h3>📝 나의 대답</h3>

- Heap은 완전 이진 트리의 형태를 갖습니다. 값이 추가될 때, 자식 노의 좌측에서 우측으로 채우며 한 부모 노드에 두 개의 자식 노드를 갖는 형태를 가집니다.

- Max Heap을 구현한다고 가정했을 때, 만약 자식의 값이 부모의 노드보다 크다면 배열의 큰 값과 부모 노드를 교체합니다.

<h3>GPT의 대답</h3>

- 루트 노드를 인덱스 0에 저장합니다. 부모 노드의 인덱스가 i라면, 왼쪽 자식 노드의 인덱스는 2i + 1이 되고, 오른쪽 자식 노드의 인덱스는 2i + 2가 됩니다.

<br/>
<h2>🤔 힙의 삽입, 삭제 방식에 대해 설명하고, 왜 이진탐색트리와 달리 편향이 발생하지 않는지 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 힙에 데이터를 삽입 시, 완전 이진 트리의 마지막 노드에 값이 추가됩니다. 최대 힙의 경우 삽입된 데이터가 부모 노드보다 크다면 부모 노드와 위치를 변경합니다. 부모 노드가 자식보다 클 경우까지 반복 수행됩니다. 삭제의 경우 Root Node가 제거되며 자식 노드 중 큰 다음 값을 Root Node에 추가합니다. 이 행위를 완전 이진 트리가 완성 될 때까지 수행합니다.

- 이진탐색트리와 달리 편향되지 않은 이유는 완전 이진 트리를 유지하기 때문입니다.

<h3>GPT의 대답</h3>

- 힙은 완전 이진 트리의 형태를 유지하면서, 힙 속성을 만족해야 합니다.

- 완전 이진 트리는 노드들이 왼쪽에서 오른쪽으로 차례대로 채워지는 구조를 가지므로, 편향이 발생하지 않습니다.

- 힙의 삽입과 삭제 과정에서 루트 노드를 기준으로 한 부분 트리에서만 교환 작업이 수행되므로, 편향이 발생하지 않습니다.

- 반면 이진 탐색 트리에서는 특정 순서로 데이터를 삽입하거나 삭제할 경우, 트리의 균형을 잃어 편향된 구조가 될 수 있습니다.

<br/>
<h2>🤔 힙 정렬의 시간복잡도는 어떻게 되나요? Stable 한가요.</h2>

<h3>📝 나의 대답</h3>

- 힙 정렬의 시간 복잡도는 O(logN)입니다. 바텀업으로 정렬이 이뤄진다면 O(logN)의 시간복잡도를 따르지만 탑다운 방식으로 정렬한다면 모든 Leaf를 순회해야 하기 때문에 Stable하지 않습니다.

<h3>GPT의 대답</h3>

- 힙 정렬의 시간 복잡도는 O(NlogN)입니다. 힙을 구성하는 과정에서는 힙 속성을 만족하기 위해 로그 시간이 소요됩니다. 이를 N번 반복하므로, O(NlogN)의 시간 복잡도가 됩니다.

- 힙 정렬은 탑다운 방식(Top-Down)으로도 구현할 수 있지만, 일반적으로는 바텀업 방식(Bottom-Up)을 사용합니다. 바텀업 방식은 초기 힙 구성 단계에서 로그 시간이 소요되고, 이후 정렬 단계에서는 상수 시간이 소요되므로 전체적으로 O(NlogN)의 시간 복잡도를 가집니다.

- 힙 정렬은 안정적인 정렬 알고리즘이 아닙니다. 안정적인 정렬 알고리즘은 동일한 값의 순서가 정렬 전후에 유지되는 것을 의미하는데, **힙 정렬은 원본 데이터의 상대적인 순서를 변경할 수 있으므로 안정적이지 않습니다.**

</div>
</details>

<details>
<summary style="font-size:20px">BBST</summary>
<div markdown="1">
<br/>
<h2>🤔 BBST (Balanced Binary Search Tree) 와, 그 종류에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- BBST는 이진 탐색 트리의 편향을 없애기 위해 고안된 자료구조입니다. BBST의 종류로 AVL 트리와 Red-Black 트리가 존재합니다.

<br/>
<h2>🤔 Red Black Tree는 어떻게 균형을 유지할 수 있을까요?</h2>

<h3>GPT의 대답</h3>

- 각 노드는 레드(Red) 또는 블랙(Black) 색깔을 가집니다. 루트 노드는 항상 블랙(Black)입니다. 모든 리프 노드(NIL 노드)는 블랙(Black)입니다.

- 레드(Red) 노드의 자식 노드들은 모두 블랙(Black)입니다. 어떤 노드로부터 자손인 리프 노드까지의 모든 경로에는 동일한 개수의 블랙(Black) 노드가 있어야 합니다. 이를 블랙 노드의 개수 규칙이라고 합니다.

<br/>
<h2>🤔 2-3-4 Tree, AVL Tree 등의 다른 BBST 가 있음에도, 왜 Red Black Tree가 많이 사용될까요.</h2>

<h3>GPT의 대답</h3>

- 상대적으로 간단한 구현, 좋은 평균적인 성능, 일반적인 응용 분야에 적합, 상대적으로 적은 회전 연산, 널 네츄럴 성질
</div>
</details>

<details>
<summary style="font-size:20px">Sorting</summary>
<div markdown="1">
<br/>
<h2>🤔 Quick Sort와 Merge Sort를 비교해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Quick Sort는 pivot을 기준으로 시작점과 끝점을 비교해 값을 비교했을 때 시작점에 가까운 것이 끝점에 있는 값보다 클 경우 교체해가며 정렬을 수행합니다.

- Quick Sort는 pivot을 기준으로 재귀를 사용하여 구현할 수 있으며 시작점의 인덱스가 끝점의 인덱스보다 작을 때만 교체 로직이 수행되어 정렬을 수행합니다.

- Merge Sort는 배열을 잘게 쪼개고 쪼갠 배열을 합치는 과정에서 대소를 비교해 정렬을 진행합니다.

- 분할 정복 컨셉을 사용하는 것은 공통의 부분이지만 로직은 다르게 수행됩니다.

<h3>GPT의 대답</h3>

- Quick Sort는 pivot을 중심으로 데이터를 분할하여 정렬하는 분할 정복 알고리즘입니다. 이 알고리즘의 평균 시간 복잡도는 O(n log n)이지만, 최악의 경우에는 O(n^2)입니다. 퀵 소트는 공간 복잡도가 더 낮으며, 실제 운영 환경에서는 대부분의 경우 병합 소트보다 빠릅니다. 하지만 퀵 소트는 안정적인 정렬 알고리즘이 아닙니다.

- 반면에, Merge Sort는 배열을 반으로 나누어 각각 정렬한 후 병합하는 분할 정복 알고리즘입니다. 병합 정렬의 시간 복잡도는 모든 경우에 대해 O(n log n)입니다. 하지만 임시 배열을 사용해야 하므로 추가적인 메모리가 필요하다는 단점이 있습니다. 병합 소트는 퀵 소트와 달리 안정적인 정렬 알고리즘입니다.

<br/>
<h2>🤔 Quick Sort에서 O(N^2)이 걸리는 예시를 들고, 이를 개선할 수 있는 방법에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- 오름차순으로 정렬을 원할 때, 내림차순으로 정렬된 배열이 주어지고 pivot 시작을 제일 왼쪽에서 시작하면 최악의 실행 시간인 O(N^2)가 소요됩니다.

- 이를 개선하기 위해선, pivot의 위치를 중간으로 지정해주어 해결할 수 있습니다.

<h3>GPT의 대답</h3>

-  'Median of Three' 전략을 사용하여 배열의 왼쪽, 오른쪽, 그리고 중간의 값을 선택하고 이들 중 중간값을 피봇으로 사용할 수 있습니다. 이러한 방법은 주어진 데이터에 상관없이 퀵 소트의 성능을 일관되게 개선하는 데 도움이 됩니다.

<br/>
<h2>🤔 Stable Sort가 무엇이고, 어떤 정렬 알고리즘이 Stable 한지 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Stable Sort는 최악과 최선 실행 시간이 조건에 상관 없이 일정한 것을 의미합니다. 예를 들어 Bubble Sort가 Stable Sort입니다. ❌ 틀렸습니다. ❌

<h3>GPT의 대답</h3>

- Stable Sort는 동일한 값이 정렬이 수행되었을 때, 상대적 순서를 유지하는 정렬 방식을 이야기합니다.

<br/>
<h2>🤔 Merge Sort를 재귀를 사용하지 않고 구현할 수 있을까요.</h2>

<h3>📝 나의 대답</h3>

- 네. 구현할 수 있습니다. 분할해서 병합할 때 생성되는 배열을 미리 만들어놓는다면 구현할 수 있습니다.

<br/>
<h2>🤔 Radix Sort에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Radix Sort는 계수 정렬을 의미하며 미리 메모리 공간에 계수 테이블을 만들어 놓고 정렬을 수행합니다.


<h3>GPT의 대답</h3>

- Radix Sort는 정렬할 숫자들을 자릿수별로 비교하며 정렬을 진행합니다.

- Radix Sort는 보조 배열 또는 메모리 공간인 "계수 테이블"을 사용하여 정렬을 수행합니다. 각 자릿수별로 0부터 9까지의 숫자가 몇 개 등장하는지를 계수 테이블에 저장하고, 이를 이용하여 숫자들을 그룹화하고 정렬합니다. 계수 테이블을 사용하여 정렬하는 과정에서 추가적인 메모리 공간을 사용하게 됩니다.

- Radix Sort는 안정적인 정렬 알고리즘이며, 비교 기반의 다른 정렬 알고리즘들과는 달리 자릿수 비교를 통해 정렬하기 때문에 선형 시간 복잡도 O(n)를 가질 수 있습니다. 하지만 정렬할 숫자들의 자릿수가 많거나 숫자의 범위가 크다면 추가적인 메모리 공간이 필요하고, 성능 측면에서 다른 알고리즘들과 비교해야 합니다.

<br/>
<h2>🤔 Bubble, Selection, Insertion Sort의 속도를 비교해 주세요.</h2>

<h3>GPT의 대답</h3>

✅ Bubble Sort

- 인접한 두 원소를 비교하고 필요한 경우 위치를 교환하는 방식으로 정렬합니다.

- 최악, 평균, 최선의 시간 복잡도는 모두 O(n^2)입니다.

- Bubble Sort는 안정적인 정렬 알고리즘이지만, 비교 및 교환을 많이 수행하므로 큰 데이터셋에 대해서는 효율적이지 않습니다.

✅ Selection Sort

- 주어진 배열에서 가장 작은 값을 선택하여 정렬된 부분 배열에 차례대로 추가합니다.

- 최악, 평균, 최선의 시간 복잡도는 모두 O(n^2)입니다.

✅ Insertion Sort

- 배열을 정렬된 부분과 정렬되지 않은 부분으로 나누고, 정렬되지 않은 부분의 원소를 정렬된 부분에 적절한 위치에 삽입합니다.

- 최악, 평균의 시간 복잡도는 O(n^2)이지만, 최선의 경우(정렬된 배열에 새로운 원소를 추가할 때)에는 O(n)의 시간 복잡도를 가질 수 있습니다.

<br/>
<h2>🤔 값이 거의 정렬되어 있거나, 아예 정렬되어 있다면, 위 세 알고리즘의 성능 비교 결과는 달라질까요.</h2>

<h3>📝 나의 대답</h3>

- 네. Insertion Sort의 실행 시간이 O(N)으로 나타날 수 있습니다.

<br/>
<h2>🤔 본인이 사용하고 있는 언어에선, 어떤 정렬 알고리즘을 사용하여 정렬 함수를 제공하고 있을까요.</h2>

<h3>GPT의 대답</h3>

✅ Java 11 이전의 버전에서는 Arrays.sort() 메서드를 사용하여 배열을 정렬할 때, 일반적으로 Dual-Pivot Quick Sort 알고리즘이 사용되었습니다. Dual-Pivot Quick Sort는 Quick Sort 알고리즘의 변형으로, 두 개의 피벗(pivot)을 사용하여 배열을 분할하고 정렬합니다.

- 하지만 Java 11부터는 Arrays.sort() 메서드의 내부 정렬 알고리즘이 바뀌었습니다. Java 11에서는 Timsort 알고리즘이 기본적으로 사용됩니다. Timsort는 Tim Peters가 개발한 안정적인 정렬 알고리즘으로, Merge Sort와 Insertion Sort의 조합을 사용합니다. Timsort는 최선 및 평균 시간 복잡도가 O(n log n)이며, 최악의 경우에도 O(n log n)의 시간 복잡도를 가지므로 효율적인 정렬 알고리즘 중 하나입니다.

<br/>
<h2>🤔 정렬해야 하는 데이터는 50G 인데, 메모리가 4G라면, 어떤 방식으로 정렬을 진행할 수 있을까요.</h2>

<h3>📝 나의 대답</h3>

- Merge Sort의 방식으로 데이터를 정렬할 것 같습니다. 이유는 정렬해야할 배열을 자르고 정렬을 수행하지 않는 부분을 보조 메모리에 적재해 정렬이 끝나면 다음 정렬 배열을 꺼내와 수행하는 방식으로 문제를 해결한다면 데이터에 비해 작은 메모리가 존재하더라도 정렬을 진행할 수 있을 것입니다.

</div>
</details>

<details>
<summary style="font-size:20px">Graph</summary>
<div markdown="1">
<br/>
<h2>🤔 그래프 자료구조에 대해 설명하고, 이를 구현할 수 있는 두 방법에 대해 설명해 주세요.</h2>

<h3>📝 나의 대답</h3>

- Graph 자료구조는 연결 상태를 나타낸 자료구조입니다. 배열과 링크드 리스트를 통해 구현할 수 있습니다.

<h3>GPT의 대답</h3>

- Graph(그래프)는 객체 간의 연결 관계를 표현하는 비선형 자료구조입니다. 그래프는 노드(Node)와 간선(Edge)으로 구성되며, 노드는 개별적인 요소를 나타내고, 간선은 노드들 간의 연결을 나타냅니다.

- 인접 행렬 (Adjacency Matrix): 그래프의 연결 상태를 2차원 배열로 나타내는 방법입니다.

- 인접 리스트 (Adjacency List): 그래프의 연결 상태를 각 노드마다 연결된 노드들의 목록으로 나타내는 방법입니다.

<br/>
<h2>🤔 각 방법에 대해, "두 정점이 연결되었는지" 확인하는 시간복잡도와 "한 정점에 연결된 모든 정점을 찾는" 시간복잡도, 그리고 공간복잡도를 비교해 주세요.</h2>

<h3>GPT의 대답</h3>

✅ 연결 노드 시간 복잡도

- 인접 행렬: O(V) : 인접 행렬에서는 한 정점의 모든 연결 상태를 행 또는 열에서 확인해야 하므로, 정점의 개수에 비례하는 시간이 소요됩니다.

- 인접 리스트: O(degree) : 인접 리스트에서는 해당 정점의 연결된 노드들을 순회하면 되므로, 한 정점에 연결된 노드들의 개수에 비례하는 시간이 소요됩니다.

✅ 공간 복잡도

- 인접 행렬: O(V^2) : 인접 행렬은 V x V 크기의 2차원 배열을 사용하기 때문에, 정점의 개수에 제곱에 비례하는 공간이 필요합니다.

- 인접 리스트: O(V + E) : 인접 리스트는 정점의 개수에 비례하는 크기의 리스트를 사용하고, 간선의 개수만큼의 추가적인 공간이 필요합니다.

<br/>
<h2>🤔 정점의 개수가 N개, 간선의 개수가 N^3 개라면, 어떤 방식으로 구현하는 것이 효율적일까요.</h2>

<h3>GPT의 대답</h3>

- 두 정점의 연결 여부를 확인하는 시간 복잡도에서는 인접 행렬이 더 우수하지만, 한 정점에 연결된 모든 정점을 찾는 시간 복잡도에서는 인접 리스트가 유리합니다. 그리고 공간 복잡도에서는 인접 행렬은 정점의 개수에 제곱에 비례하는 공간이 필요하므로, 인접 리스트보다 더 많은 공간을 차지합니다.

- 이러한 차이로 인해, 인접 행렬은 간선의 수가 많고 밀집된 그래프에서 유리하며, 인접 리스트는 간선의 수가 적거나 희소한 그래프에서 유리합니다. 따라서 그래프의 특성과 애플리케이션의 요구사항에 맞게 적절한 자료구조를 선택해야 합니다.

<br/>
<h2>🤔 사이클이 없는 그래프는 모두 트리인가요? 그렇지 않다면, 예시를 들어주세요.</h2>

<h3>📝 나의 대답</h3>

- 네. 트리입니다. 트리는 그래프의 일종이지만 순환이 존재하지 않는 것이기 때문입니다.

<h3>GPT의 대답</h3>

- 트리는 추가적인 제약 조건을 충족해야 합니다.

- 하나의 루트 노드를 가져야 합니다. 루트 노드는 트리의 시작점이며, 모든 다른 노드는 루트 노드에서부터 접근 가능해야 합니다.

- 모든 노드는 정확히 하나의 부모를 가져야 합니다. 즉, 각 노드는 다른 노드와 최대 하나의 간선으로 연결되어야 합니다.

- 임의의 노드에서 다른 노드로 가는 경로는 유일해야 합니다. 즉, 두 노드 간에는 유일한 경로가 존재해야 합니다.

</div>
</details>

<details>
<summary style="font-size:20px">Graph 최단 거리</summary>
<div markdown="1">
<br/>
<h2>🤔 트리에서는 어떤 방식으로 최단거리를 구할 수 있을까요</h2>

<h3>📝 나의 대답</h3>

- 트리에서 최단 거리를 구하는 것의 시작점은 루트 노드입니다. 찾고자하는 값의 최소값을 구하기 위해서 부르트 포스 알고리즘을 수행해 모든 경우의 수를 구해 최단 거리를 찾을 수 있습니다.

<br/>
<h2>🤔 다익스트라 알고리즘에서, 힙을 사용하지 않고 구현한다면 시간복잡도가 어떻게 변화할까요.</h2>

<h3>📝 나의 대답</h3>

- Heap을 사용하지 않고 구현한다면 연결된 노드를 매번 선형 탐색해 최단 거리를 구해야 함으로 O(N^2)의 값이 소요됩니다. Heap을 사용해 구현한다면 O(ElogN)을 갖습니다.

<br/>
<h2>🤔 정점의 개수가 N개, 간선의 개수가 N^3 개라면, 어떤 알고리즘이 효율적일까요.</h2>

<h3>GPT의 대답</h3>

✅ Heap을 사용하지 않고 다익스트라 알고리즘을 구현하는 경우, 각 노드마다 모든 인접 노드를 선형 탐색해야 합니다. 이 때 간선의 개수가 N^3개인 경우, 각 노드마다 최대 N^3번의 탐색을 수행해야 하므로 시간 복잡도는 O(N^4)가 됩니다. 이는 매우 큰 시간 복잡도로 인해 실행 시간이 상당히 증가할 수 있습니다.

✅ 반면, Heap을 사용하여 다익스트라 알고리즘을 구현하면, 최소 힙 또는 최대 힙을 사용하여 가장 작은 거리를 가진 노드를 빠르게 찾을 수 있습니다. 간선의 개수가 N^3개인 경우에도, 힙을 사용하여 우선순위 큐를 유지하면서 연산을 수행하면 시간 복잡도는 O(E log N)가 됩니다. E는 간선의 개수이므로, N^3에 비례한다고 가정하면, 시간 복잡도는 O(N^3 log N)이 됩니다. 이는 훨씬 효율적인 실행 시간을 가지게 됩니다.

<br/>
<h2>🤔 음수 간선이 있을 때와, 음수 사이클이 있을 때 각각 어떤 최단거리 알고리즘을 사용해야 하는지 설명해 주세요.</h2>

<h3>GPT의 대답</h3>

✅ 음수 간선이 있는 경우에는 다익스트라 알고리즘 대신에 벨만-포드 알고리즘을 사용하고, 음수 사이클이 있는 경우에는 최단 거리를 정의할 수 없으며, 벨만-포드 알고리즘을 사용하여 음수 사이클을 탐지할 수 있습니다.

</div>
</details>