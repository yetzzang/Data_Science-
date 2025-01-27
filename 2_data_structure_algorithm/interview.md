# CS 기술 면접 예상 질문

* 배열의 가장 큰 특징과 그로 인해 발생하는 장점과 단점에 대해 설명해주시오.
> 배열의 가장 큰 특징은 데이터를 인덱스와 함께 순차적으로 저장한다는 것 입니다. 그래 인해, 인덱스를 활용하여 데이터에 빠르게 접근할 수 있다는 장점이 있습니다. 반면, 데이터의 삽입이나 삭제는 기존의 데이터를 옮겨야한다는 단점이 있습니다. 정리하자면, 데이터의 갯수가 고정적이고 삽입/삭제가 빈번하지 않거나 데이터의 접근이 빈번한 경우 유용하게 사용될 수 있습니다.

* 배열을 사용하면 좋을 데이터의 예를 구체적으로 들어주세요. 또한, Array를 적용하면 좋은 이유와 Array를 사용하지 않으면 어떻게 되는지 함께 설명해주세요.
> 좋을 데이터의 예시로는 주식 차트와 날씨 데이터가 있습니다. 두 데이터 모두 순서를 중요하게 여기며 빈번한 삽입 또는 삭제가 요구되지 않는다는 특징이 있습니다. 그렇기 때문에 배열을 적용시에 필요한 정보에 빠르게 접근이 가능합니다. 하지만 배열을 사용하지 않는다면 원하는 정보를 얻고 싶을떼 전체 자료를 읽어드리며 하나씩 비교해야하기 때문에 시간적으로 비효울적입니다.

* 배열을 사용하여 특정 요소를 검색하는 방법은 무엇인지 설명헤주세요.
> Linear Search 선형 검색이 있습니다. 배열은 데이터를 순서대로 저장하는 특성이 있어 배열에 저장된 모든 요소를 순차적으로 탐색합니다. 따라서 시간 복잡도는 O(n)을 띕니다.

* Array와 ArrayList의 차이점에 대해 설명해주시오.
> 가장 큰 차이점은 크기입니다. Array의 크기는 고정적이기 때문에 초기화시 메모리가 할당 됩니다. 반면, ArrayList는 크기가 가변적입니다. 또한, 데이터 추가 또는 삭제 시 메모리가 재할당되기 때문에 속도가 배열에 비해 느리다는 단점이 있습니다.

* 연결 리스트란 무엇이며, 어떻게 구성되어 있는지 설명해보시오.
> 연결 리스트는 데이터의 요소들을 순서대로 저장하는 선형의 동적 자료구조에 해당합니다. 각 요소는 노드라고 불리며, 데이터와 다음 요소를 가르키는 포인터로 구성되어 있습니다. 첫 번째 노드를 가리키는 Head가 있고, 마지막 노드의 경우 더 이상 가리킬 노드가 없으므로 NULL을 가리키는 Tail이 있습니다. 이로 인해, 데이터의 삽입/삭제 시 포인터만 수정하면 되기 때문에 배열보다 빠르게 수행할 수 있습니다. 하지만, 특정 요소에 접근을 원할 경우, 순차적으로 탐색을 해야하기 때문에 배열보다 느린 속도를 띕니다. 그러므로, 데이터의 수가 가변적이거나 빈번한 삽입 또는 삭제가 요구되는 데이터에 주로 사용됩니다.

* 배열과 연결 리스트의 차이점을 설명해보시오.
> 배열과 연결리스트의 가장 큰 차이점은 데이터의 저장 방식입니다. 먼저, 배열은 정적인 선형의 자료구조로써 최대 길이를 미리 설정하여 연속된 메모리 공간에 순차적으로 데이터를 저장합니다. 이로 인해 특정한 요소에 랜덤 액세스를 지원해 빠른 접근을 원할때 효율적으로 사용된다는 장점이 있습니다. 하지만 삽입 또는 삭제 시 이와 같은 특징 때문에 기존의 요소들을 이동해야 한다는 단점이 있습니다. 그러므로 데이터의 수가 고정적이거나 빈번한 접근이 요구되는 경우 주로 사용됩니다.

> 반면, 연결 리스트의 경우 선형의 동적 자료구조로써 불연속적인 메모리 공간에 데이터를 저장합니다. 각 노드는 데이터와 다음 노드의 주소 값을 저장하고 있습니다. 이로 인해, 데이터의 삽입/삭제 시 포인터만 수정하면 되기 때문에 배열보다 빠르게 수행할 수 있습니다. 하지만, 특정 요소에 접근을 원할 경우, 순차적으로 탐색을 해야하기 때문에 배열보다 느린 속도를 띕니다. 그러므로, 데이터의 수가 가변적이거나 빈번한 삽입 또는 삭제가 요구되는 데이터에 주로 사용됩니다.

