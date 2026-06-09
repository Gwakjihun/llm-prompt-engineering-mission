# LLM Prompt Engineering Mission

## 프로젝트 개요

본 프로젝트는 LLM(Large Language Model)을 활용한 업무 자동화 프롬프트 설계 과제입니다.

회의록 요약 및 Action Item 추출 업무를 대상으로 다음 과정을 수행하였습니다.

- 3종 이상의 LLM 비교 및 선정
- 시스템 프롬프트 설계
- Few-shot Prompting 적용
- 단계적 추론 유도(Reasoning Prompt) 적용
- 환각(Hallucination) 검증
- 10턴 이상 대화 기반 문맥 유지 검증

---

## 선택한 업무 과업

### 회의록 요약 AI Assistant

회의 메모를 입력받아 아래 항목을 자동 생성합니다.

- 결정사항
- Action Items
- 리스크
- 후속 일정

---

## 프로젝트 구조

```text
docs/
├── 01_model_comparison.md
├── 02_system_design.md
└── 03_execution_log.md

prompts/
├── system_prompt_v1.md
├── system_prompt_v2.md
└── few_shot_examples.md

tests/
└── hallucination_test.md

logs/
└── raw_conversation.txt
```

---

## 사용 모델

### 비교 대상

1. GPT-5
2. Claude Sonnet
3. Gemini 2.5 Pro

---

## 주요 기법

### Zero-shot Prompting

예시 없이 작업 수행

### Few-shot Prompting

입력-출력 예시 제공

### Reasoning Prompt

단계적 검토를 통해 누락 및 오류 최소화

---

## 작성자

멀티미디어공학 전공
Prompt Engineering Mission
