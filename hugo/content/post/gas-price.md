---
title: ""
date: 2017-11-29T14:17:43+03:00
draft: false
weight: 5
---

# Gas price
-------------

&nbsp;
## Deploy Contract price

| Method           | Gas           |
| -------------    | ------------- |
| `crowdsale`      | 1716665       |
| `migrations`     | 269607        |
| `planningPoker`  | 1613396       |
| `productBacklog` | 1398455       |
| `project`        | 3001382       |
| **Total amount** | ~8*10^6       |

&nbsp;
## Project Contract price

| Method                    | Info                        | Gas           |
| -------------             | -------------               | ------------- |
| `addTrustedOracle`        |                             | 43437         |
| `addWorker`               | Add first worker            | 106889        |
| `addWorker`               | Add not first worker        | 91889         |
| `initCrowdsale`           | First call                  | 63814         |
| `initCrowdsale`           | Not first call              | 33814         |
| `initPlanningPoker`       |                             | 43965         |
| `payAward`                |                             | 80881         |
| `transfer` && `addHolder` | Add first holder            | 93010         |
| `transfer` && `addHolder` | Add not first holder        | 78010         |
| `transfer`                | Recipient is a holder       | 37031         |

&nbsp;
## PlanningPoker Contract price

| Method                    | Gas           |
| -------------             | ------------- |
| `addVoting`               | 84651         |
| `closeVoting`             | 28568         |
| `vote` && `addVoting`     | 92645         |
| `vote`                    | 42808         |

&nbsp;
## ProductBacklog Contract price

| Method                    | Gas           |
| -------------             | ------------- |
| `addVoting`               | 54286         |
| `closeVoting`             | 28502         |
| `vote` && `addVoting`     | 151383        |
| `vote`                    | 94758         |

&nbsp;
## Crowdsale Contract price

| Method                    | Info                        | Gas           |
| -------------             | -------------               | ------------- |
| `addBuyOrder`             |                             | 129224        |
| `addSellOrder`            | First sell order            | 161318        |
| `addSellOrder`            | Not first sell order        | 146318        |
| `buy`                     |                             | 37106         |
| `closeBuyOrder`           |                             | 21512         |
| `closeSellOrder`          | First closed sell order     | 28699         |
| `closeSellOrder`          | Not first closed sell order | 21850         |
| `sell`                    |                             | 57381         |