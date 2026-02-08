# Reasoning & Problem Solving Prompts

Advanced prompts for structured thinking, logical analysis, and complex problem-solving.

## Prompts in This Category

### Chain of Thought with Reflection (`cot_prompt.txt`)
A structured reasoning framework that separates the thinking process from the final output.

**Key Features:**
- Step-by-step reasoning within `<thinking>` tags
- Self-reflection to catch errors in `<reflection>` tags
- Final answer in `<output>` tags

**Best Used For:**
- Complex analytical questions
- Multi-step logical reasoning
- Problems requiring error checking

**Example Usage:**
```
Query: Explain how blockchain ensures data integrity
[Apply CoT prompt framework]
```

---

### Multi-stage Reflection Framework (`reflection_prompt.txt`)
A comprehensive approach emphasizing iterative thinking and validation.

**Key Features:**
- Structured thinking → reflection → output flow
- Multiple reflection checkpoints
- Clear separation of internal reasoning from user response

**Best Used For:**
- High-stakes decision making
- Complex analysis requiring verification
- Problems where accuracy is critical

---

### Deep Dive Problem Analysis (`deepdive.txt`)
A 3-phase rigorous approach for mathematical and constraint-based problems.

**Key Features:**
- Phase 1: Deep analysis & constraint identification
- Phase 2: Systematic equation building
- Phase 3: Rigorous validation & refinement
- Includes dimensional analysis and sanity checks

**Best Used For:**
- Mathematical word problems
- Physics problems
- Constraint-based optimization
- Engineering calculations

**Example:**
The prompt includes a detailed worked example of a canoe upstream/downstream problem.

---

### Advanced Problem Solver (`sophisticated_verbal_problem_solving.txt`)
A meta-level problem-solving framework combining multiple strategies.

**Key Features:**
- Dynamic approach selection (Zero-shot CoT, Few-shot CoT, Least-to-Most, Tree-of-Thought)
- ReAct framework integration
- Context generation and analogical reasoning
- Counterfactual analysis

**Best Used For:**
- Open-ended complex problems
- Problems requiring creative solutions
- Multi-faceted analysis
- Research questions

---

## Comparison Guide

| Prompt | Complexity | Structure | Validation | Best For |
|--------|-----------|-----------|------------|----------|
| CoT | Medium | Moderate | Single reflection | General reasoning |
| Reflection | Medium-High | Rigid | Multiple checkpoints | High-stakes decisions |
| Deep Dive | High | Very rigid | Comprehensive | Math & constraints |
| Advanced | Very High | Flexible | Multi-method | Open-ended problems |

## Usage Tips

1. **Start Simple**: Begin with `cot_prompt.txt` for most reasoning tasks
2. **Scale Up**: Use `reflection_prompt.txt` when you need extra verification
3. **Math Problems**: Always use `deepdive.txt` for mathematical word problems
4. **Complex Tasks**: Use `sophisticated_verbal_problem_solving.txt` for multi-faceted challenges

## Combining Techniques

These prompts can be combined:
- Use Deep Dive for problem decomposition, then CoT for solving each component
- Apply Reflection framework as a final validation step for any prompt
- Use Advanced Problem Solver to generate approach, then execute with CoT
