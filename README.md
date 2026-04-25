# UnitBench Scores

## Model Performance
| UnitBench          | Max  | ChatGPT 5.5 | Claude Opus 4.7 | Grok 4.20 |  ChatGPT-4o | Gemini 3 Flash | Kimi K2.6 | Deepseek v4 Flash | Qwen 80b a3b |
| -------------------|----: | ----------: | --------------: |---------: |-----------: |--------------: |---------: |-----------------: |------------: |
|       Term coverage|   25 |       18.41 |           14.32 |     14.32 |        4.10 |           2.14 |      2.38 |              2.14 |         1.67 |
|  Date band accuracy|   20 |        9.15 |            4.43 |      7.47 |        0.00 |           1.30 |      5.70 |              5.70 |          5.5 |
|  Etymology accuracy|   25 |        9.38 |            6.88 |      6.75 |        1.87 |           1.25 |      3.88 |              4.29 |         7.86 |
| Unearned Confidence|   15 |       11.13 |           10.01 |     10.66 |        5.90 |          13.80 |     15.00 |             14.25 |        14.06 | 
| Humor              |   15 |       10.96 |            9.29 |     10.46 |        5.91 |          13.88 |     15.00 |             13.88 |        13.59 |
| **Overall Score**  |  100 |     _59.03_ |         _44.93_ |   _49.66_ |     _17.78_ |        _32.37_ |   _41.96_ |           _40.26_ |      _42.68_ |

## Model Run Stats
| Model             | Cost     |       Provider |       Harness |
|-----------------  |--------: |--------------: |-------------: |
| ChatGPT-5.5       |          |    ChatGPT Pro | ChatGPT MacOS |
| Claude Opus 4.7   |          |     Anthrophic |  Claude MacOS |
| Grok 4.20         |    $0.16 |            xAI |      OpenCode |
| ChatGPT-4o        |    $0.00 | Github Copilot |        VSCode | 
| Gemini 3 Flash    |    $0.04 |     OpenRouter |      OpenCode |
| Kimi K2.6         |    $0.12 |     OperRouter |      OpenCode |
| Deepseek v4 Flash |    $0.05 |     OpenRouter |      OpenCode |
| Qwen 80b a3b      |    $0.22 |     OpenRouter |            Pi |

## UnitBench Categories
| Display label       | Canonical key         | Max | Meaning |
| ------------------- | --------------------- | --: | ------- |
| Term coverage       | `coverage`            |  25 | How many gold benchmark terms the submission matched. |
| Date band accuracy  | `date_band_accuracy`  |  20 | How accurate the `first_attested` dates are, with credit for reasonable approximate bands. |
| Etymology accuracy  | `etymology_accuracy`  |  25 | How correct and plausible the etymology explanations are. |
| Unearned Confidence | `calibration`         |  15 | How much the answer avoids fake precision and earns the confidence level it projects. |
| Humor               | `humor`               |  15 | How funny the `why_funny` explanations are under the benchmark rubric. |
| Overall Score       | `total`               |   100 | Sum of all category scores. |
