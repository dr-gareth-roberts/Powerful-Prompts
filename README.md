# Powerful Prompts

A curated collection of advanced prompting techniques for AI language models. This repository contains battle-tested prompts for reasoning, problem-solving, content creation, and more.

## Overview

These prompts leverage cutting-edge prompting techniques including Chain-of-Thought (CoT), Tree-of-Thought, Graph-of-Thought, meta-prompting, and synthetic reasoning to enhance AI model performance across diverse tasks.

## Directory Structure

```
prompts/
├── reasoning/              # Structured reasoning and problem-solving
├── estimation/             # Mathematical and Fermi estimation
├── writing/                # Content creation and review
├── advanced-techniques/    # Complex multi-strategy prompts
└── meta-utility/          # Prompt improvement and adaptive systems
```

## Prompt Categories

### 🧠 Reasoning & Problem Solving
**Location:** `prompts/reasoning/`

Advanced prompts for structured thinking and complex problem-solving.

- **`cot_prompt.txt`** - Chain of Thought with Reflection
  - Implements step-by-step reasoning with built-in error checking
  - Separates thinking process from final output
  - Best for: Complex queries requiring careful analysis

- **`reflection_prompt.txt`** - Multi-stage Reflection Framework
  - Structured approach with thinking, reflection, and output phases
  - Validates reasoning at each step
  - Best for: High-stakes decisions requiring verification

- **`deepdive.txt`** - Deep Dive Problem Analysis
  - 3-phase approach: analysis, systematic solving, rigorous validation
  - Includes constraint identification and dimensional analysis
  - Best for: Mathematical word problems and constraint-based challenges

- **`sophisticated_verbal_problem_solving.txt`** - Advanced Problem Solver
  - Combines multiple prompting strategies (meta-prompting, ReAct, Tree-of-Thought)
  - Dynamic approach selection based on problem type
  - Best for: Open-ended complex problems requiring creative solutions

### 📊 Estimation & Mathematical Reasoning
**Location:** `prompts/estimation/`

Specialized prompts for quantitative reasoning and approximation.

- **`fermi.txt`** - Comprehensive Fermi Estimation Framework
  - 15-step process for back-of-the-envelope calculations
  - Includes multiple validation loops and assumption checking
  - Contains worked examples from simple to highly complex
  - Best for: Order-of-magnitude estimations and "guesstimate" problems

### ✍️ Writing & Content Creation
**Location:** `prompts/writing/`

Prompts for high-quality content generation and evaluation.

- **`summarisation.txt`** - Expert 10-Stage Summarization
  - Comprehensive process from analysis to meta-reflection
  - Outputs summary with confidence assessment
  - Best for: Professional-grade text summarization

- **`factual-consistency-summarisation.txt`** - Factual Consistency Checker
  - Validates summary accuracy against source material
  - Best for: Ensuring summarization fidelity

- **`editorial_review_prompt.txt`** - Publication-Quality Review
  - Comprehensive style guide evaluation
  - Covers tone, grammar, citations, and inclusive language
  - Best for: Professional article and content review

- **`generate_expert_qna_prompt.txt`** - Expert Q&A Generation
  - Creates high-quality question-answer pairs
  - Best for: Training data generation and knowledge assessment

- **`generate-verbal-feedback-in-pairwise-ranking.txt`** - Response Comparison
  - Detailed comparative analysis of two responses
  - Focuses on ranking and evaluation criteria
  - Best for: Model evaluation and preference learning

### 🚀 Advanced Techniques
**Location:** `prompts/advanced-techniques/`

Cutting-edge multi-strategy prompting approaches.

- **`graph-of-thought-prompting.txt`** - Graph-based Analysis
  - 16-step process creating concept graphs with nodes and edges
  - Identifies clusters, feedback loops, and emergent patterns
  - Best for: Complex systems analysis and relationship mapping

- **`synthetic_reasoning_prompt.txt`** - Synthetic Prompting
  - Backward and forward reasoning chain generation
  - Creates related examples to build understanding
  - Best for: Learning from examples and analogical reasoning

