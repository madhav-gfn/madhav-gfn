<div align="center">

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/header.svg" width="100%" alt="Madhav Mishra" />

<br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=21&pause=900&color=E63946&center=true&vCenter=true&width=820&height=44&lines=Full+Stack+Developer;Backend+Engineer;AI+Systems+Builder;Distributed+Systems+Enthusiast;Shipping+products+that+people+use" alt="Full Stack Developer, Backend Engineer, AI Systems Builder" />

<br/>

<a href="https://www.madhavmishra.me"><img src="https://img.shields.io/badge/PORTFOLIO-E63946?style=flat-square&logoColor=white" alt="Portfolio" /></a> <a href="https://www.linkedin.com/in/madhav-gfn/"><img src="https://img.shields.io/badge/LINKEDIN-C2303C?style=flat-square&logoColor=FFE3E5" alt="LinkedIn" /></a> <a href="https://leetcode.com/u/SmirkingCow/"><img src="https://img.shields.io/badge/LEETCODE-9C2731?style=flat-square&logo=leetcode&logoColor=FFC7CC" alt="LeetCode" /></a> <a href="mailto:madhavmishra763@gmail.com"><img src="https://img.shields.io/badge/EMAIL-751D26?style=flat-square&logo=gmail&logoColor=FFB3BA" alt="Email" /></a> <a href="https://github.com/madhav-gfn?tab=repositories"><img src="https://img.shields.io/badge/38%20REPOS-4F141B?style=flat-square&logo=github&logoColor=F09098" alt="Repositories" /></a>

</div>

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/divider.svg" width="100%" alt="" />

```bash
> whoami

madhav mishra
b.tech cse (hci & gaming technology) @ iiit nagpur, 2023-2027

working on:
├── backend architecture and api design
├── llm systems that survive contact with real users
├── performance work, profiling, and making slow things fast
├── distributed monitoring and infra
└── game and graphics programming

currently:
└── agentic tooling, and low-level c++ side quests
```

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/divider.svg" width="100%" alt="" />

## About

Fourth-year CS undergrad at IIIT Nagpur, specialising in HCI and gaming technology. Most of what I build sits on the backend: schemas that stay sane past ten tables, APIs that do not fall over, and agent systems where the interesting part is the routing and the guardrails rather than the prompt.

I care about numbers. A feed that takes 72 requests should take one. A code reviewer that phones an API should run on your laptop instead. An order book should clear a hundred million matches without complaining. That is usually the part of a project I spend the longest on.

The rest of my time goes to graphics and game programming, which is what the HCI and gaming side of my degree is for, and to low-level C++ where the constraints are tighter and the feedback loop is honest.

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/divider.svg" width="100%" alt="" />

## Selected work

