---
title: ""
date: 2017-11-22T21:20:58+03:00
draft: false
weight: 8
---

## PlanningPoker Contract

Planning Poker is the main concept of scrum methodology. Team members estimate tasks and the finalaverage result represents the award amount. When a new task added to a project management tool trustedOracle initializes new voting:

```
struct Voting {
  string issue;
  uint votesCount;
  uint sum;
  bool isValid;
  bool isOpen;
  bool awardPaid;
  mapping (address => uint) votes;
}
```