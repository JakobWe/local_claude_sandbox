# Context discipline
- Never read an entire directory of files "to understand the codebase" — read only 
  the specific file(s) needed for the current task.
- Before reading a Java class, check if you already have its contents in context 
  from earlier in this session. Don't re-read unless the file may have changed.
- When you need to know a class's public API (not its implementation), search for 
  just the method/field signatures and class-level Javadoc rather than reading the 
  full file — grep for `public `, `protected `, `class `, `interface `.
- Don't open test files, generated code, or build directories (target/, build/, 
  *.class) unless directly asked.
- For large classes (>300 lines), read only the relevant method(s) plus imports 
  and class declaration — use line ranges, not whole-file reads.
- If a task touches many classes, work through them one at a time and summarize 
  findings before moving to the next, rather than loading them all upfront.
- Prefer grep/search over reading full files when locating where something is 
  defined or used.
