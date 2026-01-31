# OpenClaw Workspace

이 저장소는 OpenClaw 에이전트의 워크스페이스입니다. 여기서 에이전트의 페르소나, 지침, 그리고 커스텀 기술(Skills)을 관리합니다.

## 시스템 설정과 연결하기

이 디렉토리를 OpenClaw의 공식 워크스페이스로 사용하려면 다음 단계를 따르세요:

1. `~/.openclaw/openclaw.json` 파일을 열고 `agents.defaults.workspace` 경로를 이 디렉토리의 절대 경로로 수정합니다:

```json
{
  "agents": {
    "defaults": {
      "workspace": "/Users/jang-kyoung-yoon/Documents/openclaw_work"
    }
  }
}
```

2. (또는) 심볼릭 링크를 사용하여 기존 워크스페이스 위치를 이 폴더로 연결할 수도 있습니다:

```zsh
rm -rf ~/.openclaw/workspace
ln -s /Users/jang-kyoung-yoon/Documents/openclaw_work ~/.openclaw/workspace
```

## 주요 파일 안내

- `AGENTS.md`: 에이전트의 역할과 지침 정의
- `SOUL.md`: 에이전트의 성격(Persona) 정의
- `TOOLS.md`: 커스텀 도구 정의
- `skills/`: 커스텀 기술들을 담는 폴더
