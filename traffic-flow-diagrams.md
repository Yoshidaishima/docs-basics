# Basic trafic diagrams

```mermaid
flowchart LR
  user --> web
  web -.-> user
  web --> api
  api -.-> web
  api --> database
  database -.-> api
```
