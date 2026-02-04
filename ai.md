# Flow of capital
### Overview
``` mermaid
info
```
``` mermaid
flowchart LR
  
  a["`Intel
  AMD
  Nvidea`"]
  b["`OpenAI
  XAI
  Microsoft`"]
  c["`Oracle
  Coreweave`"]

  a <--> b
  b <--> c
  c <--> a

```
``` mermaid
flowchart LR

  i[Intel]
  a[AMD]
  n[Nvidea]
  or[Oracle]
  oa[OpenAI]
  x[XAI]
  m[Microsoft]
  c[Coreweave]


  subgraph Data Centers : Purchase chips & lease compute
    direction TB
    or
    c
  end

  subgraph Chip Design & Manufacturing
    direction TB
    i
    a
    n
  end

  subgraph Purchasers chips
    direction TB
    oa
    x
  end

  m --1. 58b investment--> oa
  oa --2. 58b to use data centers --> m
  m --3. 58b for chips--> n
  n --4. 58b invest--> oa

  oa --5. 300b deal--> or
  or --6. 10s of billions purchase--> n
  n --Invest ~100b provided OpenAi buys more chips--> op
  

```
