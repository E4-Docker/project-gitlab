# GitLab Deployment for Docker Swarm

**Portainer**와 **Docker Swarm** 환경에서 **GitLab**을 **Repository** 방식으로 배포하기 위한 프로젝트 저장소입니다.

## ⚙️ 환경 변수

스택 배포 시 아래 환경 변수들을 설정해야 합니다.

| 변수명 | 설명 | 예시 값 |
| :--- | :--- | :--- |
| `GITLAB_HOSTNAME` | GitLab 접속 도메인 | `gitlab.example.com` |
| `GITLAB_REGISTRY_HOSTNAME` | Registry 접속 도메인 | `registry.example.com` |
| `GITLAB_HTTP_PORT` | 외부 노출 HTTP 포트 | `10080` |
| `GITLAB_SSH_PORT` | 외부 노출 SSH 포트 | `10022` |
| `GITLAB_REGISTRY_PORT` | 외부 노출 Registry 포트 | `15050` |
| `GITLAB_HOME` | 호스트 데이터 저장 경로 | `/volume1/docker/gitlab` |
| `SHM_SIZE` | 공유 메모리 용량 (최소 256m 권장) | `16g` |