* 단순 연결 리스트를 역순으로 출력하는 방법을 설명해보시오.
> 해당 방법으로는 스택에 연결 리스트의 요소를 순차적으로 넣고 빼는 방법이 있습니다. 이 방법은 스택을 사용하므로 추가 메모리가 요구됩니다. 다른 방법으로는 재귀 함수를 이용하는 것 입니다. 재귀 함수 내에서 현재 노드의 다음 노드를 출력하기 전에 재귀 호출을 통해 다음 노드로 이동합니다. 재귀 호출이 끝나면 현재 노드를 출력합니다.

*  Array 와 Linked List 의 Memory Allocation 은 언제 일어나며, 메모리의 어느 영역을 할당받는가요?
> 배열은 컴파일 단계에서 스택 영역에 메모리를 할당 받고, 링크드 리스트는 런타임 단계에서 새로운 노드를 추가할 때마다 힙 영역에 메모리 할당이 일어납니다.

* 벡터와 배열을 차이점을 설명하고, 어떤 경우 벡터가 더 용이한지 설명하시오
> 배열은 정적인 자료구조이며 벡터는 동적인 자료구조 입니다. 배열은 크기가 고정적이기 때문에 메모리가 할당 되어 있습니다. 그에 반해 벡터는 필요에 따라 동적으로 메모리 할당이 가능합니다. 이러한 이유로, 요소의 개수가 동적으로 변하는 경우 벡터가 더 용이하게 사용됩니다. 단편적인 예시로, 사용자가 온라인 쇼핑을 하며 상품을 선택할 때마다 요소가 추가됩니다. 때문에 사용자가 선택한 상품의 수에 따라 벡터의 크기가 자동적으로 조정됩니다. 더불어 메모리 할당이 유동적이며 메모리 관리가 중요한 경우 사용됩니다.

* 벡터의 용량 capacity와 크기 size의 차이는 무엇인지 설명하시오
> 용량은 벡터가 현재 할당 된 메모리 공간의 크기를 나타냅니다. 크기는 벡터에 저장된 원소의 개수를 나타냅니다. 한 요소를 추가할때 용량이 부족하다면 벡터는 현재 용량의 두배 크기로 늘립니다. 만약 벡터의 용량이 2였다면 삽입 후 벡터의 용량은 4가 될 것 이고, 사이즈는 3이 될 것 입니다.

* 벡터의 메모리 할당과 해제는 어떻게 이루어지나요?
> 메로리 할당은 동적 배열의 크기 조절 시에 이루어지며, 해제는 벡터가 파괴될 때 이루어집니다.

* Stack과 Queue의 차이점에 대해 설명하세요
> 스택은 쌓아올리는 형식의 후입선출 Last In First Out 구조 입니다. 데이터를 정해진 방향으로 쌓을 수 있으며, 한 방향으로만 접근이 가능하다는 특성이 있습니다. 주로 DFS 나 재귀 알고리즘에 활용됩니다.
이러한 특성으로 웹 브라우저 방문 기록, 뒤로 가기, 실행 취소, 역순 문자열 만들기, 또는 후위 표기법등에 주로 사용됩니다.

> 큐는 줄을 세우는 형식의 선입선출 First In First Out 구조입니다. 큐는 한 쪽 끝에서 삽입을, 다른 한 쪽 끝에서 삭제를 수행합니다. 이러한 특성으로, 주로 데이터가 시간 순서대로 처리되어햐 하는 경우 사용됩니다. 실생활 예시로는 프린터의 출력처리, 콜센터 고객 대기 시간, BFS 구현, 캐시 구현에 사용됩니다.

* Stack과 Queue의 공통점에 대해 설명하세요.
> 공통점으로는 큐와 스택 모두 순차적으로 데이터를 처리한다는 특성이 있씁니다. 이러한 특성으로 주로 배열로 구현이 되기 때문에 중간 요소 임의 접근 또는 삽입/삭제가 불가능 합니다. 만약, 두가지 특성을 모두 가지는 자료구조를 원한다면 덱 (Deque: Double-ended Queue)을 사용합니다. 덱은 양쪽 끝에서 데이터 삽입과 삭제가 가능합니다. 따라서, 양 쪽 끝에 연산이 필요한 경우 주로 사용됩니다.

* 스택으로 큐를 구현하는 방법과 큐로 스택을 구현하는 방법에 대해 설명해주세요.
>   1. 스텍으로 큐 구현하기
    스택 2개를 활용해서 구현할 수 있습니다.
    스택 A와 B가 있을 때, 큐에 PUSH연산이 일어나면 스택 A에 PUSH 합니다.
    이후 큐에 POP연산을 한다면 스택A의 모든 데이터를 스택 B로 옮깁니다. 그렇게 되면 스택 A의 역순으로 데이터가 저장될 것이고, 스택 B를 POP하면 큐에 저장된 데이터 순서대로 출력될 것입니다.
    즉, 스택 A는 인큐의 역할, 스택 B는 디큐의 역할을 하게 됩니다.
    PUSH를 하면 스택 A에 가장 늦게 들어온 데이터가 맨 위에 쌓일 것이고, 이를 다시 스택 B로 옮기면 큐의 구조(선입선출)로 저장됩니다.

