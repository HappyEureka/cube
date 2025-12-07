# CUBE

**Collaborative Multi-Agent Block-Pushing Environment for Collective Planning with LLM Agents**

> **Heads up!** CUBE is currently undergoing cleanup to make the codebase more polished and developer-friendly. The environment is functional, but some components are still being streamlined. Feel free to explore and experiment, keeping in mind that things are still evolving.

## Overview

**CUBE** is a lightweight, scalable, and interpretable environment for studying **cooperative intelligence** in LLM agents, RL agents, and hybrid neurosymbolic systems at scale.

Existing multi-agent benchmarks often involve only a few agents or require many agents without meaningful cognitive demands. CUBE fills this gap by introducing tasks where **difficulty grows with the number of agents**, requiring individual reasoning ability and genuine multi-agent cooperation.

Agents operate in a 2D grid world and must **push weighted blocks** into a goal region while coordinating under embodied constraints such as:

- congestion
- collisions
- force requirements
- block-chain
- agent-chain
- dynamic environmental uncertainty

CUBE uses a **dual-layer design** that exposes and tests cooperative cognition:

- A **primitive layer** governing grid actions and physical dynamics
- A **symbolic layer** offering higher-level actions such as `move_to_block`, `rendezvous`, `push_block`, and `wait_agents`, making it natural for LLM-based planning and communication

A single parameter **n** controls grid size, team size, block distribution, and overall complexity, creating a transparent and reproducible **difficulty curriculum** for studying cooperation from small teams to hundreds of agents.

CUBE is also the environment used by **DR. WELL**, a decentralized neurosymbolic framework that tackles cooperation through joint negotiation, individual planning, and a shared world model for iterative improvement.

**[CUBE: Collaborative Multi-Agent Block-Pushing Environment for Collective Planning with LLM Agents](https://happyeureka.github.io/cube/)**

https://happyeureka.github.io/cube/

**[DR. WELL: Dynamic Reasoning and Learning with Symbolic World Model for Embodied LLM-Based Multi-Agent Collaboration](https://narjesno.github.io/DR.WELL/)**

https://narjesno.github.io/DR.WELL/

## Key Features

- **Cooperative intelligence at scale with hundreds of LLM agents**
- **Symbolic and primitive action layers supporting neurosymbolic reasoning**
- **Difficulty curriculum controlled by a single parameter**
- **Rich symbolic feedback for customizable supervision and analysis**

## Citation

If you use CUBE in your research, please cite:

```bibtex
@inproceedings{yangcube,
  title     = {CUBE: Collaborative Multi-Agent Block-Pushing Environment for Collective Planning with LLM Agents},
  author    = {Yang, Hanqing and Nourzad, Narjes and Chen, Shiyu and Joe-Wong, Carlee},
  booktitle = {Workshop on Scaling Environments for Agents},
  year      = {2025}
}
```

If you are exploring embodied LLM-based cooperation, you may also find DR. WELL relevant:

```bibtex
@inproceedings{nourzad2025drwell,
  title     = {DR. WELL: Dynamic Reasoning and Learning with Symbolic World Model for Embodied LLM-Based Multi-Agent Collaboration},
  author    = {Nourzad, Narjes and Yang, Hanqing and Chen, Shiyu and Joe-Wong, Carlee},
  booktitle = {Workshop on Bridging Language, Agent, and World Models for Reasoning and Planning},
  year      = {2025}
}
```
