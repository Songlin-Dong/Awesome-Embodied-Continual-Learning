# Contributing to Awesome Embodied Continual Learning

Thank you for your interest in contributing! This list is maintained by [Songlin Dong](https://songlin-dong.github.io) and welcomes contributions from the community.

## How to Add a Paper

### Format

Use the following format consistently:

```
Paper Title (VenueYear) [[paper](url)] [[code](url)]
```

Examples:
```
Continual Learning for Robot Manipulation via Experience Replay (ICRA2024) [[paper](https://arxiv.org/...)] [[code](https://github.com/...)]
Lifelong Navigation in Dynamic Environments (CoRL2023) [[paper](https://arxiv.org/...)]
```

- **Venue abbreviations**: Use standard short forms — CVPR, ICCV, ECCV, NeurIPS, ICML, ICLR, AAAI, CoRL, ICRA, IROS, RSS, RAL, T-RO, IJRR, etc.
- **Year**: Append 4-digit year directly to venue with no space, e.g. `CVPR2024`
- **Links**: `[paper]` is required; `[code]` is optional but encouraged
- **arXiv**: Use `(arXiv2024)` for preprints not yet published at a venue

### Steps

1. **Fork** this repository
2. **Add** your paper in the appropriate section(s):
   - Add under the correct **task category** (Manipulation, Navigation, etc.)
   - Add under the correct **approach category** (Replay, Regularization, etc.)
   - Add under the correct **year** section
3. Keep entries sorted **newest first** within each year
4. **Open a pull request** with:
   - Title: `Add [Paper Short Title] (VenueYear)`
   - Brief note on which task/approach categories it belongs to

## What Qualifies

A paper qualifies for this list if it:

- Studies an **embodied agent** (robot, avatar, or simulated agent) in a physical or simulated world
- Addresses **continual, lifelong, or incremental learning** (sequential task learning, avoiding catastrophic forgetting, forward/backward transfer, etc.)
- Is published at a **peer-reviewed venue** or is a well-cited arXiv preprint

Papers that are *only* general continual learning (no embodied setting) belong in other lists such as [Awesome Incremental Learning](https://github.com/xialeiliu/Awesome-Incremental-Learning).

## Reporting Issues

If you notice a broken link, a missing paper, or an incorrect categorization, please open an **Issue** with a brief description.

---

Thank you for helping make this list more comprehensive! 🤖
