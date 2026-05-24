# NestJS Official Docs Korean Study

NestJS 공식 문서를 한국어로 정리하고, 문서 내용을 직접 구현하면서 학습하는 저장소이다.

공식 문서를 그대로 번역하는 것에만 집중하지 않고, 문서에서 설명하는 개념을 실제 코드로 작성하며 이해하는 것을 목표로 한다. 공부하면서 추가로 알게 된 내용, 구현 중 막혔던 부분, 정리해두면 좋을 내용을 함께 기록한다.

## Study Goal

- NestJS 공식 문서를 한국어로 정리한다.
- 공식 문서의 예제와 개념을 직접 구현한다.
- 구현하면서 알게 된 내용을 추가 학습 노트로 남긴다.
- 섹션별로 문서와 코드를 나누어 정리한다.
- 나중에 다시 참고할 수 있는 개인 NestJS 학습 레퍼런스를 만든다.

## Study Flow

각 학습 내용은 아래 흐름으로 정리한다.

1. 공식 문서를 읽는다.
2. 핵심 내용을 한국어로 정리한다.
3. 관련 예제를 직접 구현한다.
4. 구현 과정에서 알게 된 내용을 기록한다.
5. 필요하면 추가 자료를 참고해서 보완한다.

## Project Structure

초기 구조는 단순하게 시작하고, 학습 내용이 늘어나면 점진적으로 추가한다.

```text
.
├── README.md
├── docs
│   └── section-01
│       ├── README.md
│       ├── translation.md
│       ├── study-notes.md
│       └── implementation.md
├── examples
│   └── section-01
└── references
    └── official-docs-links.md
```

## Directory Guide

### `docs`

공식 문서 번역, 요약, 추가 학습 내용을 정리한다.

- `README.md`: 섹션 소개와 전체 흐름을 작성한다.
- `translation.md`: 공식 문서 내용을 한국어로 정리한다.
- `study-notes.md`: 추가로 공부한 내용과 개인적으로 이해한 내용을 기록한다.
- `implementation.md`: 실제 구현 과정과 적용 방법을 정리한다.

### `examples`

공식 문서 내용을 직접 구현한 코드를 정리한다.

### `references`

공식 문서 링크와 추가 참고 자료를 정리한다.

## First Study

첫 번째 학습 내용은 **Swagger 구현**으로 시작한다.

NestJS 프로젝트에 Swagger를 적용하면서 API 문서를 자동으로 생성하는 흐름을 익힌다. 처음에는 간단한 Controller와 DTO를 기준으로 Swagger UI를 띄우는 것부터 진행하고, 이후 요청/응답 스키마, 태그, 인증 설정 등을 점진적으로 추가한다.

정리할 내용은 아래와 같다.

- Swagger를 사용하는 이유
- `@nestjs/swagger` 설치
- `main.ts`에서 Swagger 설정하기
- 기본 API 문서 생성하기
- DTO와 Swagger 데코레이터 연결하기
- Swagger UI에서 API 확인하기

## Branch Strategy

브랜치는 아래 흐름으로 관리한다.

- `main`: 최종적으로 정리된 안정적인 내용만 반영한다.
- `develop`: 학습 내용을 통합해서 관리한다.
- `feature/section01`: 첫 번째 학습 내용을 작업한다.
- `feature/section02`: 두 번째 학습 내용을 작업한다.
- `feature/section03`: 세 번째 학습 내용을 작업한다.

작업은 `main`에서 `develop`을 만들고, `develop`에서 섹션별 `feature` 브랜치를 생성해서 진행한다.

```text
main -> develop -> feature/section01
```

섹션 작업이 끝나면 `feature/section01`을 `develop`에 병합한다. 정리된 내용이 안정적이라고 판단되면 `develop`을 `main`에 병합한다.

## Notes

이 저장소는 NestJS 공식 문서를 읽고 직접 구현하면서 쌓아가는 학습 기록이다. 처음부터 모든 구조를 완성하지 않고, 공부하는 내용이 늘어날 때마다 문서와 예제를 추가한다.
