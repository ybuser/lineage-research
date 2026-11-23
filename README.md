# Lineage

*Parent Resolution from Context: Feature Composition and LLM Behavior*

Lineage는 주어진 문맥에서 부모를 찾는 능력과 근거가 부족할 때 연결을 보류하는 능력을 평가합니다. 2026년 10월 ARR에 제출한 원고와 11월 19일 OpenRouter 후속 실험의 결과를 정리했습니다.

## OpenRouter 후속 실험

기존 원고는 전체 Test 1,120건 중 의미 평가 사례 1,117건을 사용했습니다. 아래 표는 같은 Test의 출처 비중첩 869건에서 사전 지정한 첫 실행(run 0)의 결과입니다. JEM은 판단 상태와 해당되는 부모 ID가 모두 맞은 비율입니다. L/M은 Law와 Military를 동일 가중 평균한 값입니다.

| 오픈 모델 | L/M 0-shot | L/M 6-shot | Geography 0-shot | Geography 6-shot |
| --- | ---: | ---: | ---: | ---: |
| Qwen3.8 27B | 87.00% | 88.74% | 75.00% | 76.30% |
| Gemma 4 31B IT | 71.06% | 83.65% | 81.17% | 81.49% |
| GLM-5.3-Flash | 89.58% | 88.49% | 81.82% | 83.77% |
| Mistral Small 4 | 71.19% | 46.44% | 68.51% | 49.03% |
