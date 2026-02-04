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
---
title: Flow of Capital
---
flowchart LR

  i[Intel]
  a[AMD]
  n[Nvidia]
  or[Oracle]
  oa[OpenAI]
  x[XAI]
  m[Microsoft]
  c[Coreweave]


  subgraph Data Centers
    subgraph Purchase chips & Lease
      direction TB
      or
      c
    end
  end

  subgraph Chip Design
    subgraph & Manufacturing
      direction TB
      i
      a
      n
    end
  end

  subgraph Purchasers chips
    subgraph -
      direction TB
      oa
      x
    end
  end

  m --1. 58b investment--> oa
  oa --2. 58b to use data centers --> m
  m --3. 58b for chips--> n
  n --4. 58b investment--> oa

  oa --5. 300b deal--> or
  or --6. 10s of billions purchase--> n
  n --Invest ~100b provided OpenAI buys more chips--> oa
  

```
