HTML Equivelent of an UNORDERED LIST is Hyphen.

<UL>
	<LI>Cat</LI>
	<LI>Dog</LI>
	<LI>Turtle</LI>
</UL>

- Cat
- Dog
- Turtle

EXAMPLE MERMAID FLOWCHART
```mermaid
graph TD;
  START-->RUN_PROGRAM?;
  RUN_PROGRAM?-->RUN_TRUE;
  RUN_PROGRAM?-->RUN_FALSE;
  RUN_TRUE-->MAIN;
  MAIN-->READ_FILE;
  READ_FILE-->MAIN;
  MAIN-->PROCESS_INPUT;
  PROCESS_INPUT-->MAIN;
  MAIN-->RUN_PROGRAM?;
  RUN_FALSE-->END_PROGRAM;
end
```
MORE ELABORATE MERMAID FLOWCHART
```mermaid
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