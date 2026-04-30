# design-skills

A collection of Claude Code skills for the design team — an experiment in helping designers iterate directly in code while keeping a design-focused approach, so we can still produce unique, polished work without leaving the craft behind.

The idea: rather than handing designs off to engineering and losing fidelity in translation, designers can explore, branch, and refine ideas in code using these skills as scaffolding for the parts that aren't worth re-deriving every time (visual language, iteration patterns, polish conventions).

## Skills

- **`pai-visual-language`** — stylistic conventions and brand voice for presentations.ai UI work (color emphasis, copy voice, density, hierarchy patterns). Use alongside the design system, not as a replacement.
- **`crazy8s`** — branching visual-iteration workflow that produces 8 variations in one rolling file, waits for a pick, then branches 8 more from that pick. For exploring alternatives quickly without committing early.

## Using these skills

Each skill lives in `skills/<name>/SKILL.md`. To use one with Claude Code, symlink or copy it into your `~/.claude/skills/` directory:

```sh
ln -s "$(pwd)/skills/pai-visual-language" ~/.claude/skills/pai-visual-language
ln -s "$(pwd)/skills/crazy8s" ~/.claude/skills/crazy8s
```

Then invoke them in Claude Code with `/pai-visual-language` or `/crazy8s`, or let Claude pick them up automatically when the task matches.
