# Mark Yong

I run a local LLM inference stack built around three RTX PRO 6000 Blackwell 
GPUs (96 GB each, 288 GB total) on an EPYC host under Proxmox. LiteLLM handles
routing across vLLM, SGLang, and llama.cpp, and I use the system to run larger
open-weight models such as GLM-5.3-Flash and DeepSeek V4 entirely on-prem.

Background: data science and analytics in fintech and banking. Most
recently Principal Data Scientist / Group Head of Data at Funding
Societies, leading a regional team of about 20 across Singapore,
Indonesia, Malaysia, and India. Before that, six years at UOB in finance
analytics, leaving as VP. CFA, FRM, and Berkeley MIDS along the way.

## Selected work

- inference-platform:
the configs and operational notes behind that stack, including the
routing tiers and a couple of postmortems from incidents that changed
the setup.
- dsv41-exl3-sm120-tp3-notes:
getting DeepSeek-V4.1-Flash EXL3 serving at TP3 on
those GPUs. Benchmarks, the configs that failed, and a reproducible
image build. Short version: it boots, it trails the dense alternative,
and long context does not fit.
- deep-research: a homelab
adaptation of LangChain's Open Deep Research, wired to MiniMax in the
homelab and self-hosted SearXNG.
- llm-council: my LangGraph
take on Karpathy's LLM council. Candidate labels are shuffled before
ranking and the seed is persisted, so ordering effects don't quietly
turn into irreproducible results.

## Benchmarking

Throughput numbers with configs launch flags, model. quantisation details, and benchmark
commands next to results, pin digests where practical, keeping
failed runs in the write-up.

## Elsewhere

Singapore. Open to senior/principal data science, applied AI, and AI
systems roles.

[LinkedIn](https://www.linkedin.com/in/mark-yong)
