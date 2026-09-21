# Mark Yong

I run my own LLM inference stack: three RTX PRO 6000 Blackwell GPUs
(96 GB each, 288 GB total) on an EPYC host under Proxmox, with LiteLLM
routing between vLLM, SGLang, and llama.cpp services. About 15
containers, four open-weight model families, and no third-party LLM API
anywhere in the serving path.

Background: data science and analytics in fintech and banking. Most
recently Principal Data Scientist / Group Head of Data at Funding
Societies, leading a regional team of about 20 across Singapore,
Indonesia, Malaysia, and India. Before that, six years at UOB in finance
analytics, leaving as VP. CFA, FRM, and Berkeley MIDS along the way.

## Selected work

- [inference-platform](https://github.com/mark-yong/inference-platform):
  the configs and operational notes behind that stack, including the
  routing tiers and a couple of postmortems from incidents that changed
  the setup.
- [dsv41-exl3-sm120-tp3-notes](https://github.com/mark-yong/dsv41-exl3-sm120-tp3-notes):
  getting DeepSeek-V4.1-Flash EXL3 serving at tensor parallelism 3 on
  those GPUs. Benchmarks, the configs that failed, and a reproducible
  image build. Short version: it boots, it trails the dense alternative,
  and long context does not fit. I wrote up why.
- [deep-research](https://github.com/mark-yong/deep-research): a homelab
  adaptation of LangChain's Open Deep Research, wired to MiniMax in the
  homelab and self-hosted SearXNG.
- [llm-council](https://github.com/mark-yong/llm-council): my LangGraph
  take on Karpathy's LLM council. I shuffle the candidate labels before
  ranking and exclude self-votes from the aggregate, both to cut bias,
  and the shuffle seed is persisted so runs stay debuggable.

## Benchmarking

Throughput numbers without their configuration aren't worth much. I
publish launch flags, model and quantisation details, and benchmark
commands next to results, pin digests where practical, and keep the
failed runs in the write-up.

## Elsewhere

Singapore. Open to senior/principal data science, applied AI, and AI
systems roles.

[LinkedIn](https://www.linkedin.com/in/mark-yong)
