# Powerful Prompts

![Powerful Prompts banner](assets/github-prompting.jpg)

Battle-tested prompts for sharper AI reasoning, writing, estimation, and adaptive systems—ready to copy, adjust.

## Directory Structure

```
prompts/
├── reasoning/              # Structured reasoning and problem-solving
├── estimation/             # Mathematical and Fermi estimation
├── writing/                # Content creation and review
├── advanced-techniques/    # Complex multi-strategy prompts
└── meta-utility/          # Prompt improvement and adaptive systems
```

## Prompt Map

**Reasoning (`prompts/reasoning/`)**
- `cot_prompt.txt`, `reflection_prompt.txt`, `deepdive.txt`, `sophisticated_verbal_problem_solving.txt`

**Estimation (`prompts/estimation/`)**
- `fermi.txt`

**Writing (`prompts/writing/`)**
- `summarisation.txt`, `factual-consistency-summarisation.txt`, `editorial_review_prompt.txt`, `generate_expert_qna_prompt.txt`, `generate-verbal-feedback-in-pairwise-ranking.txt`

**Advanced Techniques (`prompts/advanced-techniques/`)**
- `graph-of-thought-prompting.txt`, `synthetic_reasoning_prompt.txt`, `mystery_solver.txt`, `abstract-prompt.txt`, `atomic_elements_prompt.txt`, `prompt_chain_of_symbols.txt`

**Meta & Utility (`prompts/meta-utility/`)**
- `adaptive_dynamic_AI_assistant.txt`, `prompt_improver_context_meta_codes.md`

## Quick Start

### Basic Usage

1. Pick a prompt from the map above.
2. Copy the file content.
3. Swap placeholder variables (usually `{{DOUBLE_BRACES}}`).
4. Paste into your AI interface or code.

### Example: Using Chain of Thought

```python
# For programmatic use
cot_prompt = """
You are an AI assistant that uses a Chain of Thought (CoT) approach with reflection...
[Full prompt content]
"""

response = model.generate(cot_prompt + "\n\nQuery: " + user_question)
```

### Example: Fermi Estimation

```
Replace {{FERMI_QUESTION}} with your estimation problem, e.g.
"How many piano tuners are there in Leeds?"
```

## Best Practices

### Choosing the Right Prompt

1. Logical reasoning: `cot_prompt.txt` or `reflection_prompt.txt`
2. Calculations: `fermi.txt` or `deepdive.txt`
3. Writing: any file in `prompts/writing/`
4. Complex multi-faceted problems: `abstract-prompt.txt` or `graph-of-thought-prompting.txt`
5. Adaptive behaviour: `adaptive_dynamic_AI_assistant.txt`

### Optimisation Tips

- Combine prompts (e.g., CoT + Reflection)
- Adjust detail level to match complexity
- Iterate with reflection to refine outputs
- Customise placeholders to your domain

## Advanced Usage

### Chaining Prompts

```
1. Break the task with `atomic_elements_prompt.txt`
2. Solve each element with `cot_prompt.txt`
3. Validate with `reflection_prompt.txt`
```

### Prompting Techniques to Try (beyond those in the files)

- Self-consistency sampling: draft several reasoning paths and keep the consensus answer.
- Deliberate planning: outline steps before generating the solution.
- Socratic questioning: ask clarifying questions before answering.
- Few-shot scaffolding: show a mini example for each subtask, not just the final output.
- Program-Aided Logic (PAL): write executable pseudo-code and then explain the result.
- Retrieval-augmented prompting: fetch context (or craft hypotheticals like HyDE) before reasoning.
- Constraint-first prompting: declare hard limits, non-goals, and style rules upfront.
- Persona stacking: rotate through expert roles to stress-test answers.
- Counterfactual stress tests: ask “what would make this fail?” then patch the answer.
- Style transfer prompting: match tone/voice from a short reference excerpt.

## Use Cases

### Research & Analysis
- Literature review synthesis
- Complex problem decomposition
- Multi-factor decision analysis

### Education
- Worked example generation
- Step-by-step problem solving
- Conceptual understanding assessment

### Content Creation
- Technical writing
- Article editing and review
- Summary generation

### Software Development
- Debugging complex issues
- System design analysis
- Code review and optimisation

## Contributing

Contributions are welcome! When adding new prompts:

1. Place new prompts in the right category folder.
2. Use descriptive filenames (lowercase with underscores or hyphens).
3. Explain placeholder variables.
4. Add examples where helpful.
5. Update this README with a short note.

## File Naming Conventions

- Use lowercase with underscores or hyphens.
- Be descriptive: `chain_of_thought.txt` not `cot.txt`.
- Indicate technique: `*_prompt.txt`, `*_framework.txt`.
- Match content to the filename.

## License

MIT License - See [LICENSE](LICENSE) for details

## Citation

If you use these prompts in your research or projects, please cite:

```bibtex
@misc{powerful-prompts-2024,
  author = {Roberts, Gareth},
  title = {Powerful Prompts: A Collection of Advanced AI Prompting Techniques},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/dr-gareth-roberts/Powerful-Prompts}
}
```

## Additional Resources

- [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [Chain-of-Thought Paper](https://arxiv.org/abs/2201.11903)
- [Tree-of-Thought Paper](https://arxiv.org/abs/2305.10601)
- [Graph-of-Thought Paper](https://arxiv.org/abs/2308.09687)

## Support

For questions, issues, or suggestions:
- Open an issue on GitHub
- Contribute improvements via pull requests

---

**Last Updated:** February 2026
