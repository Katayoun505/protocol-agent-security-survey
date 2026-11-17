# Security Evaluation of Protocol-Connected Agentic AI Systems

Companion repository for the survey **"Security Evaluation of Protocol-Connected Agentic AI Systems: A Survey of Threats, Benchmarks, Metrics, and Open Challenges"** (Rafat and Fachkha, 2026, under review).

The survey systematically reviews security benchmarks and evaluation studies for LLM-based agents that use standard protocols: the **Model Context Protocol (MCP)** for agent–tool interaction, and **A2A, ANP, ACP, AP2 and Coral** for agent–agent interaction. This repository holds the structured data behind the paper so that others can reuse, check and extend it.

## Contents

| File | What it contains |
|---|---|
| `benchmark_inventory.csv` | The 18 included benchmarks and evaluation studies plus 5 baselines: protocol, multi-agent support, environment, models, threats, scale, metrics, success-verification level, defenses, code availability, venue |
| `screening_log.csv` | All 222 screened records with the inclusion decision and the reason for exclusion |
| `search_log.csv` | Every Google Scholar query and "Cited by" list used, with the number of results and pages screened |
| `trust_boundaries.csv` | The seven trust boundaries (B1–B7) of a protocol-connected agent system |
| `taxonomy.csv` | Taxonomy of protocol-level attacks by layer, workflow stage and trust boundary, mapped to the benchmarks that evaluate them |
| `metrics_framework.csv` | Security metric families and how often the corpus measures each |
| `benchmark_comparison.tex` | The comparison table from the paper, ready to include in LaTeX |

## Scope and method in brief

- **Time window:** January 2023 to October 2026 (state on 17 November 2026).
- **Search:** Google Scholar keyword queries, plus backward and forward snowballing ("Cited by" lists of MCPTox, MSB, MCP-SafetyBench and A2ASecBench).
- **Inclusion:** (I1) the work proposes a benchmark, testbed or evaluation framework, or is an evaluation study; (I2) it evaluates the security of LLM agents or their protocol infrastructure, with at least one LLM agent, host or client evaluated; (I3) the system communicates through a standardised agent protocol.
- **Result:** 222 records screened, 18 included, 5 tool-use baselines without a protocol layer, 199 excluded.
- Every number in the inventory was checked against the final published version of each paper (or the latest arXiv version for preprints).

## Column notes for `benchmark_inventory.csv`

- **environment:** R = at least one real, publicly released protocol implementation, server, host, client or harness is part of the evaluated system; E = all protocol components built or emulated by the authors; S = tools simulated without a protocol implementation.
- **success_verified_at:** Call = the agent issues the malicious call; Effect = a side effect actually occurs; Cons. = downstream consequence for the task; n/s = not stated.
- **code_released:** yes / no / restricted (available on request).

## Contributing

The field moves quickly. If you know of a benchmark we missed, or a number that changed in a newer version of a paper, please open an issue or a pull request with the paper link. New entries are screened with the same criteria (I1–I3).

## Citation

```bibtex
@misc{rafat2026protocolsecurity,
  title  = {Security Evaluation of Protocol-Connected Agentic AI Systems: A Survey of Threats, Benchmarks, Metrics, and Open Challenges},
  author = {Rafat, Katayoun and Fachkha, Claude},
  year   = {2026},
  note   = {Under review}
}
```

## License

The data in this repository is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0). Paper titles and metadata belong to their respective authors.
