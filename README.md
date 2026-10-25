<div align="center">

# 이동현 · Backhacandy

**AI 에이전트와 함께 데스크톱 앱과 게임을 만드는 개발자**<br>
*A developer building desktop apps and games together with AI agents*

<br>

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte_5-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri_2-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Unity](https://img.shields.io/badge/Unity_6-000000?style=flat-square&logo=unity&logoColor=white)

📫 backha.candy0101@gmail.com

</div>

---

## 🇰🇷 소개

평소에 쓰다가 불편했던 것을 직접 도구로 만들고, 그 도구로 다시 더 큰 것을 만듭니다.
요즘은 여러 AI 코딩 에이전트가 한 프로젝트를 **나눠서 동시에** 개발하게 하는 방법에 관심이 많습니다.

### 프로젝트

#### 🧠 AITermHub — 여러 AI 코딩 에이전트를 한 창에서
`Tauri 2` `Rust` `SvelteKit` `Svelte 5` `TypeScript` · 저장소 비공개(정리 후 공개 예정)

Claude Code·Codex를 탭으로 돌리고, 한 프로젝트를 여러 에이전트가 나눠 동시에 개발하게 하는 Windows 데스크톱 앱입니다.
- **팀 탭**: 에이전트 N명이 같은 폴더에서 담당 경로(glob)를 나눠 동시에 작업합니다. 3명 이상이면 가벼운 모델이 지시를 칸별 몫으로 나누고, 인계 메모와 "요청"을 서로 전달하며, 남의 영역을 고치면 경고합니다.
- **AI 회사 모드**: 총괄 모델이 티켓을 나누고, git worktree에서 작업한 뒤, 다른 회사 모델이 교차 리뷰합니다. GitHub 이슈·PR로 원격 팀원에게 맡길 수도 있습니다.
- **쉬는 에이전트 메모리 ≈ 0 MB**: 프로세스를 끄지 않고 일시정지해 메모리만 반납하므로, 프롬프트 캐시가 유지되어 토큰 손해가 없습니다.
- 계정 여러 개 자동 전환, 실시간 코드 뷰와 줄 단위 리뷰, 스트림 이벤트를 모아 처리해 렉 제거
- 커밋 130여 개 · 코드 약 2.6만 줄 · 테스트 300여 개(vitest + cargo)

#### ⚔️ 마나 흐름 (OpenWorldRPG) — 2D 액션 RPG
`Unity 6` `URP 2D` `C#` · Windows · Android · 저장소 비공개(정리 후 공개 예정)

탑다운 2D 오픈월드 액션 RPG입니다. v1.7까지 만들었습니다.
- 3단 콤보·강공격·**패링**·**완벽 회피와 환영 반격**·필살기, 파티 3인 교체와 협주 공격
- 제작·요리·건축·낚시·채집·동물 친구 같은 생활 콘텐츠, 이야기 수첩·몬스터 도감·업적
- 2D 조명과 후처리, 자유 시점·입체(2.5D)·1인칭 시점, 날씨
- 유니티 없이 바로 들어가는 개발자 모드, PlayMode 자동 테스트
- C# 파일 285개 · 약 6.3만 줄

<sub>게임 아이디어는 사지방 개발자(@dev_in_airforce)의 릴스를 참고했고, 코드는 직접 구현했습니다. 그래픽은 Ninja Adventure 에셋 팩(CC0)을 사용했습니다.</sub>

#### 🗓️ DeskMate — 바탕화면 일정·과제 위젯
`Tauri 2` `Rust` `SvelteKit` `TypeScript` · 저장소 비공개(정리 후 공개 예정)

바탕화면에 붙어 있는 대학생용 일정·과제 대시보드입니다.
- 학교 **이클래스 연동**: 앱 안 브라우저로 로그인하고, 할 일·마감을 가져오고, 제출 여부를 감지합니다. 세션이 만료되면 자동으로 다시 로그인합니다.
- 과제·루틴 알림(마감이 가까울수록 단계적으로), 주간·월간 캘린더, D-day, 포모도로와 일일 집계, 메모, 배경 테마
- 코드 약 5,000줄

---

## 🇺🇸 About

I build tools for things that bother me in daily work, then use those tools to build bigger things.
Lately I'm focused on getting several AI coding agents to develop one project **in parallel**.

### Projects

#### 🧠 AITermHub — many AI coding agents in one window
`Tauri 2` `Rust` `SvelteKit` `Svelte 5` `TypeScript` · private repo (to be published)

A Windows desktop app that runs Claude Code and Codex as tabs and lets several agents build one project at the same time.
- **Team tab**: N agents share a folder and own glob-based paths. With 3+ agents, a lightweight model splits each instruction into per-agent tasks; handoff notes and requests are routed between agents, and edits outside one's area raise a warning.
- **AI Company mode**: a lead model plans tickets, workers run in git worktrees, and a model from another vendor cross-reviews. Tickets can be delegated to remote teammates via GitHub issues and PRs.
- **≈ 0 MB idle memory**: idle agents are suspended instead of restarted, so the prompt cache stays warm and no tokens are wasted.
- Account rotation on usage limits, a live code view with line-level review, and batched stream rendering for a smooth UI
- 130+ commits · ~26k lines · 300+ tests (vitest + cargo)

#### ⚔️ ManaFlow (OpenWorldRPG) — 2D action RPG
`Unity 6` `URP 2D` `C#` · Windows · Android · private repo (to be published)

A top-down 2D open-world action RPG, currently at v1.7.
- 3-hit combos, heavy attacks, **parry**, **perfect dodge with phantom counter**, ultimates, 3-character party swapping
- Life content: crafting, cooking, building, fishing, gathering, pets; story journal, bestiary, achievements
- 2D lighting and post-processing, free camera, 2.5D and first-person views, weather
- A developer mode that boots straight into the game without the Unity editor, plus automated PlayMode tests
- 285 C# files · ~63k lines

<sub>The game idea was inspired by reels from @dev_in_airforce; all code is my own implementation. Art uses the Ninja Adventure asset pack (CC0).</sub>

#### 🗓️ DeskMate — desktop schedule & assignment widget
`Tauri 2` `Rust` `SvelteKit` `TypeScript` · private repo (to be published)

A dashboard pinned to the desktop for university students.
- **University e-class integration**: logs in through an in-app browser, fetches to-dos and deadlines, detects submissions, and re-logs in automatically when the session expires
- Escalating reminders for assignments and routines, weekly and monthly calendar, D-day, Pomodoro with daily totals, memo, background themes
- ~5,000 lines
