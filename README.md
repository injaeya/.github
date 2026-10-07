# .github — 공통 양식 저장소

이 저장소는 코드가 아니라 **양식**을 둡니다. GitHub는 여기 있는 파일을 **자기 양식이 없는 모든 저장소의 기본값**으로 씁니다.

| 파일 | 역할 |
|---|---|
| `.github/ISSUE_TEMPLATE/bug.yml` · `feature.yml` · `docs.yml` · `decision.yml` | 이슈를 만들 때 고르는 양식 4종 |
| `.github/ISSUE_TEMPLATE/config.yml` | 빈 이슈 금지, 규칙 링크 |
| `PULL_REQUEST_TEMPLATE.md` | PR 본문 기본 양식(다섯 칸 + 티어) |
| `CONTRIBUTING.md` | 일하는 방식 한 장 요약 |

## 저장소별로 다르게 쓰고 싶으면

무엇을 바꾸느냐에 따라 대체되는 단위가 다릅니다.

- **이슈 양식은 폴더 통째로 대체됩니다.** 그 저장소의 `.github/ISSUE_TEMPLATE/` 에 양식이나 `config.yml` 이 **하나라도** 있으면, 여기 공통 양식 4종과 `config.yml` 은 **전부** 쓰이지 않습니다. 파일 이름이 같은지와는 상관없습니다. 하나만 덧붙이려다 나머지가 조용히 사라지니, 바꾸려면 여기 `.github/ISSUE_TEMPLATE/` 의 파일 5개를 **모두** 복사해 와서 고치세요.
- **PR 양식·`CONTRIBUTING.md` 같은 나머지 파일은 파일 단위입니다.** 그 저장소에 **같은 이름의 파일**을 두면 그 파일만 그쪽이 우선합니다. 단 **덧붙이기가 아니라 바꿔치기**입니다 — 여기 파일을 복사해 와서 고치세요.

어느 쪽이든 복사해서 고쳐야 필수 칸(수용 기준·`Closes #N`·티어)이 빠지지 않습니다.
근거: [GitHub 문서 — 기본 커뮤니티 건강 파일 만들기](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)

## 고칠 때

이 저장소는 코드 프로젝트가 아니라 git-flow(develop/release)를 쓰지 않습니다. `main` 하나에 PR로 반영합니다. 양식을 바꾸면 그 순간부터 모든 저장소에 적용되니, 바꾸기 전에 리더 세션에서 규칙과 어긋나지 않는지 확인합니다.

_제정 2026-09-07 · 근거 = 전역 작업 규칙 §7 (git-flow · Conventional Commits 1.0.0 · SemVer 2.0.0)_
