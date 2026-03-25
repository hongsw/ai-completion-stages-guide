# 레벨별 실습 로드맵

이 문서의 목표는 단순히 "AI에는 이런 단계가 있다"고 설명하는 데 있지 않다.

목표는 사용자가 각 레벨에서 **직접 한 번 실습해보고**, 그 과정에서 **현재 단계의 한계와 다음 단계의 필요성**을 체감하게 만드는 것이다.

즉, 이 문서는 지식 목록이 아니라 **사고 확장 훈련 경로**다.

---

## Level 1. 챗봇 수준
- 상세 실습 페이지: [level-1-chatbot.ko.md](./levels/level-1-chatbot.ko.md)
### 학습 목표
- LLM과 대화하며 생산성을 높이는 법을 익힌다.
- 같은 작업이라도 프롬프트에 따라 결과 편차가 큼을 체감한다.

### 실습 포인트
- 같은 요청을 ChatGPT / Claude / Gemini에 각각 시켜보기
- 같은 프롬프트를 3번 반복해 결과 비교하기
- 한 문단 요약, 표 정리, 회의록 정리 같은 단일 태스크 수행

### 대표 공개 자료
- Awesome LLM Apps: <https://github.com/Shubhamsaboo/awesome-llm-apps>
- Awesome-LLM: <https://github.com/Hannibal046/Awesome-LLM>
- Awesome LLM Resources: <https://github.com/WangRongsheng/awesome-LLM-resources>

### 현재 단계의 불편
- 매번 사람이 직접 물어봐야 한다
- 내 문서/시스템/업무와 연결되지 않는다
- 같은 작업을 반복해도 재현성이 낮다

### 다음 단계의 필요성
> "대화는 되는데, 내 흐름에 연결되진 않네."

그래서 **Level 2 자동화**가 필요해진다.

---

## Level 2. 다중 챗봇 연결 / n8n 자동화 수준
- 상세 실습 페이지: [level-2-automation.ko.md](./levels/level-2-automation.ko.md)
### 학습 목표
- AI를 업무 흐름 안으로 집어넣는다.
- 단순 Q&A를 넘어 이벤트 기반 자동화를 체험한다.

### 실습 포인트
- 폼 입력 → LLM 요약 → 메신저 전송 자동화 1개 만들기
- 이메일/문서/메신저를 연결해 반복 작업 줄이기
- 템플릿 기반 분기 처리 실험하기

### 대표 공개 자료
- n8n: <https://github.com/n8n-io/n8n>
- n8n Docs: <https://github.com/n8n-io/n8n-docs>
- Awesome n8n Templates: <https://github.com/enescingoz/awesome-n8n-templates>
- n8n AI Automations: <https://github.com/lucaswalter/n8n-ai-automations>

### 현재 단계의 불편
- 단순 연결은 되지만 예외처리가 약하다
- AI가 스스로 도구를 쓰는 느낌은 아니다
- 규칙 기반 연결이 많아 복잡성이 커지면 금방 깨진다

### 다음 단계의 필요성
> "자동화는 되는데, AI가 실제로 도구를 쓰며 일하진 못하네."

그래서 **Level 3 스킬/플러그인/MCP**가 필요해진다.

---

## Level 3. 스킬 · 플러그인 · MCP 수준
- 상세 실습 페이지: [level-3-mcp-tools.ko.md](./levels/level-3-mcp-tools.ko.md)
### 학습 목표
- AI가 외부 툴을 호출해 실제 행동하는 구조를 이해한다.
- 파일, 검색, API, DB 등과 연결된 AI를 써본다.

### 실습 포인트
- 파일 읽기/쓰기 가능한 에이전트 환경 써보기
- 검색 + 요약 + 문서 저장 흐름 만들기
- MCP 서버 하나를 연결해 도구 사용 체험하기

### 대표 공개 자료
- Model Context Protocol org: <https://github.com/modelcontextprotocol>
- MCP Spec: <https://github.com/modelcontextprotocol/modelcontextprotocol>
- Awesome MCP Servers: <https://github.com/wong2/awesome-mcp-servers>
- Awesome MCP Servers (alt): <https://github.com/appcypher/awesome-mcp-servers>
- mcp-agent: <https://github.com/lastmile-ai/mcp-agent>

### 현재 단계의 불편
- 도구는 잘 쓰지만 아직 한 명짜리 고급 비서에 가깝다
- 긴 프로젝트를 구조적으로 나눠 처리하기 어렵다
- 역할 분리와 협업이 약하다

### 다음 단계의 필요성
> "툴은 잘 쓰는데, 복잡한 일은 팀처럼 나눠서 해야 하지 않나?"

그래서 **Level 4 서브 에이전트 팀**이 필요해진다.

---

## Level 4. 서브 에이전트 팀 수준
- 상세 실습 페이지: [level-4-subagents.ko.md](./levels/level-4-subagents.ko.md)
### 학습 목표
- 하나의 문제를 여러 역할로 분해하는 법을 익힌다.
- PM, Research, Writer, Reviewer 같은 구조를 실험한다.

