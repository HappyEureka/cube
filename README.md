# CUBE

**Collaborative Multi-Agent Block-Pushing Environment for Collective Planning with LLM Agents**

> **Heads up!** CUBE is currently undergoing cleanup to make the codebase more polished and developer-friendly. The environment is fully functional, but some components are still being streamlined. Feel free to explore and experiment—just keep in mind that things are still evolving.

## Overview

**CUBE** is a lightweight, scalable, and interpretable environment for studying **embodied cooperation** among LLM agents, RL agents, and hybrid neurosymbolic systems.

Agents operate in a 2D grid world and must **push weighted blocks** into a goal region while dealing with:

- congestion  
- collisions  
- force requirements  
- block-chain
- agent-chain
- environment dynamics (changing conditions)

CUBE uses a **dual-layer design**:

- A **primitive layer** that handles grid actions and physical dynamics  
- A **symbolic layer** that provides high-level actions such as `move_to_block`, `rendezvous`, `push_block`, and `wait_agents`, making it natural for LLM planning

A single parameter **n** determines grid size, team size, and block distribution, producing a transparent and reproducible **difficulty curriculum** from small to large team cooperation.

**Paper:**  
[*CUBE: Collaborative Multi-Agent Block-Pushing Environment for Collective Planning with LLM Agents*](https://happyeureka.github.io/cube/) 

CUBE is also the environment used by [*DR. WELL*](https://narjesno.github.io/DR.WELL/), a decentralized neurosymbolic method for embodied multi-agent reasoning.



## Key Features

- **Embodied multi-agent cooperation at scale**
- **Symbolic + primitive action layers**
- **Curriculum controlled by a single parameter**
- **Rich symbolic feedback concepts for customized feedback**

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
