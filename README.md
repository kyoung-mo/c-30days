# C-30Days

임베디드 시스템 개발을 위한 C 언어 학습 과제 모음입니다.  
비트 조작, 메모리 관리, 자료구조, 시스템 프로그래밍 등 실무에서 필요한 핵심 개념을 다룹니다.  
개인 과제 정리용이라 정답이 틀리는 경우가 많습니다!

## 📚 과제 구성

### Week 1: 비트 연산과 데이터 표현
- **Day 1**: 특정 비트 제어 매크로 구현
- **Day 2**: Endianness 변환 함수 (Network ↔ Host)
- **Day 3**: 패킹 데이터(Packed Data) 파싱
- **Day 4**: 비트 단위 Reverse (Mirroring)
- **Day 5**: 1의 개수 세기 (Population Count)
- **Day 6**: 원형 비트 시프트 (Circular Shift/Rotate)
- **Day 7**: Checksum 계산 (XOR 방식) LCR ↔ CRC

### Week 2: 포인터와 메모리 관리
- **Day 8**: 안전한 Memcpy 구현 (Overlap 처리)
- **Day 9**: 제네릭 Swap 함수 (`void*`)
- **Day 10**: 이중 포인터를 활용한 2차원 배열 동적 할당
- **Day 11**: 함수 포인터 배열을 이용한 계산기
- **Day 12**: 구조체 멤버 오프셋 매크로 (`offsetof` 구현)
- **Day 13**: 고정 크기 메모리 풀 (Memory Pool) 할당기
- **Day 14**: 헥사 덤프 (Hexdump) 유틸리티

### Week 3: 임베디드 필수 자료구조
- **Day 15**: 원형 버퍼 (Ring Buffer) 구현
- **Day 16**: 단일 연결 리스트 역순 정렬
- **Day 17**: 비트맵 (Bitmap) 관리자
- **Day 18**: 우선순위 큐 (Min Heap) - 태스크 스케줄링용
- **Day 19**: 스택 오버플로우 감지 (Canary)
- **Day 20**: 희소 행렬 (Sparse Matrix) 압축
- **Day 21**: 유한상태 머신 (FSM) - 함수 포인터 활용

### Week 4: 알고리즘 및 시스템 모사
- **Day 22**: 소프트웨어 타이머 (Linked List 기반)
- **Day 23**: 문자열 토크나이저 (strtok 재구현)
- **Day 24**: 디바운싱 (Debouncing) 알고리즘
- **Day 25**: 이동 평균 필터 (Moving Average)
- **Day 26**: 생산자-소비자 (Producer-Consumer) 시뮬레이션
- **Day 27**: CRC-32 구현
- **Day 28**: 가변 인자 함수 구현 (my_printf)
- **Day 29**: 간단한 협력형 스케줄러 (Cooperative Scheduler)
- **Day 30**: 로그 시스템 (Level & Buffer)

## 🎯 학습 목표

- ✅ **메모리 효율성**: 최소한의 메모리로 최대 성능
- ✅ **포인터 안정성**: 메모리 오류 및 누수 방지
- ✅ **비트 연산 최적화**: 하드웨어 제어를 위한 효율적 구현
- ✅ **임베디드 실무 대비**: 실제 개발에서 사용하는 기법

## 🔧 개발 환경

```bash
gcc dayX.c -o dayX && ./dayX
```

## 📁 디렉토리 구조

```
.
├── week1/          # 비트 연산 과제
├── week2/          # 메모리 관리 과제
├── week3/          # 자료구조 과제
└── week4/          # 알고리즘 & 시스템 모사
```

## 📝 작성 규칙

- 변수명 / 함수명: `snake_case`
- 매크로: `UPPER_CASE`
- 구조체: `PascalCase`
- 표준 라이브러리 최소 사용 (직접 구현 우선)
- 메모리 누수 금지, 매직 넘버 금지, 복잡한 로직 주석 필수
