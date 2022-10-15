HTML Equivelent of an UNORDERED LIST is Hyphen.

<UL>
	<LI>Cat</LI>
	<LI>Dog</LI>
	<LI>Turtle</LI>
</UL>

- Cat
- Dog
- Turtle

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
ADVANCED MERMAID FLOWCHART
```mermaid
graph TB

  SubGraph1 --> SubGraph1Flow
  subgraph "SubGraph 1 Flow"
  SubGraph1Flow(SubNode 1)
  SubGraph1Flow -- Choice1 --> DoChoice1
  SubGraph1Flow -- Choice2 --> DoChoice2
  end

  subgraph "Main Graph"
  START[START PROGRAM] --> MAINTENANCE[Check Maintenance Items]
  Node2 --> SubGraph1[Jump to SubGraph1]
  SubGraph1 --> END_PRGROGRAM[STOP PROGRAM]
end
```