## Ashritha Gonuguntla

Carnegie Mellon University. I work on **whether AI systems actually do what we
claim they do** ,  evaluation that holds up, and the systems engineering
underneath it.

Most of my recent work follows one thread: the standard way to measure something
is often subtly invalid, and measuring it properly changes the answer.

### Publications

**[The Plan, Not the Decoder](https://arxiv.org/abs/2608.21713)** ,  ECCV 2026 (**oral**)
Reasoning-augmented text-to-image models emit a machine-readable plan before
decoding. I show compositional failures originate in the plan rather than the
decoder, and repair them at inference time by editing the plan alone.
[code](https://github.com/AshrithaG/compositional-t2i-diagnostics)

**[The Replay Gap](https://arxiv.org/abs/2608.08239)** ,  Efficient Reasoning Workshop @ COLM 2026
Every LLM-routing benchmark scores routers by replaying logged trajectories. In a
multi-step agent that is unsound. ~900 branching rollouts show early model swaps
diverge at the first post-fork action 74–77% of the time, leaving ~3% of replayed
states valid.
[code](https://github.com/AshrithaG/replay-gap) ·
[data](https://huggingface.co/datasets/ashritha0907/replay-gap-trajectories) ·
[page](https://ashrithag.github.io/replay-gap/)

### Selected work

| | |
|---|---|
| **[nanoinfer](https://github.com/AshrithaG/nanoinfer)** | Inference engine from scratch in C++: own conv kernels, liveness-based memory planner, int8 quantization. Within 1% of ONNX Runtime on dense models, and honest about the 1.3–1.7× gap on depthwise ones. |
| **[mlops-replay](https://github.com/AshrithaG/mlops-replay)** | An MLOps platform evaluated rather than merely built ,  nine years of NYC taxi data replayed monthly, with a measured detection rate and false-alarm rate for its own monitoring. |
| **[gated-residual-rl](https://github.com/AshrithaG/gated-residual-rl)** | A learned gate decides when to override a frozen base policy on contact-rich peg insertion. 85% success vs 45% base, intervening in 66% of timesteps. |
| **[gridpilot](https://github.com/AshrithaG/gridpilot)** | An LLM agent operating a simulated power grid during cascading failure: IEEE 118-bus physics, verified tools, simulate-before-apply guardrail, 50-incident benchmark. |
| **[federated-fault-diagnosis](https://github.com/AshrithaG/federated-fault-diagnosis)** | FedAvg vs FedProx on CWRU bearing data under non-IID clients, partial participation, and stragglers. |

📫 agonugun@andrew.cmu.edu