### 실습 포인트
- 조사자 / 작성자 / 검토자 역할 분리
- 하나의 주제를 역할별 산출물로 나눠보기
- 멀티에이전트 프레임워크 예제를 1개 실행해보기

### 대표 공개 자료
- AutoGen: <https://github.com/microsoft/autogen>
- CrewAI: <https://github.com/crewAIInc/crewAI>
- CrewAI Examples: <https://github.com/crewAIInc/crewAI-examples>
- LangGraph: <https://github.com/langchain-ai/langgraph>
- awesome-ai-agents: <https://github.com/e2b-dev/awesome-ai-agents>
- awesome-openclaw-agents: <https://github.com/mergisi/awesome-openclaw-agents>

### 현재 단계의 불편
- 누가 무엇을 했는지 추적이 약하다
- 상태/로그/실패지점이 불명확하다
- 팀은 있는데 팀 운영체계가 없다

### 다음 단계의 필요성
> "에이전트 팀은 만들었는데, 운영이 안 된다."

그래서 **Level 5 하네스**가 필요해진다.

---

## Level 5. 에이전트 하네스 수준
- 상세 실습 페이지: [level-5-harness.ko.md](./levels/level-5-harness.ko.md)
### 학습 목표
- 멀티에이전트를 시스템으로 통제하는 법을 배운다.
- 상태, 입출력, 재시도, 평가, 로그의 중요성을 이해한다.

### 실습 포인트
- 동일한 태스크를 역할별로 분리하고 로그 남기기
- 실패 시 어느 단계에서 깨졌는지 추적하기
- 사람이 승인해야 다음 단계로 가는 가드레일 설계하기

### 대표 공개 자료
- harness-100: <https://github.com/revfactory/harness-100>
- LangGraph: <https://github.com/langchain-ai/langgraph>
- mcp-agent: <https://github.com/lastmile-ai/mcp-agent>

### 현재 단계의 불편
- 시스템은 생겼지만 스스로 계속 나아가진 못한다
- 운영자가 개입해 튜닝해야 한다
- 실패에서 자동으로 배우는 구조가 약하다

### 다음 단계의 필요성
> "실행은 통제되는데, 스스로 개선하진 못하네."

그래서 **Level 6 오로보로스**가 필요해진다.

---

## Level 6. 에이전트 오로보로스 수준
### 학습 목표
- 계획-실행-평가-반성-재계획 루프를 설계한다.
- 자기개선 구조와 메타 에이전트 사고를 이해한다.

### 실습 포인트
- 결과물에 대해 자기평가 프롬프트 추가
- 실패 사례를 바탕으로 다음 실행 전략 수정
- 평가 루프가 성능에 어떤 영향을 주는지 비교

### 대표 공개 자료
- Reflexion paper: <https://arxiv.org/abs/2303.11366>
- Generative Agents paper: <https://arxiv.org/abs/2304.03442>
- AutoGen: <https://github.com/microsoft/autogen>
- LangGraph: <https://github.com/langchain-ai/langgraph>

### 현재 단계의 불편
- 내부적으로는 잘 돌아도 외부 검증과 신뢰 확보가 약하다
- 개인/팀 내부 자산으로만 남는다

### 다음 단계의 필요성
> "좋은 구조인데, 남들이 검증하고 따라오게 만들려면?"

그래서 **Level 7 오픈소스 공개**가 필요해진다.

---

## Level 7. 오픈소스 공개 수준
### 학습 목표
- 내부 자산을 외부 검증 가능한 문서, 코드, 예제로 바꾼다.
- 커뮤니티/생태계 관점에서 구조를 생각한다.

### 실습 포인트
- 작은 템플릿/에이전트/문서 1개 공개하기
- README, 튜토리얼, 예제 폴더 구성하기
- 사용자 입장에서 바로 실행 가능한 Quick Start 만들기

### 대표 공개 자료
- Awesome-LLM: <https://github.com/Hannibal046/Awesome-LLM>
- awesome-ai-agents: <https://github.com/e2b-dev/awesome-ai-agents>
- awesome-openclaw-agents: <https://github.com/mergisi/awesome-openclaw-agents>
- LangGraph: <https://github.com/langchain-ai/langgraph>
- AutoGen: <https://github.com/microsoft/autogen>

### 현재 단계의 불편
- 공개는 했지만 아직 사업 모델이 약하다
- 기술 데모와 지속 가능한 서비스 사이 간극이 있다

### 다음 단계의 필요성
> "좋은 오픈소스인데, 이걸 서비스로 어떻게 팔지?"

그래서 **Level 8 Generate as a Service**가 필요해진다.

---

## Level 8. Generate as a Service 수준
### 학습 목표
- 생성형 AI를 서비스 상품으로 설계한다.
- 고객이 반복 구매할 수 있는 결과물 단위를 생각한다.

### 실습 포인트
- 특정 업종용 문서 생성 서비스 기획
- 한 가지 산출물(광고문안, 강의안, 요약 리포트)을 템플릿화
- 입력-생성-검수-납품 구조 설계

