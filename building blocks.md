```mermaid
  flowchart TD
  subgraph pt["protocals"]
  TCP["tcp/ip"] --> HT["http"] & HTS["htttps"]
  FTP
  UDP
  end
  
  subgraph API["api"]
  P1["path/resources/id"]
  P2["path/resources/id/resources/id"]
  
  subgraph rs[ ]
  RS["response"] --> JSON & HTML["html"]
  end
  end 
  
  subgraph DB["databases"]
  KS["key-value stores"] -.->Radis
  GS["graph stores"] -.-> Graph_DB
  CS["column stores"] 
  DS["document stores"] -.-> MD["Mongo DB"] & DY["Dynamo DB"]
  end
  
```
