# Level 4. 서브 에이전트 팀

## 이 단계의 정의
하나의 업무를 여러 역할로 나누고, 각 역할을 에이전트처럼 배치하는 단계입니다.

## 이 단계에서 얻는 능력
- 역할 분리
- 조사 / 작성 / 검토 분업
- 복잡한 작업을 병렬 또는 단계별로 처리

## 대표 불편
- 팀은 있는데 운영 구조가 약함
- 누가 무엇을 했는지 추적이 어려움
- 상태, 로그, 재시도가 체계적이지 않음

## 왜 다음 단계가 필요한가
에이전트 팀이 있다고 곧 시스템이 되는 것은 아닙니다.
재현성과 운영 통제가 필요합니다.

## 관련 clawfit reference level
- **Reference Level 2 — Workflow wrappers and orchestration tools**
  - 여러 실행 흐름을 감싸는 래퍼/오케스트레이션 감각과 연결됩니다.
- **Reference Level 3 — Architecture and benchmark references**
  - 멀티에이전트 구조, 추상화 계층, benchmark 관점이 여기서 중요해집니다.

## 추천 공개 자료
- AutoGen: <https://github.com/microsoft/autogen>
- CrewAI: <https://github.com/crewAIInc/crewAI>
- CrewAI Examples: <https://github.com/crewAIInc/crewAI-examples>
- LangGraph: <https://github.com/langchain-ai/langgraph>
- awesome-ai-agents: <https://github.com/e2b-dev/awesome-ai-agents>

## 1시간 실습 미션
### 미션
하나의 작업을 최소 3개 역할로 나눠 보세요.

### 추천 주제
- 보고서 작성
- 제품 조사
- 강의안 초안 만들기
- 마케팅 문구와 검토

### 실습 절차
1. 하나의 작업을 고릅니다.
2. 아래 3개 역할로 나눕니다.
   - 조사자
   - 작성자
   - 검토자
3. 각 역할이 어떤 입력을 받고 어떤 출력을 내야 하는지 적습니다.
4. 멀티에이전트 프레임워크 예제 하나를 보고, 내가 짠 구조와 어떻게 비슷한지 비교합니다.

## 실습 후 질문
- 역할을 나누니 뭐가 좋아졌나?
- 반대로 어디서 더 복잡해졌나?
- 왜 이제 로그/상태/재시도 구조가 필요해졌나?

## 다음 단계
- 다음 추천: [Level 5. 에이전트 하네스](./level-5-harness.ko.md)
