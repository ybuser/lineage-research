# Lineage

*Parent Resolution from Context: Feature Composition and LLM Behavior*

Lineage는 주어진 문맥에서 부모를 찾는 능력과 근거가 부족할 때 연결을 보류하는 능력을 평가합니다. 2026년 10월 ARR에 제출한 원고의 재현 자료와 11월 19일 OpenRouter 후속 실험을 정리했습니다.

## 결과표

기존 원고는 전체 Test 1,120건 중 의미 평가 사례 1,117건을 사용했습니다. 아래 후속 실험 표는 같은 Test에서 출처가 겹치지 않는 869건의 사전 지정 첫 실행(run 0)을 보여줍니다. JEM은 판단 상태와 해당되는 부모 ID가 모두 맞은 비율입니다. L/M은 Law와 Military를 동일 가중 평균한 값입니다.

| 오픈 모델 | L/M 0-shot | L/M 6-shot | Geography 0-shot | Geography 6-shot |
| --- | ---: | ---: | ---: | ---: |
| Qwen3.8 27B | 87.00% | 88.74% | 75.00% | 76.30% |
| Gemma 4 31B IT | 71.06% | 83.65% | 81.17% | 81.49% |
| GLM-5.3-Flash | 89.58% | 88.49% | 81.82% | 83.77% |
| Mistral Small 4 | 71.19% | 46.44% | 68.51% | 49.03% |

- [기존 ARR 원고의 비교표](OCTOBER_MANUSCRIPT_JEM.csv)
- [OpenRouter 주요 비교표](OPENROUTER_PRIMARY_RUN0.csv)
- [OpenRouter 전체 조건과 지표](OPENROUTER_ALL_CONDITIONS.csv)
- [OpenRouter 세 번의 실행 간 변동](OPENROUTER_REPEAT_VARIATION.csv)
