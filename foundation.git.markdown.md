HTML Equivelent of an UNORDERED LIST is Hyphen.

<UL>
	<LI>Cat</LI>
	<LI>Dog</LI>
	<LI>Turtle</LI>
</UL>

- Cat
- Dog
- Turtle

Graph Test
```mermaid
graph TD;
  START-->RUN_PROGRAM?;
  RUN_PROGRAM?-->RUN_TRUE;
  RUN_PROGRAM?-->RUN_FALSE;
  RUN_TRUE-->MAIN;
  MAIN-->READ_FILE;
  READ_FILE-->MAIN;
  MAIN-->PROCESS_INPUT;
  MAIN-->RUN_PROGRAM?;
  RUN_FALSE-->END_PROGRAM;