### Redis란

key-value형태를 가지는 오픈 소스 기반의 비관계형 데이터 베이스 관리 시스템 (DBMS)이다. 인메모리 기반이고 영속성과 다양한 데이터 구조를 지원핟다.

### 왜 쓰냐?

Redis는 앞서 말했듯 디스크에 저장되는 것이 아닌 **메모리에 저장**이 된다. 때문에 컴퓨터가 다운되면 **정보가 저장되지 않고 사라진다**는 단점이 존재한다. 반면에 디스크는 컴퓨터가 다운되어도 저장이된다. 하지만 데이터가 메모리에 저장되는 속도가 디스크에 저장되는 **속도보다 훨씬 빠르다**는 장점도 있다. 또한 사용자의 수가 그렇게 많지 않은 서비스는 DB에 저장되는것에 무리가 없지만 사용자가 많아지면 데이터베이스에 무리가 갈 수 있다. 따라서 자주사용되는 정보를 캐싱하게 되는데 이때 Redis가 사용된다.

### 특징

- **key-value**의 구조를 가진다.
- 데이터처리속도가 상당히 빠르다.
- 여러가지 자료구조를 지원한다.
    - String
    - Sets
    - SotedSet
    - HashSet
- **싱글쓰레드**이기때문에 한번에 하나의 명령만을 처리할 수 있다.
- **샤딩**과 **레플리케이션**을 지원한다.

확실히 레디스 명령어나 작동원리를 자세히 알면 도움이 될것같다.

좋은 글이있어서 남겨놓는다.

[https://velog.io/@hyeondev/Redis-란-무엇일까](https://velog.io/@hyeondev/Redis-%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%BC%EA%B9%8C)