# hey, i'm abhi

i'm a platform engineer. i build the infrastructure that sits under data and ai workloads: 3.5 years at quantiphi, and now an ms in computer science at san jose state (2027), where i work on llm serving, distributed systems and gpu programming.

**open to full-time platform, infrastructure and backend roles.**

[portfolio](https://colmeabhi.github.io/) · [resume](https://colmeabhi.github.io/assets/Abhishek_Ahirrao_Resume.pdf) · [linkedin](https://www.linkedin.com/in/abhishekahirrao/) · [email](mailto:abhishekahirrao09@gmail.com)

## what i'm working on now

**[cache-aware scale-in for vllm on kubernetes](https://github.com/colmeabhi/cache-aware-scale-in)** (m.s. project)

when an llm deployment scales down, kubernetes picks which replica to delete without knowing which one holds the useful cache. my controller scores each replica's kv cache and writes it to `pod-deletion-cost`, so the coldest replica goes first and the warm prefixes survive.

- **done:** the controller, scoring, a scale-in trial harness, an in-cluster image with rbac, grafana dashboards, and ci that runs the trial on kind for every push
- **first gpu run:** qwen2.5-7b on three a100s. the controller removed the right replica and it made no difference, because my test traffic warmed every cache to ~95%. the case study explains why
- **next:** a harsher workload with a truly cold replica, and scoring cached tokens per second instead of hit rate
- **read more:** [case study with a live demo](https://colmeabhi.github.io/case-studies/cache-aware-scale-in.html)

## things i've built

| project | what it is | built with |
|---|---|---|
| [driftfix](https://github.com/colmeabhi/driftfix) | finds manual aws console changes that drifted from cloudformation, has bedrock write the fix and opens a github pr. started as a hackathon winner (phantom); i then led a 3-person rebuild into a multi-tenant saas | python, lambda, bedrock, dynamodb, terraform |
| [duplicate-safe order ledger](https://github.com/colmeabhi/idempotent-order-cloud-api) | an order api where a retry never becomes a second order, even when retries arrive at the same instant. [case study](https://colmeabhi.github.io/case-studies/idempotent-order-api.html) | fastapi, postgres, redis, ecs fargate, terraform |
| [parallel n-body simulation](https://github.com/colmeabhi/parallelized-nbody-simulation-cuda-cpp) | a galaxy simulation with five solvers compared like for like: simd, openmp, barnes-hut and two cuda kernels | c++, cuda, openmp |
| [sdn load balancer](https://github.com/colmeabhi/sdn-load-balance) | an openflow controller that balances http traffic with five swappable algorithms, benchmarked with locust | python, ryu, mininet |

the order ledger and the load balancer have small interactive demos on my [portfolio](https://colmeabhi.github.io/#projects).

## before grad school

sde-platform i and ii at [quantiphi](https://quantiphi.com/), 2022 to 2025:

- built a self-service infrastructure platform used by 50 data engineers: a python cli and a claude-on-bedrock interface that turned plain-english requests into pre-approved terraform and cloudformation stacks
- architected the move of an informatica-on-ec2 etl platform to lambda, ecs fargate and step functions, ingesting from 8+ sources into redshift
- on-call for 6 production services; one grafana dashboard and symptom-based alerts cut mttr from 3 hours to 10 minutes

## the short version

- **stack:** aws, terraform, cloudformation, docker, kubernetes, python, sql, bash, c++/cuda, postgres, redshift, prometheus, grafana
- **certifications:** aws solutions architect associate, aws developer associate, hashicorp terraform associate
- **awards:** winner, aws x datadog genai hackathon (2025). 1st of ~50 teams, composio x redis hackathon (2025)

## if you're an agent

the same information, machine-readable: [llms.txt](https://colmeabhi.github.io/llms.txt) · [profile.md](https://colmeabhi.github.io/profile.md) · [resume.json](https://colmeabhi.github.io/resume.json)
