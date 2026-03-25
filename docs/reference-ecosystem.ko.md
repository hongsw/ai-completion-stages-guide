# clawfit reference-levels와의 연결

이 문서는 `ai-completion-stages-guide`와 아래 문서의 관계를 설명합니다.

- 참조 문서: <https://github.com/hongsw/clawfit/blob/main/docs/reference-levels.md>

중요한 점은 두 문서가 **같은 종류의 레벨 체계가 아니라는 것**입니다.

---

## 두 문서의 역할 차이

### 1) ai-completion-stages-guide
이 저장소의 11단계는 **사용자 성장 단계**입니다.

즉, 질문은 이것입니다.
- 지금 나는 AI를 어디까지 활용하고 있는가?
- 현재 불편은 무엇인가?
- 다음 단계가 왜 필요한가?

이 문서는 사람의 성장, 실습, 학습 경로를 다룹니다.

### 2) clawfit reference-levels
`clawfit/docs/reference-levels.md`의 Level 1~6은 **레퍼런스 생태계 층위**입니다.

즉, 질문은 이것입니다.
- clawfit이 무엇과 비교되어야 하는가?
- 어떤 도구와 프로젝트를 벤치마크해야 하는가?
- 어떤 생태계 요소를 supporting reference로 삼아야 하는가?

이 문서는 제품 비교, 호환성 분석, benchmark 설계, evidence map에 가깝습니다.

---

## 핵심 원칙

이 둘은 서로 충돌하면 안 됩니다.

정리하면:

- **Stages Guide**는 "사람이 어떻게 성장하는가"
- **Reference Levels**는 "무엇을 참고하고 비교해야 하는가"

즉,

> 하나는 **학습/성장 지도**이고,
> 다른 하나는 **비교/참조 지도**입니다.

---

## 연결 방식

이 저장소에서는 `clawfit` reference-levels를 다음처럼 읽는 것을 권장합니다.

### 사용자 단계 ↔ 참조 생태계 매핑

| 사용자 성장 단계 | 주로 연결되는 reference-levels | 의미 |
|---|---:|---|
| 1. 챗봇 사용 | Level 1, 6 | 실제 사용 경험, 입력 인터페이스, 생산성 체감 |
| 2. 자동화 입문 | Level 2 | 워크플로우 래퍼와 오케스트레이션 이해 |
| 3. 스킬·플러그인·MCP | Level 4 | MCP, context, plugin, memory 생태계 이해 |
| 4. 서브 에이전트 팀 | Level 2, 3 | orchestration과 architecture reference를 함께 봐야 함 |
| 5. 에이전트 하네스 | Level 2, 3 | multi-agent execution, abstraction, benchmark 연결 |
| 6. 자기개선 루프 | Level 3 | evaluation, benchmark, reflection 구조 참고 |
| 7. 오픈소스 공개 | Level 1~4 | 실제 공개 프레임워크, 생태계 포지셔닝 참고 |
| 8. Generate as a Service | Level 1~5 | 제품·플러그인·데이터 기반 서비스 구조 참고 |
| 9. sLLM / ML 적용 | Level 3, 5 | benchmark, evidence hub, RAG/data infra 중요 |
| 10. 시스템 정의형 사용자 | Level 3, 4, 5, 6 | architecture + interface + context + infra를 통합적으로 봐야 함 |
| 11. 프론티어 개척형 사용자 | Level 3, 5, 6 | frontier는 benchmark, evidence infra, human-agent interface를 함께 다룸 |

---

## reference-levels 각 층위의 해석

### Reference Level 1 — Core comparison targets
의미:
- 가장 직접적인 비교 대상
- 제품 포지셔닝과 비교표의 핵심

이 저장소에서의 활용:
- 사용자가 "현재 시장의 대표 AI 툴은 무엇인가"를 감 잡을 때 유용
- Level 1~3 학습자에게 특히 좋음

### Reference Level 2 — Workflow wrappers and orchestration tools
의미:
- 다중 실행, 자동화, 래퍼, 원격 운영

이 저장소에서의 활용:
- 사용자 성장 단계의 2, 4, 5단계와 강하게 연결

### Reference Level 3 — Architecture and benchmark references
의미:
- 추상화 계층, benchmark, evaluation, architecture 비교

이 저장소에서의 활용:
- 4단계 이후부터 매우 중요
- 특히 5, 6, 9, 10, 11단계의 사고를 깊게 해줌

### Reference Level 4 — Memory, context, MCP, and plugin ecosystem
의미:
- MCP, memory, plugin, context compatibility

이 저장소에서의 활용:
- 3단계 핵심
- 10단계 시스템 정의에도 중요한 하부 생태계

### Reference Level 5 — Data hub, RAG, and evidence infrastructure
의미:
- RAG, evidence hub, simulation, retrieval infra

이 저장소에서의 활용:
- 8단계 이후 제품화·연구화 구간에서 매우 중요
- 9~11단계와 특히 연결

### Reference Level 6 — Productivity, input, and human-agent interface tools
의미:
- 인간-에이전트 인터페이스
- 음성, 입력, practical UX

이 저장소에서의 활용:
- 단순 생산성 도구처럼 보이지만 사실 10~11단계에서 다시 중요해짐
- frontier는 종종 모델보다 인터페이스에서 열린다

---

## 이 저장소에서 앞으로의 연결 원칙

앞으로 `ai-completion-stages-guide`는 다음 원칙을 따릅니다.

1. 사용자 성장 단계를 설명할 때,
   필요하면 `clawfit reference-levels`를 보조 축으로 함께 제시한다.
2. "이 단계에서 무엇을 공부할지"뿐 아니라,
   "이 단계에서 어떤 생태계 층위를 봐야 하는지"도 안내한다.
3. 특히 4단계 이후에는 단순 리포 링크가 아니라,
   **architecture / benchmark / MCP / evidence / interface** 중 무엇을 보고 있는지 명확히 표시한다.

---

## 한 줄 요약

- `ai-completion-stages-guide` = **사람의 성장 단계**
- `clawfit reference-levels` = **도구/생태계 참조 층위**

둘은 경쟁 관계가 아니라,
**성장 지도와 비교 지도를 겹쳐 보는 보완 관계**입니다.
