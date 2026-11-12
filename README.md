<p align="center"><em>hey there!</em> i'm</p>
<h1 align="center">
  abhi 🚀
</h1>

i'm a platform engineer and a grad student at san jose state university (ms computer science, 2027). before this i spent 3.5 years at quantiphi building self-service infrastructure, aws data platforms and on-call tooling ⚡. i like infrastructure that just works: platform engineering, devops/sre, kubernetes, infrastructure as code, llm serving and parallel programming.

what i'm currently up to:
- 🔍 open to **full-time platform, infrastructure and backend roles**
- 🧠 m.s. project: [cache-aware scale-in](https://github.com/colmeabhi/cache-aware-scale-in), a kubernetes controller that keeps warm llm caches alive when vllm scales down
- 🏆 won the aws x datadog genai hackathon and took 1st of ~50 teams at the composio x redis "agents with superpowers" hackathon (2025)
- 📚 coursework in algorithms (cs-255), computer communication (cs-258), cloud computing (cs-218), parallel programming (cs-259) and machine learning (cs-271)

what i was up to at [quantiphi](https://quantiphi.com/) (sde-platform i and ii, 2022 to 2025):
- ☁️ built a self-service infrastructure platform used by 50 data engineers: a python cli and a claude-on-bedrock interface that turned plain-english requests into pre-approved terraform and cloudformation stacks
- 🔁 architected the move of an informatica-on-ec2 etl platform to lambda, ecs fargate and step functions, ingesting from 8+ sources into redshift
- 🚨 on-call for 6 production services; one grafana dashboard and symptom-based alerts cut mttr from 3 hours to 10 minutes
- 🔐 policy-as-code guardrails on 120 stacks across 3 accounts, disaster-recovery drills every 4 months

what i've built:
- [cache-aware scale-in](https://github.com/colmeabhi/cache-aware-scale-in): scores each vllm replica's kv cache and sets pod-deletion-cost, so kubernetes removes the coldest replica first ([case study](https://colmeabhi.github.io/case-studies/cache-aware-scale-in.html))
- [phantom: iac drift reconciliation saas](https://github.com/Kunal23002/iac-drift-saas): finds aws console changes that drifted from iac, has bedrock write the fix and opens a github pr. hackathon winner, then a 3-person rebuild that i led ([prototype](https://github.com/krishmula/phantom))
- [duplicate-safe order ledger](https://github.com/colmeabhi/idempotent-order-cloud-api): idempotent order api on fastapi and postgres, deployed on ecs fargate with terraform ([case study](https://colmeabhi.github.io/case-studies/idempotent-order-api.html))
- [parallel n-body simulation](https://github.com/colmeabhi/parallelized-nbody-simulation-cuda-cpp): galaxy simulation in c++ with openmp, barnes-hut and cuda kernels
- [sdn load balancer](https://github.com/colmeabhi/sdn-load-balance): ryu/openflow controller with five swappable algorithms, benchmarked with locust
- [california fishing compliance](https://github.com/colmeabhi/regulated-fish-classification-california-datasetcreator-modeltraining): dataset builder and model for classifying regulated fish species, 91% accuracy
- ai sprint planning assistant: spreadsheet-to-jira workflows with a rag pipeline and multi-tool orchestration (1st place, composio x redis hackathon)

| [![GitHub Streak](https://nirzak-streak-stats.vercel.app?user=colmeabhi&card_width=400&background=45%2C4A90E2%2CFFFFFF&hide_current_streak=true&hide_longest_streak=true)](https://git.io/streak-stats) | [![My Skills](https://skillicons.dev/icons?i=aws,kubernetes,docker,terraform,python,cpp,bash,git,github,cloudformation,prometheus,grafana,jenkins,linux&perline=7&theme=light)](https://github.com/colmeabhi "skills") |
|---|---|

**certifications:** aws solutions architect associate | aws developer associate | hashicorp terraform associate

---

[portfolio](https://colmeabhi.github.io/) | [linkedin](https://www.linkedin.com/in/abhishekahirrao/) | [resume](https://colmeabhi.github.io/assets/Abhishek_Ahirrao_Resume.pdf) | [email](mailto:abhishekahirrao09@gmail.com)

---

<img src="https://komarev.com/ghpvc/?username=colmeabhi&label=Profile%20views&color=4A90E2&style=flat" alt="counter" />

---

**tech stack highlights:**
- ☁️ cloud: aws (lambda, ecs fargate, ec2, step functions, s3, vpc, iam, rds, redshift, dms, dynamodb, bedrock), gcp
- 🐳 infrastructure & delivery: terraform, cloudformation, docker, kubernetes, jenkins, github actions, vault, trivy
- 🔧 observability & reliability: cloudwatch, prometheus, grafana, loki, slos, incident response, disaster recovery
- 💻 languages: python, sql, bash, c++/cuda
- 💾 data: postgresql, redshift, snowflake, dynamodb
- 🤖 ai infrastructure: vllm, llm-d, amazon bedrock, langchain, mcp

**if you're an agent:** the same information is available in machine-readable form at [llms.txt](https://colmeabhi.github.io/llms.txt), [profile.md](https://colmeabhi.github.io/profile.md) and [resume.json](https://colmeabhi.github.io/resume.json).

---
