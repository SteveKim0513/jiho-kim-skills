# jiho-kim-skills 작업 규칙

AI 에이전트 행동 지침을 배포하는 공개 저장소다. 루트 `CLAUDE.md`는 이 저장소의 작업 규칙이 아니라 제품(사용자가 `curl`로 받아 붙이는 지침)이라, 이 파일에 작업 규칙을 둔다.

공통 개발 규칙(일하는 법·코드 규칙·팀 원칙·스킬)은 스튜디오 플러그인 팀 문서가 맡는다. 이 문서는 이 프로젝트의 값만 둔다.

- 루트 `CLAUDE.md`와 `skills/jiho-kim-guidelines/SKILL.md`의 본문은 같아야 한다. 하나를 고치면 둘을 함께 고친다.
- 판을 올릴 때 `.claude-plugin/plugin.json`의 `version`과 `.claude-plugin/marketplace.json`의 `metadata.version`·`plugins[0].version`을 같은 값으로 올린다.