- **`mystery_solver.txt`** - Detective Investigation Framework
  - Modular component-based investigation system
  - Implements Plan-to-Execute and iterative refinement
  - Best for: Complex multi-step investigations and debugging

- **`abstract-prompt.txt`** - Multi-Faceted Problem Solving
  - Integrates context, analogies, and counterfactuals
  - Combines ReAct and Tree-of-Thought frameworks
  - Best for: Comprehensive analysis requiring multiple perspectives

- **`atomic_elements_prompt.txt`** - Atomic Action Decomposition
  - Graph-of-Thought backward + recursive Chain-of-Thought forward
  - Breaks complex goals into atomic actionable steps
  - Best for: Project planning and task breakdown

- **`prompt_chain_of_symbols.txt`** - Symbolic Reasoning
  - Uses compact symbolic notation for spatial reasoning
  - Reduces cognitive load through abstraction
  - Best for: Geometry, spatial relationships, and logic puzzles

### 🛠️ Meta & Utility
**Location:** `prompts/meta-utility/`

Tools for prompt optimization and adaptive behavior.

- **`adaptive_dynamic_AI_assistant.txt`** - Adaptive Assistant Framework
  - Dynamically adopts expert personas
  - Decomposes tasks and generates context on-the-fly
  - Best for: Versatile general-purpose assistance

- **`prompt_improver_context_meta_codes.md`** - Meta-code System
  - Structured task and formatting specification language
  - Enables concise, precise prompt communication
  - Best for: Standardizing prompt instructions and workflows

## Quick Start

### Basic Usage

1. Choose a prompt from the appropriate category
2. Copy the prompt content
3. Replace any placeholder variables (typically in `{{DOUBLE_BRACES}}`)
4. Paste into your AI interface

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
Replace {{FERMI_QUESTION}} with your estimation problem:
"How many piano tuners are there in Chicago?"
```

## Best Practices

### Choosing the Right Prompt

1. **For logical reasoning**: Start with `cot_prompt.txt` or `reflection_prompt.txt`
2. **For calculations**: Use `fermi.txt` or `deepdive.txt`
3. **For writing tasks**: Explore `prompts/writing/`
4. **For complex multi-faceted problems**: Try `abstract-prompt.txt` or `graph-of-thought-prompting.txt`
5. **For adaptive behavior**: Use `adaptive_dynamic_AI_assistant.txt`

### Optimization Tips

- **Combine prompts**: Many prompts can be used together (e.g., CoT + Reflection)
- **Adjust detail levels**: Scale up/down the number of steps based on problem complexity
- **Iterate**: Use reflection prompts to refine outputs iteratively
- **Customize**: Modify prompts to match your specific domain or use case

## Advanced Usage

### Chaining Prompts

```
1. Use atomic_elements_prompt.txt to break down a complex task
2. Apply cot_prompt.txt to solve each atomic element
3. Use reflection_prompt.txt to validate the solution
```

### Prompt Engineering Techniques Featured

- **Chain-of-Thought (CoT)**: Step-by-step reasoning
- **Tree-of-Thought (ToT)**: Exploring multiple reasoning branches
- **Graph-of-Thought (GoT)**: Concept relationship mapping
- **Meta-Prompting**: Self-improving prompts
- **ReAct**: Reasoning + Acting framework
- **Synthetic Prompting**: Learning through generated examples
- **Recursive Decomposition**: Breaking problems into subproblems

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
- Code review and optimization

## Contributing

Contributions are welcome! When adding new prompts:

1. Place them in the appropriate category directory
2. Use descriptive filenames (lowercase with underscores or hyphens)
3. Include comments explaining placeholder variables
4. Add examples where helpful
5. Update this README with a description

## File Naming Conventions

- Use lowercase with underscores or hyphens
- Be descriptive: `chain_of_thought.txt` not `cot.txt`
- Indicate technique: `*_prompt.txt`, `*_framework.txt`
- Match content to filename

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
