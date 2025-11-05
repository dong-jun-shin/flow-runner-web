# Flow Runner
<img width="512" height="384" alt="image" src="https://github.com/user-attachments/assets/186b4b10-e5fb-43e3-9f89-4009660ce75f" />

## Get Started

Flow Runner는 복잡한 컴퓨터 과학 알고리즘과 자료구조를 시각적으로 체험하고 학습할 수 있도록 설계된 인터랙티브 웹 애플리케이션입니다.

다음 [링크](https://flow-runner-beta.vercel.app/ko)에 접속하여 애플리케이션을 확인할 수 있습니다.

<img width="1082" height="763" alt="image" src="https://github.com/user-attachments/assets/e434f7ab-c089-4082-babb-aba0c7ece553" />

## Overview

- Flow Runner는 알고리즘(정렬, 탐색, 그래프, 자료구조 등)의 실행 과정을 시각화하여 보여줍니다.
- 사용자는 애니메이션을 통해 단계별로 알고리즘이 동작하는 과정을 직관적으로 이해할 수 있으며, 다양한 프로그래밍 언어로 작성된 소스 코드와 상세 설명을 함께 보며 학습 효과를 높일 수 있습니다.
- 자동 재생과 수동 단계별 실행 모드를 모두 지원하여 자신의 학습 속도에 맞춰 이용 가능합니다.

### 주요 기능

-   **알고리즘 시각화**: 알고리즘의 동작 과정을 다양한 시각화 방식(배열, 그리드, 그래프, 차트, 벡터, 링크드리스트, 트리)으로 제공
-   **인터랙티브 컨트롤**: 재생, 일시정지, 속도 조절, 이전/다음 단계 이동, 리셋 기능
-   **다양한 테스트 케이스**: 기본, 무작위, 엣지 케이스 등 여러 테스트 데이터 제공
-   **다국어 소스 코드**: JavaScript, Python, Java, C++ 등 여러 프로그래밍 언어로 작성된 소스 코드 제공
-   **상세 정보 제공**: 각 알고리즘의 원리, 실행 단계별 설명
-   **다국어 지원**: 한국어/영어 지원 및 자동 언어 감지
-   **반응형 디자인**: 데스크톱, 태블릿, 모바일 등 반응형 UI 지원

### 알고리즘 카테고리

프로젝트의 알고리즘은 학습 흐름과 유지보수성을 고려하여 다음과 같은 카테고리로 구성되어 있습니다:

- **Searching**: `binary-search`
- **Graphs**: `bfs`, `dfs`, `a-star`, `dijkstra`, `topological-sort`
- **Sorting**: `bubble-sort`, `merge-sort`, `selection-sort`, `quick-sort`
- **Data Structures**: `stack`, `queue`, `deque`, `linked-list`, `b-tree`
- **Techniques**: `sliding-window`, `monotonic-stack`
- **Greedy**: `greedy-coin-change`
- **Simulation**: `monte-carlo`
- **ML**: `cosine-similarity`

## Spec Summary

| 구분 | 내용 |
| --- | --- |
| **프레임워크** | Next.js 15 (App Router) |
| **언어** | TypeScript 5+ |
| **UI 라이브러리** | React 19 |
| **스타일링** | Tailwind CSS 3.4+ |
| **애니메이션** | Framer Motion 12+ |
| **국제화** | next-intl 4.3+ |
| **API** | Next.js API Routes |
| **테스트** | Vitest (Unit) + Playwright (E2E) |
| **코드 품질** | ESLint + TypeScript |
| **빌드 도구** | Turbopack |

## Infra

Flow Runner는 서버리스 아키텍처를 기반으로 합니다.

-   **Hosting**: Vercel을 통해 정적 파일을 호스팅하고, Next.js의 서버리스 함수를 실행합니다.
-   **Backend**: 사용자의 피드백을 GitHub Issue로 생성하기 위한 간단한 API를 Next.js API Route로 구현하였습니다.
-   **CI/CD**: GitHub에 소스 코드 Push로 Vercel을 통해 자동 빌드 및 배포가 이루어지도록 구성되어 있습니다.
