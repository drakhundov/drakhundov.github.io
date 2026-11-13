---
layout: default
---

# Abdul Akhundzada

Welcome. Most of the work here grows out of a fondness for mathematics, and it deliberately spans several disciplines: benchmarking large language models, retrieval systems, machine learning from first principles, algorithms and data structures, operating-system internals in C, real-time scheduling, and processor design in Verilog.

I'm based in Istanbul, Türkiye, completing my degree in Computer Engineering at **Istanbul Technical University**, and previously interned at **Baykar** as an AI engineer. I'm glad to discuss any of this work in English, Turkish or Russian.

<p class="muted">interests: mathematics, philosophy, history, music (classical guitar), writing, literature, linguistics</p>

## work

### machine learning & llms

- [qwen3.5-quant-bench](https://github.com/drakhundov/qwen3.5-quant-bench): fp16 vs AWQ quantization of Qwen3.5-2B on MME-RealWorld, served with vLLM, measured on latency, memory and accuracy together
- [rag-api](https://github.com/drakhundov/rag-api): retrieval-augmented generation over PDFs, with OCR, query translation, heuristic routing and reciprocal rank fusion
- [ml-suite](https://github.com/drakhundov/ml-suite): regression, logistic regression, KNN, k-means and naive Bayes from scratch in NumPy
- [llm-tooling](https://github.com/drakhundov/llm-tooling): a minimal ReAct-style agent whose tools are declared as typed Python functions

### systems & hardware

- [basic-cpu](https://github.com/drakhundov/basic-cpu): a 16-bit CPU in Verilog, from ALU and register files to a 12-state control unit
- [rtss](https://github.com/drakhundov/rtss): real-time scheduling emulator in C++: cyclic executive, RM, DM, EDF, LLF
- [minifs](https://github.com/drakhundov/minifs): an inode-based file system in C
- [unix](https://github.com/drakhundov/unix): classic Unix utilities rewritten in C
- [signal-translator](https://github.com/drakhundov/signal-translator): line coding and modulation schemes, digital and analog

### algorithms & data structures

- [algo-analysis](https://github.com/drakhundov/algo-analysis): sorting and selection algorithms in C++, benchmarked
- [Red-Black-Tree](https://github.com/drakhundov/Red-Black-Tree): red-black tree with iterative and recursive variants, property-tested
- [Binary-Search-Tree](https://github.com/drakhundov/Binary-Search-Tree), [Heap](https://github.com/drakhundov/Heap): the structures underneath
- [freebase-search](https://github.com/drakhundov/freebase-search): shortest paths across the Freebase knowledge graph, in Haskell

## background

- **Baykar**: AI Engineer Intern, summer 2026
- **İTÜ Teknopark**: Project Scholar in agentic AI and RPA, 2025 to present.
- **T3 Vakfı**: AI Engineer Intern, summer 2025. LLM agents with RAG pipelines that automate high-volume customer support, using semantic chunking and vector retrieval.
- **İTÜ TAYF**: Software Engineer, 2024. A C++ ground-station server collecting real-time telemetry from a model satellite, with a Qt interface for live data.
- **Istanbul Technical University**: B.Sc. Computer Engineering (English), expected June 2027

{% if site.notes.size > 0 %}
## notes

{% assign notes = site.notes | sort: "date" | reverse -%}
{% for note in notes limit: 5 -%}
- <span class="muted">{{ note.date | date: site.theme_config.date_format }}</span> [{{ note.title | downcase }}]({{ note.url | relative_url }})
{% endfor -%}
{% if site.notes.size > 5 %}- [all notes >](/notes/){% endif %}
{% endif %}

## links

- [github](https://github.com/drakhundov)
- [linkedin](https://www.linkedin.com/in/abdul-akhundzadeh)
- [email](mailto:abdul.akhundzada@outlook.com)
- [cv (pdf)](/cv.pdf)
