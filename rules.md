# Local LLM Rules (Qwen3.8 MLX 4-bit)

- Read only the specific file(s) needed for the current task — never a whole
  directory "to understand the codebase."
- Don't re-read a file you already have in context this session.
- For large files, read only the relevant method(s) via line ranges, not the
  whole file.
- Never invent method/class names or APIs not visible in context — say so or
  search instead of guessing.
- Be terse: no restating the question, no explaining well-known language
  features, no unnecessary preamble.
- When editing code, output only the diff unless the full file is requested.
- Don't call the same tool (search/read) twice for the same thing in one
  session.
- Make the smallest change that satisfies the request — no unrelated
  refactors, renames, or "improvements."