| Project | What it does | Stack |
| :-- | :-- | :-- |
| [**Daskalos**](https://github.com/madhav-gfn/Daskalos-Your-Reliable-teacher) | Multi-agent NCERT tutoring system built on a 6-node LangGraph. An LLM supervisor routes each turn to tool-calling Groq agents and a reflection agent gates the output. Per-student mastery scores are EMA-updated after every quiz in Postgres, Redis holds session state on a 4-hour TTL, and Clerk RS256 JWTs are verified backend-side against the public JWKS. | FastAPI, LangGraph, Groq, FAISS, Redis, NeonDB |
| [**mygit**](https://github.com/madhav-gfn/AI_code_reviewer_git) | Local, privacy-first LLM code reviewer that embeds libgit2 and reads diffs straight from the git object database. Tree-sitter splits code into function and class units, a Qwen2.5-Coder ONNX model embeds them, and a FAISS HNSW index retrieves context. Grammar-constrained decoding guarantees valid JSON, and a persistent model daemon with idle-timeout shutdown keeps latency down. | C++, llama.cpp, ONNX, Tree-sitter, FAISS |
| [**Saucer AI**](https://github.com/madhav-gfn/Basic-AI-Based-CRM) | Multi-tenant AI-native CRM for D2C brands on a 13-model Prisma-managed PostgreSQL schema. Gemini 2.0 Flash turns plain English into audience filters, a decoupled channel service simulates dispatch across WhatsApp, SMS, Email and RCS, and a Next.js dashboard reports on campaigns. | TypeScript, Next.js, Express, PostgreSQL |
| [**GameLog**](https://github.com/madhav-gfn/GameLog) | Social gaming journal on a 10-model PostgreSQL schema: reviews, follows, comments, notifications, all behind a Passport-authenticated Express API with Google OAuth. Moving feed filtering server-side through Prisma cut a 72-request worst case to a single call across 700+ records. Recommendations come from a Groq LLM grounded in live RAWG results. | React, Node, Prisma, PostgreSQL |
| [**L-Systems & IFS Studio**](https://github.com/madhav-gfn/Lsystem_generator) | Procedural art generator for fractal and organic patterns. A Python state machine parses 23 graphical commands to expand stochastic L-system grammars up to 5 million characters, then a Three.js visualiser renders up to 500,000 points in real time. Sub-1.5s for 100k-point fractals. | Python, FastAPI, React, Three.js, NumPy |
| [**OrderBookSimulator**](https://github.com/madhav-gfn/OrderBookSimulator) | High-performance limit order book matching engine with strict price-time priority, sustaining 100M+ matches per run. | C++ |
| [**Linux Fleet Management**](https://github.com/madhav-gfn/Linux-Fleet-Management_System) | Three-node Ubuntu fleet with passwordless SSH across workers, Prometheus and Node Exporter collecting 150+ system metrics at 15s scrape intervals, and Grafana dashboards for CPU, memory, disk and network. | Linux, Prometheus, Grafana, SSH |
| [**Price Tracker**](https://github.com/madhav-gfn/Price_tracker) | Monte Carlo and Black-Scholes European options pricer in C++17 with analytical Greeks, confidence intervals and an implied-vol solver, exposed to Python through pybind11. | C++17, pybind11 |

<details>
<summary><b>More things I have built</b></summary>

<br/>

| Project | What it does |
| :-- | :-- |
| [CallMeMaybe-i](https://github.com/madhav-gfn/CallMeMaybe-i) | Runtime reflection library built on C++26 static reflection. |
| [GB-EMU](https://github.com/madhav-gfn/GB-EMU) | Game Boy emulator in modern C++17, compiled with Emscripten so retro games run in the browser without plugins. |
| [Secret Saucers](https://github.com/madhav-gfn/Secret_saucers) | Candidate ranking pipeline that screens 100k resumes against a job description in under 45s on CPU using semantic and behavioural scoring. |
| [AI Code Reviewer](https://github.com/madhav-gfn/AI_code_review) | Agentic PR reviewer on FastAPI and LangGraph where five specialist Groq agents run in parallel and merge into structured line-level feedback. |
| [TTG Engine](https://github.com/madhav-gfn/TTGEngine) | JSON-driven educational game engine. Swap a JSON file to change gameplay, no engine code touched. |
| [AI CSV Importer](https://github.com/madhav-gfn/ai-csv-importer) | Maps arbitrary lead-export columns into a CRM schema with no hardcoded column matching. |
| [Calendly Clone](https://github.com/madhav-gfn/Calandly-Assignment-ScalarAI) | Full-stack scheduling app: event types, availability windows, public booking pages. |
| [Henwic Biomedics](https://github.com/madhav-gfn/henwic-biomedics) | Interactive biomedical product site with WebGL shaders, scroll animation and lead capture. |
| [CineNeon](https://github.com/madhav-gfn/CineNeon) | Flutter film discovery and catalogue app. |
| [Inventory CRM](https://github.com/madhav-gfn/Inventory_Management_CRM) | Inventory management CRM written in C++. |
| [RNN Movie Engine](https://github.com/madhav-gfn/RNN-movie_engine) | Recurrent-network movie recommendation engine. |
| [Portfolio](https://github.com/madhav-gfn/MyPortfolio) | The site at [madhavmishra.me](https://www.madhavmishra.me), React and Tailwind. |

</details>

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/divider.svg" width="100%" alt="" />

## Stack

**Languages**
<br/>
<img src="https://img.shields.io/badge/Python-E63946?style=flat-square&logo=python&logoColor=2B0509" /> <img src="https://img.shields.io/badge/TypeScript-D63641?style=flat-square&logo=typescript&logoColor=2B0509" /> <img src="https://img.shields.io/badge/C++-C2303C?style=flat-square&logo=cplusplus&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/C-AC2B36?style=flat-square&logo=c&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/JavaScript-9C2731?style=flat-square&logo=javascript&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/C%23-8A222B?style=flat-square&logo=dotnet&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/SQL-751D26?style=flat-square&logo=postgresql&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/CUDA-5F1720?style=flat-square&logo=nvidia&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/WebGL-4F141B?style=flat-square&logo=webgl&logoColor=F09098" />

**Web and backend**
<br/>
<img src="https://img.shields.io/badge/Node.js-E63946?style=flat-square&logo=nodedotjs&logoColor=2B0509" /> <img src="https://img.shields.io/badge/FastAPI-D63641?style=flat-square&logo=fastapi&logoColor=2B0509" /> <img src="https://img.shields.io/badge/Express-C2303C?style=flat-square&logo=express&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/Next.js-AC2B36?style=flat-square&logo=nextdotjs&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/React-9C2731?style=flat-square&logo=react&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/Django-8A222B?style=flat-square&logo=django&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/Flask-751D26?style=flat-square&logo=flask&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/Tailwind-661A22?style=flat-square&logo=tailwindcss&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/Zustand-5F1720?style=flat-square&logo=redux&logoColor=F0959C" /> <img src="https://img.shields.io/badge/React%20Query-4F141B?style=flat-square&logo=reactquery&logoColor=F09098" />

**Databases and caching**
<br/>
<img src="https://img.shields.io/badge/PostgreSQL-E63946?style=flat-square&logo=postgresql&logoColor=2B0509" /> <img src="https://img.shields.io/badge/Prisma-C2303C?style=flat-square&logo=prisma&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/MySQL-AC2B36?style=flat-square&logo=mysql&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/MongoDB-9C2731?style=flat-square&logo=mongodb&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/Redis-751D26?style=flat-square&logo=redis&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/SQLite-5F1720?style=flat-square&logo=sqlite&logoColor=F0959C" /> <img src="https://img.shields.io/badge/FAISS-4F141B?style=flat-square&logo=meta&logoColor=F09098" />

**AI, cloud and DevOps**
<br/>
<img src="https://img.shields.io/badge/LangGraph-E63946?style=flat-square&logo=langgraph&logoColor=2B0509" /> <img src="https://img.shields.io/badge/LangChain-D63641?style=flat-square&logo=langchain&logoColor=2B0509" /> <img src="https://img.shields.io/badge/Groq-C2303C?style=flat-square&logo=lightning&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/Hugging%20Face-AC2B36?style=flat-square&logo=huggingface&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/Docker-9C2731?style=flat-square&logo=docker&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/Linux-8A222B?style=flat-square&logo=linux&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/Prometheus-751D26?style=flat-square&logo=prometheus&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/Grafana-661A22?style=flat-square&logo=grafana&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/Google%20Cloud-5F1720?style=flat-square&logo=googlecloud&logoColor=F0959C" /> <img src="https://img.shields.io/badge/Oracle%20Cloud-4F141B?style=flat-square&logoColor=F09098" />

**Tools and testing**
<br/>
<img src="https://img.shields.io/badge/Git-E63946?style=flat-square&logo=git&logoColor=2B0509" /> <img src="https://img.shields.io/badge/GitHub%20Actions-C2303C?style=flat-square&logo=githubactions&logoColor=FFE3E5" /> <img src="https://img.shields.io/badge/Pytest-9C2731?style=flat-square&logo=pytest&logoColor=FFD1D6" /> <img src="https://img.shields.io/badge/Postman-751D26?style=flat-square&logo=postman&logoColor=FFB3BA" /> <img src="https://img.shields.io/badge/JWT-5F1720?style=flat-square&logo=jsonwebtokens&logoColor=F0959C" /> <img src="https://img.shields.io/badge/Unity-4F141B?style=flat-square&logo=unity&logoColor=F09098" />

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/divider.svg" width="100%" alt="" />

## By the numbers

<div align="center">

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/stats.svg?v=2" width="100%" alt="Language distribution across 38 public repositories" />

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=madhav-gfn&bg_color=00000000&color=E63946&line=E63946&point=E63946&area=true&area_color=E63946&hide_border=true&custom_title=Contribution%20activity&radius=6" width="98%" alt="Contribution activity" />

</div>

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/divider.svg" width="100%" alt="" />

<div align="center">

<code>open to internships and freelance work on backends, AI systems, and anything that needs to run faster</code>

<br/><br/>

<a href="https://www.madhavmishra.me"><img src="https://img.shields.io/badge/madhavmishra.me-E63946?style=for-the-badge&logoColor=white" alt="Portfolio" /></a>

<br/>

<img src="https://raw.githubusercontent.com/madhav-gfn/madhav-gfn/main/assets/footer.svg" width="100%" alt="Build or be forgotten" />

</div>