>   2. 큐로 스택 구현하기
    큐 2개를 활용해서 구현할 수 있습니다.
    큐 A와 B가 있을 때, 스택에 PUSH 연산이 일어나면, 해당 요소를 우선 큐 A에 PUSH 합니다.
    그 다음 마지막 원소(방금 PUSH한 요소)를 제외한 나머지를 큐 B에 옮긴 후, 다시 큐 A에 차례대로 PUSH한다.
    그럼 가장 나중에 들어온 값이 큐의 첫 번째 위치로 이동하게 되고, TOP이나 POP 연산이 일어날 경우 순서에 맞게 데이터를 POP할 수 있다.

* 우선순위 큐에 대해 설명하세요.
> 우선순위 큐란 각 요소가 우선순위를 가지고 있으며, 우선순위가 우위한 데이터가 먼저 처리되는 자료구조입니다. 이러한 특성으로 데이터의 추가는 어떤 순서로 해도 상관이 없지만, 삭제 시엔 우선순위가 가장 높은, 다르게 말하면 가장 작은 값을 삭제합니다. 이러한 특성으로 인해 시간이 중요한 작업에서 요소의 우선 순위를 통해 빠르게 처리가 가능하다는 장점을 가지고 있습니다. 이러한 시간적인 장점을 극대화 시키기 위해 주로 이진트리 구조의 힙 구현이널리 사용되고 있습니다. 이유로는 힙 구현 방식엔 배열이나 연결리스트를 사용할 수 있지만 특정 상황에 따라 O(n)의 시간 복잡도가 요구 됩니다. 반면, 힙으로 구현한 경우 삽입/삭제 시에 O(log n)이 보장되기 때문입니다. 하지만 다른 구현 방법에 비해 힙 구협이 어렵다는 단점도 있습니다. 사용 사례로는 작업 스케줄링, 시뮬레이션 시스템, 네트워크 라우팅 등이 있습니다.

* 우선순위 큐의 동작원리가 어떻게 되나요?
> 우선순위 큐는 우선순위가 가장 높은 데이터를 먼저 꺼내기 위한 자료구조입니다. 따라서 힙이 가장 일반적으로 사용됩니다. 만약 top이 최대라면 최대힙, 최소라면 최소힙으로 구현하게 됩니다. 힙은 이진트리의 구조로 모든 정점이 자신의 자식 보다 높은 우선순위를 가지고 있다는 특성이 있습니다. 이러한 성질 때문에 삽입과 삭제 시 O(logN)의 시간 복잡도를 가집니다.

* 자료구조 힙의 특징을 설명해주세요.
> 힙은 완전 이진 트리의 일종으로 부모 노드값이 자식 노드 값보다 항상 크거나 작다는 특징을 가지고 있습니다. 종류로는 루트 값이 가장 큰 값인 최대 힙, 루트가 가장 작은 값인 최소 힙이 있습니다. 이러한 특성으로 데이터 정렬에 활용이 가능하며, 우선 순위가 우위한 요소 부터 처리되는 우선 순위 큐 구현에 주로 사용됩니다. 삽입 또는 삭제 시 O(logN)의 시간 복잡도를 가집니다.

* 힙의 삽입 및 삭제 연산에 대해 설명해주세요.
> 삽입 시에는 가장 마지막 위치에 요소를 추가합니다. 그 후, 새로 삽입 된 노드를 부모 노드와 비교해가며 위치를 바꾸는 과정을 반복합니다. 이대, 최대힙 또는 최소힙의 속성을 유지합니다. 삭제의 경우엔 항상 루트 노드가 삭제 됩니다. 이 후, 힙의 마지막 노드를 루트 노드로 이동시킨 후 루트 노드와 자식 노드를 비교해가며 위치를 조정하고, 힙의 속성을 유지힙니다.

*
>셋은 중복된 원소를 허용하지 않고, 원소들을 저장하는 자료구조입니다. 해시 테이블을 사용하여 셋을 구현할 때, 각 원소를 해시 함수를 사용하여 해시 값으로 변환한 다음, 해당 해시 값을 배열의 인덱스로 매핑하여 저장합니다. 이를 통해 중복을 허용하지 않으면서도 빠른 원소 검색이 가능합니다


해시 함수의 정의는 key를 **고정된 길이**의 hash로 변경해주는 역할을 한다. 이 과정을 **hashing**이라고 한다.key를 해시함수라는 함수에 Input으로 넣어서 Ouput으로 나오는 것이 Hash(해시)라고 생각하면 되고, 이 Hash(해시)가 저장위치가 된다고 생각하면 된다.

해시는 색인 또는 인덱스, hash function은 key->hash로 만들어 주는 함수, 해시테이블은 hash를 주소로 삼아 데이터를 저장하는 자료구조이다.
