# 04. Bonus Assignment

## Bonus 1 - GPTs 배포

### GPT 이름

Meeting Summary AI Assistant

---

### GPT 목적

회의록을 입력받아 다음 정보를 자동으로 정리하는 업무 자동화 AI Assistant를 제작하였다.

- 결정사항
- Action Items
- 리스크
- 후속 일정
- 확인 필요 항목

---

### 적용한 프롬프트 엔지니어링 기법

#### 1. Persona Prompting

프로젝트 매니저(Project Manager) 출신 업무 자동화 코치라는 페르소나를 적용하였다.

#### 2. Few-shot Prompting

회의록 입력 및 출력 예시 3개를 제공하여 일관된 형식의 결과를 생성하도록 설계하였다.

#### 3. Reasoning Prompt

회의 내용을 단계적으로 분석하도록 설계하였다.

분석 절차:

1. 회의 목표 파악
2. 결정사항 추출
3. Action Item 추출
4. 리스크 추출
5. 누락 정보 검토
6. 최종 결과 생성

#### 4. Hallucination Prevention

- 회의록에 없는 정보 생성 금지
- 정보 부족 시 확인 질문 수행
- 확실하지 않은 정보는 "확인 필요"로 표시

---

### GPT 설정 화면

![GPTs 설정 화면](../img/1)

설명:

Meeting Summary AI Assistant GPT 생성 화면

---

### GPT 테스트 결과

![GPT 테스트 결과](../img/2)

설명:

회의록 입력 후 자동으로 결정사항, Action Items, 리스크를 추출하는 결과

---

### 재사용성

본 GPT는 회의록만 입력하면 동일한 형식으로 결과를 생성할 수 있도록 설계되었다.

사용자는 별도의 프롬프트를 반복 입력하지 않고 업무 자동화를 수행할 수 있다.

---

## Bonus 2 - 멀티모달 확장

### 목표

회의록 요약 프로세스를 시각적으로 표현하여 업무 흐름을 쉽게 이해할 수 있도록 하였다.

---

### 생성 이미지

![Workflow Diagram](../img/workflow_diagram.png)

---

### 생성 프롬프트

Create a professional workflow infographic.

Title:
Meeting Summary AI Assistant Workflow

Steps:
Meeting Notes Input
→ Requirement Check
→ Decision Extraction
→ Action Item Extraction
→ Risk Analysis
→ Final Report

Style:
Corporate infographic
Blue and white color palette
Clean modern design

---

### 활용 목적

- 업무 프로세스 시각화
- 신규 사용자 이해도 향상
- AI 업무 자동화 흐름 설명
