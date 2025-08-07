# Q: React에서 Virtual DOM이 무엇인지, 이를 사용하는 이유는 무엇인지 설명해주세요.

virtual DOM이란 실제 DOM의 복사본으로 JavaScript 객체 형태로 메모리에 저장되는 구조입니다.<br/>
React는 상태(state)나 props가 변경될때마다 새로운 Virtual DOM을 생성하고 이전 Virtual DOM과 비교(diffing)하여 변경된 부분만을 실제 DOM에 반영합니다.
이 과정에서 여러 상태 업데이트가 동시에 발생한 경우, React는 이를 하나의 렌더링 사이클로 묶어 처리하는 배치 업데이트(Batched Updates)를 수행하여 불필요한 렌더링을 줄여 성능을 최적화 할 수 있습니다.

## 💬 예상되는 꼬리 질문?


