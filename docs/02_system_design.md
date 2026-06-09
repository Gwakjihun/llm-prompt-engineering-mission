# 02. 시스템 설계 문서

## 1. 문제 정의

회의 후 회의록을 정리하는 과정은 반복적이며 많은 시간이 소요된다.

특히 다음 항목을 수작업으로 정리해야 한다.

- 결정사항
- Action Items
- 리스크
- 후속 일정

본 프로젝트는 해당 과정을 자동화하기 위한 AI Assistant를 설계하는 것을 목표로 한다.

---

## 2. 타겟 사용자

- 프로젝트 매니저(PM)
- 서비스 기획자
- 개발자
- 스타트업 팀원

---

## 3. 입력 데이터 형태

회의 메모

회의록

회의 녹취 요약본

---

## 4. 출력 규격

- 결정사항
- Action Items
- 리스크
- 후속 일정
- 확인 필요 항목

---

## 5. 입력 템플릿

[회의 내용]

(회의 메모 입력)

[원하는 결과]

결정사항 / Action Items / 리스크

[톤]

사내 공유용

[금지]

추측 금지

[확인 질문]

최대 3개까지 허용

## 6. 페르소나 정의

이름:
Meeting Summary Coach

역할:
프로젝트 매니저 출신 업무 자동화 코치

전문 분야:
프로젝트 관리
회의 운영
업무 프로세스 정리

말투:
간결하고 비즈니스 친화적

금지 사항:
추측성 정보 생성

우선순위:
정확성 > 형식 준수 > 친절성

## 7. 시스템 프롬프트

[system_prompt_v2 전문](https://github.com/Gwakjihun/llm-prompt-engineering-mission/blob/main/prompts/system_prompt_v2.md)

## 8. Few-shot 예시

[few_shot_examples.md](https://github.com/Gwakjihun/llm-prompt-engineering-mission/blob/main/prompts/few_shot_examples.md)

## 9. 환각 검증 설계

[hallucination_test.md](https://github.com/Gwakjihun/llm-prompt-engineering-mission/blob/main/tests/hallucination_test.md)

## 10. 프롬프트 개선 이력

v1

- 단순 요약 지시

문제점

- 형식 불안정
- 확인 질문 부재
- 환각 가능성 존재

v2

- 페르소나 추가
- 확인 질문 규칙 추가
- 단계적 처리 절차 추가
- 확인 필요 항목 추가

개선 결과

- 형식 일관성 향상
- 환각 감소
- 문맥 유지 성능 향상
