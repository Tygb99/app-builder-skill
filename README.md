# app-plan skill

새 앱 프로젝트를 시작할 때 Claude가 인터뷰를 통해 기획을 구체화하고 문서 구조를 잡아주는 스킬.

## 이 스킬이 하는 것

1. 비개발자도 답할 수 있는 질문으로 앱 기능을 파악한다
2. 답변을 기술 스택으로 내부 변환한다
3. 이 앱에 맞는 문서 파일 구조를 제안하고 실제로 생성한다

## 설치

```bash
mkdir -p ~/.claude/skills/app-plan
cp SKILL.md ~/.claude/skills/app-plan/SKILL.md
```

## 사용법

Claude Code에서 아래 중 하나를 입력하면 자동 트리거된다:

- `/app-plan`
- "앱 만들려고 해"
- "새 프로젝트 시작"
- "앱 기획 도와줘"
- "문서 구조 잡아줘"

## 파일 구성

```
app-plan-skill/
  README.md               ← 지금 보고 있는 파일
  SKILL.md                ← 스킬 본체 (이것만 설치하면 됨)
  principles/
    DOCS_PRINCIPLES.md    ← 스킬이 따르는 문서 운영 원칙 (참고용)
```

`DOCS_PRINCIPLES.md`는 설치 필수 파일이 아니다.
스킬이 왜 이런 문서 구조를 만드는지 배경을 이해하고 싶을 때 참고한다.
