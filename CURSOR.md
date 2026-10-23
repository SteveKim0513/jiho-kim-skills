# Cursor에서 쓰기

이 저장소에는 **Cursor 프로젝트 규칙**이 들어 있어서, 여기서 작업하면 지침이 자동으로 적용된다.

## 이 저장소 안에서

1. Cursor로 폴더를 연다.
2. [`.cursor/rules/jiho-kim-guidelines.mdc`](.cursor/rules/jiho-kim-guidelines.mdc)가 `alwaysApply: true`로 커밋돼 있어 따로 설치할 게 없다.
3. **Settings → Rules**에서 `jiho-kim-guidelines`가 보이면 된다.

## 다른 프로젝트에서 쓰기

**Cursor (권장):** `.cursor/rules/jiho-kim-guidelines.mdc`를 그 프로젝트의 `.cursor/rules/`에 복사한다. 기존 규칙과 합쳐도 된다.

**다른 도구:** 루트 지침 파일만 읽는 도구라면 [`CLAUDE.md`](CLAUDE.md)를 복사하거나 기존 지침에 덧붙인다.

## 개인 스킬로 쓰기

`~/.cursor/skills` 아래에 재사용 스킬로 두려면 [`skills/jiho-kim-guidelines/SKILL.md`](skills/jiho-kim-guidelines/SKILL.md)를 복사하거나 심볼릭 링크한다.

## Claude Code와 Cursor

- **Claude Code:** [`README.md`](README.md)의 플러그인 설치 방법을 따른다. 프로젝트별로는 `CLAUDE.md`를 쓴다.
- **Cursor:** 위의 `.cursor/rules/` 파일을 쓴다. Cursor는 `.claude-plugin/`과 `CLAUDE.md`를 기본으로 읽지 않는다.

## 고칠 때

원칙을 바꾸면 세 파일을 함께 고친다: [`CLAUDE.md`](CLAUDE.md), [`.cursor/rules/jiho-kim-guidelines.mdc`](.cursor/rules/jiho-kim-guidelines.mdc), [`skills/jiho-kim-guidelines/SKILL.md`](skills/jiho-kim-guidelines/SKILL.md). 본문은 항상 같아야 한다.
