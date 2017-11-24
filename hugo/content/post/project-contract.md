---
title: ""
date: 2017-11-22T21:19:12+03:00
draft: false
weight: 7
---

## Project Contract

The main contract implements ERC20 interface. New Tokens generate only when some work has been done and represent the contribution of each participant.

Project Owner deploys contracts, link all of them to Project contract and add Workers

```
struct Worker {
  address _address;
  string username;   //JIRA username
}
```

Owner also initializes trustedOracle account, which can call payAward function. This is done for security purposes because oracle private key stored on the server and can be compromised but with this separations, it's not critical.