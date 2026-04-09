# App Builder Skill

아이디어 한 줄에서 **실행 가능한 PRD + 프로젝트 문서 구조**까지 한 번에 도출하는 Claude Code 스킬.

## What it does

```
인터뷰 → 경쟁사 분석 → 차별화 전략 → PRD + 문서 구조 출력
```

비개발자도 기술 용어 없이 답할 수 있는 인터뷰를 통해 앱 기획을 구체화하고, 경쟁사 조사 기반의 실행 가능한 PRD와 프로젝트 문서 구조를 생성합니다.

## Workflow

| Phase | 내용 |
|-------|------|
| 1 | 앱 정체 파악 (이름, 기능, 타겟, 플랫폼) |
| 2 | 기능·디자인 구체화 (데이터, 계정, 결제, AI, 알림 등) |
| 3 | 배포 & 개발 방식 |
| 4 | 경쟁사 조사 (web_search + web_fetch) |
| 5 | 차별화 전략 도출 |
| 6 | PRD 작성 + 프로젝트 문서 구조 생성 |

## Output

- **PRD 문서** (20개 섹션): 문제 정의, 경쟁사 분석, 차별화, DB 스키마, API 설계, 마일스톤, 수익 모델, KPI, 리스크 등
- **프로젝트 문서 구조**: README, CLAUDE.md, docs/ 하위 문서 (AUTH, DB, BILLING, AI_SYSTEMS 등 필요한 것만)

## Installation

```bash
# Claude Code에서
/install-skill https://github.com/Tygb99/app-builder-skill.git
```

또는 수동으로:

```bash
git clone https://github.com/Tygb99/app-builder-skill.git
cp -r app-builder-skill ~/.claude/skills/app-builder
```

## Usage

Claude Code에서 아래와 같이 말하면 자동으로 트리거됩니다:

- "앱 만들고 싶어"
- "PRD 만들어줘"
- "새 프로젝트 시작"
- "서비스 기획해줘"
- "사이드 프로젝트 기획"

## Structure

```
app-builder/
├── SKILL.md                          # 메인 스킬 정의
├── README.md
├── references/
│   └── prd-template.md               # PRD 템플릿
└── principles/
    └── DOCS_PRINCIPLES.md            # 문서 구조 원칙
```

## License

MIT
