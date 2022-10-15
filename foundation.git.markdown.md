#GitLab Markdown Notes

---

##Task Lists

1. [X] Unordered List
1. [~] Add Extra Features free of charge to customer.
1. [ ] Graphing
   1. [x] Simple Mermaid Chart
   1. [ ] Advanced Mermaid Chart
   1. [~] Usable Enterprise Relational Diagrams

---

##HTML Equivelent of an UNORDERED `<UL><LI></LI></UL>` is <kbd>-</kbd> or <kbd>*</kbd> or <kbd>+</kbd>

<UL>
	<LI>Cat</LI>
	<LI>Dog</LI>
	<LI>Turtle</LI>
</UL>

- <kbd>-</kbd>Cat
+ <kbd>+</kbd>Dog
* <kbd>*</kbd>Turtle
---
SIMPLE MERMAID FLOWCHART
```mermaid
graph TD;
  START-->MAIN_LOOP_EVALUATION;
  MAIN_LOOP_EVALUATION-->CONTINUE_THE_LOOP;
  MAIN_LOOP_EVALUATION-->END_THE_LOOP; 
  END_THE_LOOP-->STOP;
  CONTINUE_THE_LOOP-->MAIN;
  MAIN-->RUN_PROCESSES;
  MAIN-->MAIN_LOOP_EVALUATION;
```
##ADVANCED MERMAID FLOWCHART
```mermaid
graph TB

  SubGraph1 --> SubGraph1Flow
  subgraph "Maintenance Tasks"
  SubGraph1Flow(SubNode 1)
  SubGraph1Flow -- Choice1 --> DoChoice1
  SubGraph1Flow -- Choice2 --> DoChoice2
  end

  subgraph "Main Graph"
  START[START PROGRAM] --> HSKP[M]
  MAINTENANCE--> HSKP[run]
  SubGraph1 --> END_PRGROGRAM[STOP PROGRAM]
end
```

```mermaid
graph TB

  SubGraph1 --> SubGraph1Flow
  subgraph "SubGraph 1 Flow"
  SubGraph1Flow(SubNode 1)
  SubGraph1Flow -- Choice1 --> DoChoice1
  SubGraph1Flow -- Choice2 --> DoChoice2
  end

  subgraph "Main Graph"
  Node1[Node 1] --> Node2[Node 2]
  Node2 --> SubGraph1[Jump to SubGraph1]
  SubGraph1 --> FinalThing[Final Thing]
end
```
---
Tables
|col1|col2|col3|
|a|b|c|
|1||3|
---