### 대표 공개 자료
- Awesome LLM Apps: <https://github.com/Shubhamsaboo/awesome-llm-apps>
- awesome-ai-apps: <https://github.com/Arindam200/awesome-ai-apps>
- n8n AI Automations: <https://github.com/lucaswalter/n8n-ai-automations>

### 현재 단계의 불편
- 비용/지연/도메인 적합성이 한계가 된다
- 범용 모델만으로는 서비스 최적화가 어렵다

### 다음 단계의 필요성
> "서비스는 되는데, 우리 도메인에 최적화된 모델이 필요하네."

그래서 **Level 9 sLLM/ML 적용**이 필요해진다.

---

## Level 9. sLLM / ML 구현 및 서비스 적용 수준
### 학습 목표
- 작은 모델, 랭커, 분류기, 파인튜닝 구조를 이해한다.
- 서비스 품질/속도/비용 최적화를 직접 설계한다.

### 실습 포인트
- 작은 분류기 또는 랭킹 모델 실험
- QLoRA 기반 파인튜닝 개념 이해
- 특화 데이터셋이 성능에 미치는 영향 관찰

### 대표 공개 자료
- TinyLlama: <https://github.com/jzhang38/TinyLlama>
- QLoRA: <https://github.com/artidoro/qlora>
- Awesome-Chinese-LLM: <https://github.com/HqWu-HITCS/Awesome-Chinese-LLM>
- Awesome-LLMOps: <https://github.com/tensorchord/Awesome-LLMOps>

### 현재 단계의 불편
- 개별 모델/서비스는 있으나 연구적 권위와 공개 benchmark는 부족할 수 있다
- 더 넓은 생태계 영향력을 만들기 어렵다

### 다음 단계의 필요성
> "모델과 서비스는 있는데, 연구·평가·공개 benchmark까지 묶고 싶다."

그래서 **Level 10 Full LLM / 벤치마크 / 논문** 단계가 필요해진다.

---

## Level 10. 시스템 정의형 사용자 수준
### 학습 목표
- 어떤 인터페이스, 운영 구조, 환경 구성이 더 나은 AI 경험을 만드는지 정의한다.
- 단순 구현자가 아니라 시스템 설계자로 사고를 확장한다.

### 실습 포인트
- 에이전트/도구/사용자 흐름을 구조도로 재정의해보기
- "우리 조직/서비스에는 어떤 AI 운영 방식이 맞는가" 문서화하기
- 멀티모달 인터페이스와 환경화 관점에서 UX 재설계하기

### 대표 공개 자료
- Microsoft Agentic AI maturity: <https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/maturity-model-overview>
- MITRE AI Maturity Model: <https://www.mitre.org/news-insights/publication/mitre-ai-maturity-model-and-organizational-assessment-tool-guide>

### 현재 단계의 불편
- 잘 만든 시스템은 있어도, 다음 세대 경험을 정의하는 언어가 약할 수 있다
- 구현은 가능한데 새 기준을 제시하진 못할 수 있다

### 다음 단계의 필요성
> "우리가 잘 만든 건 맞는데, 아직 frontier를 열었다고 보긴 어렵다."

그래서 **Level 11 프론티어 개척형 사용자** 단계가 필요해진다.

---

## Level 11. 프론티어 개척형 사용자 수준
### 학습 목표
- 새로운 AI 상호작용, 멀티모달 환경, 운영체제적 경험, 연구 질문을 개척한다.
- 기존 레퍼런스를 따라가는 것을 넘어 새로운 기준을 만든다.

### 실습 포인트
- 아직 널리 정리되지 않은 AI 사용 시나리오를 개념화하기
- 새로운 benchmark 또는 평가 질문 만들기
- 실험 결과를 논문/테크 리포트/오픈소스로 공개하기

### 대표 공개 자료
- Agentic AI review: <https://www.mdpi.com/1999-5903/17/9/404>
- LLaMA paper: <https://arxiv.org/abs/2302.13971>
- Meta Llama: <https://ai.meta.com/llama/>
- Mistral: <https://github.com/mistralai>
- Attention Is All You Need: <https://arxiv.org/abs/1706.03762>

### 최종 메시지
이 단계는 단순히 AI를 잘 쓰는 수준이 아니라,
**지능 시스템의 다음 질서를 제안하고 시험하는 수준**이다.

---

## GitHub Pages 구성 제안
이 문서는 향후 GitHub Pages에서 다음처럼 보이게 만들면 좋다.

- 홈: "나는 지금 몇 단계인가?"
- 레벨 지도: 1~10단계 카드
- 각 레벨 페이지:
  - 정의
  - 왜 필요한가
  - 현재 단계의 불편
  - 다음 단계의 필요성
  - 공개 리포지토리 큐레이션
  - 1시간 실습 미션
  - 추천 독자
- 마지막 페이지:
  - 창업자용 로드맵
  - 연구자용 로드맵
  - 일반인용 로드맵
