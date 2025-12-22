---
{"publish":true,"title":"hjahn.kr","created":"2025-12-22T15:13:12.574+09:00","modified":"2025-12-22T16:01:58.546+09:00","cssclasses":""}
---

> [!warning] In-development
> This blog is currently in-development.

## Check AnyBlock plugin
[timeline]
- 2000-07-12
	- birth
- 2025-12-22
	- now

[node]
- node 1
	- node 2
	- node 3

[mermaid]
- a
	- b
- b
	- c
- c
	- a

## Check Dataview for non-visible files

| File                                                                                                                                                                                                                   | research question                                                                                                                                         | method                                                                                                                             | findings                                                                                                                                         | limits                                                                                                                           |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| [[1. Project/Research/Human Agent Interaction/papers/RepoGraph- Enhancing AI Software Engineering with Repository-level Code Graph\|RepoGraph- Enhancing AI Software Engineering with Repository-level Code Graph]] | 어떻게 하면 LLM이 전체 코드 저장소의 복잡한 구조와 의존성을 효과적으로 이해하고 탐색하여, 실제 소프트웨어 문제(repository-level)를 더 잘 해결하게 할 수 있을까?                                                     | 1️⃣ 각 코드 라인을 노드로, 각 라인 간의 dependency를 링크로 하여 그래프를 생성하여 repository 정보를 구축 2️⃣ 특정 상황에 필요한 노드를 검색한 뒤 llm에게 해당 노드 중심으로 k개 flatten해서 입력 | 1️⃣ SWE-bench 결과 RAG, Agentless 논문, SWE-agent 등에 적용(해당 방법에서의 llm 입력으로 그래프 정보 추가) 했을 때, 과도한 비용 증가 없이 성능 향상 2️⃣ 문제 해결을 위한 파일 localization에 뛰어남을 보임 | dependency만 고려해도 모든 이슈를 처리할 수 있을까? dependency로 연결되지 않아도 한 이슈를 해결하는데 고려해야 할 요소들이 있지 않을까?                                          |
| [[1. Project/Research/Human Agent Interaction/papers/Agentless- Demystifying LLM-based Software Engineering Agents\|Agentless- Demystifying LLM-based Software Engineering Agents]]                                 | 복잡한 agent-based의 software engineering 대신 단계별 프로세스를 잘 정의해서 해결할 수는 없을까?                                                                                     | LLM이 행동을 결정하는 대신, localization, repair, patch validation의 3 단계를 명시적으로 수행하는 Agentless 프레임워크를 개발함                                    | 1️⃣ SWE-bench Lite benchmark에서 기존 오픈소스 agent 기반 방식들보다 적은 비용을 사용하면서 성능 향상 2️⃣ SWE-bench Lite 벤치마크에 존재하던 문제를 발견하여, 그를 수정하고 SWE-bench Lite-S 배포     | high level의 구조로 repository를 분석했다기보다는, 파일 하나 하나를 별개로 보고 어떻게 검색을 할지에 집중함. file structure 말고 repository를 표현하기 위해 필요한 정보들이 더 있지 않을까? |
| [[1. Project/Research/Human Agent Interaction/papers/SWE-agent- Agent-Computer Interfaces Enable Automated Software Engineering\|SWE-agent- Agent-Computer Interfaces Enable Automated Software Engineering]]       | agent들이 linux shell, python interpreter 등 큰 action space의 것들을 직접 이용하기보다, 사람이 vs code를 사용하는 것처럼 agent를 위한 tool들을 제공해준다면 실제 소프트웨어 공학 문제들을 더 잘 해결할 수 있지 않을까? | 사람이 Computer와 상호작용하며 해결하듯, Agent도 Computer와 상호작용하기 위한 간단한 인터페이스인 ACI를 정의하여 Agent에게 제공함                                             | 1️⃣ SWE-bench에서 GPT-4 Turbo를 base로 RAG 기반 기존 시스템 3.8% 보다 12.47%로 성능 향상 2️⃣ linux shell만을 사용하는 방법보다 ACI로 10.7 퍼센트 포인트 향상                          | \-                                                                                                                               |


## Check non-visible base link with preview
![[Research Base.base]]

## Check non-visible PDF preview

![[1. Project/Research/Human Agent Interaction/papers/pdfs/RepoGraph- Enhancing AI Software Engineering with Repository-level Code Graph.pdf]]