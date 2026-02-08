# Advanced Techniques

Cutting-edge prompting strategies combining multiple methodologies for complex problem-solving.

## Prompts in This Category

### Graph-of-Thought Prompting (`graph-of-thought-prompting.txt`)

Visualizes complex concepts as interconnected graphs of ideas.

**16-Step Process:**
1. Initial Nodes (5-7 key concepts)
2. Node Expansion (relevance, sub-ideas, challenges)
3. Edge Identification (relationships and strengths)
4. Cluster Analysis (thematic grouping)
5. Bridge Concepts (connecting different clusters)
6. Feedback Loops (circular relationships)
7. External Influences (outside factors)
8. Temporal Dynamics (evolution over time)
9. Emergent Patterns (unexpected insights)
10. Graph Refinement (optimization)
11. Alternative Perspectives (stakeholder views)
12. Solution Pathways (problem-solving routes)
13. Knowledge Gaps (uncertainty identification)
14. Synthesis (key insights summary)
15. Action Steps (concrete next steps)
16. Reflection (process evaluation)

**Best For:**
- Complex systems analysis
- Strategic planning
- Relationship mapping
- Multi-stakeholder problems
- Research topic exploration

**Variables:**
- `{{USER_QUERY}}`: Query or problem to analyze

**Example Applications:**
- Business strategy development
- Scientific research planning
- Policy analysis
- Technology ecosystem mapping

---

### Synthetic Reasoning (`synthetic_reasoning_prompt.txt`)

Learns through generated examples using backward and forward reasoning.

**Strategy:**
- **Backward Process**: Generate simpler related questions
- **Forward Process**: Build up to complex answer
- Creates reasoning chains through synthetic examples

**Process:**
1. Start with target question
2. Generate simpler related questions (backward)
3. Answer simpler questions
4. Build forward to complex answer
5. Synthesize insights

**Includes Two Seed Examples:**
1. Photosynthesis and carbon cycle (moderate complexity)
2. AI impact on job market (high complexity)

**Best For:**
- Learning new domains
- Building intuition
- Analogical reasoning
- Educational content
- Research exploration

---

### Mystery Solver (`mystery_solver.txt`)

Detective-style investigation framework for complex problem-solving.

**Persona:**
World-class detective combining Sherlock Holmes, House MD, and elite intelligence agencies.

**Core Structure:**
Uses component-based architecture:
- `<Component>`: Task decomposition
- `<Objective>`: Goal definition
- `<Input>`: Information gathering
- `<Process>`: Analysis methodology
- `<Output>`: Results presentation
- `<Continuation>`: Next steps
- `<Conclusion>`: Reflection and improvement

**Integrated Techniques:**
1. **Meta-Prompting**: Prompts within prompts
2. **Modularity**: Distinct investigation modules
3. **Abstraction**: Pattern identification
4. **Iteration**: Hypothesis refinement
5. **Debugging**: Hypothesis validation
6. **Graph-of-Thought**: Logical connection mapping
7. **React Technique**: Dynamic component updates
8. **Plan-to-Execute**: Structured investigation
9. **Reflection**: Process improvement

**Best For:**
- Complex investigations
- Root cause analysis
- Debugging (code or systems)
- Research mysteries
- Multi-step problem chains

---

### Abstract Prompt (`abstract-prompt.txt`)

Multi-faceted problem-solving combining numerous advanced techniques.

**Framework Components:**
1. **Context & Analogy Integration**: Generate relevant context and analogies
2. **Question Reformulation**: Multiple phrasings for clarity
3. **Counterfactual Analysis**: "What if" scenarios
4. **Approach Selection**: Zero-shot CoT, Few-shot CoT, Least-to-Most, Tree-of-Thought
5. **Problem Decomposition**: Structured representation
6. **Multi-Faceted Reasoning**: ReAct + Tree-of-Thought
7. **Dynamic Adjustment**: Real-time strategy refinement

**Key Features:**
- Meta-prompting for self-improvement
- Multiple reasoning paths
- Comprehensive validation
- Adaptive methodology

**Best For:**
- Open-ended research questions
- Strategic analysis
- Complex decision-making
- Novel problem types
- Academic research

---

### Atomic Action Decomposition (`atomic_elements_prompt.txt`)

Breaks complex goals into atomic, actionable steps.

**Two-Phase Approach:**

**Phase 1: Graph-of-Thought (Backward)**
- Start with target narrative/goal
- Work backward to identify subgoals
- Construct dependency graph
- Identify means to achieve goal

**Phase 2: Recursive Chain-of-Thought (Forward)**
- Start with first means from graph
- Recursively break down into smaller steps
- Continue until reaching atomic actions
- Single logical step = stopping condition

**Example Included:**
Novel enzyme discovery narrative decomposition

**Best For:**
- Project planning
- Complex goal achievement
- Scientific narrative construction
- Process documentation
- Task breakdown for delegation

**Variables:**
- `[TARGET NARRATIVE SUMMARY]`: Desired outcome (~300 words)

---

### Symbolic Reasoning (`prompt_chain_of_symbols.txt`)

Uses compact symbolic notation for spatial and logical reasoning.

**Notation System:**
- `↑` : above
- `↓` : below
- `→` : right
- `←` : left
- `=` : touching
- `∞` : far from

**Example:**
```
Original: "A small blue square is far above a small blue circle"
Symbolic: A: (small, blue, square) ∞↑ (small, blue, circle)
```

**Benefits:**
- Reduces cognitive load
- Clarifies spatial relationships
- Enables logical deduction
- Minimizes ambiguity

**Best For:**
- Geometry problems
- Spatial reasoning puzzles
- Logic problems
- Abstract reasoning tests
- Relationship mapping

**Example Problems Included:**
Block-based spatial reasoning with multiple objects and relationships

---

## Comparison Matrix

| Technique | Complexity | Structure | Learning Curve | Best Domain |
|-----------|-----------|-----------|----------------|-------------|
| Graph-of-Thought | High | Flexible | Medium | Systems analysis |
| Synthetic Reasoning | Medium | Structured | Low | Learning/Education |
| Mystery Solver | Very High | Modular | High | Investigation |
| Abstract Prompt | Very High | Comprehensive | Very High | Research |
| Atomic Elements | High | Two-phase | Medium | Planning |
| Symbolic Reasoning | Medium | Notation-based | Medium | Spatial/Logic |

## When to Use Which

### For Analysis Tasks
- **System-level**: Graph-of-Thought
- **Investigation**: Mystery Solver
- **Research**: Abstract Prompt

### For Planning Tasks
- **Goal decomposition**: Atomic Elements
- **Project planning**: Atomic Elements + Graph-of-Thought

### For Learning Tasks
- **New concepts**: Synthetic Reasoning
- **Pattern recognition**: Graph-of-Thought

### For Logic Tasks
- **Spatial reasoning**: Symbolic Reasoning
- **Complex deduction**: Mystery Solver

## Advanced Combinations

### Research Project
```
1. Graph-of-Thought: Map research landscape
2. Atomic Elements: Break into research tasks
3. Synthetic Reasoning: Build understanding of each area
4. Abstract Prompt: Synthesize findings
```

### Complex Investigation
```
1. Mystery Solver: Framework setup
2. Graph-of-Thought: Relationship mapping
3. Symbolic Reasoning: Formal logic representation
4. Synthetic Reasoning: Generate hypotheses
```

### Strategic Planning
```
1. Abstract Prompt: Multi-faceted analysis
2. Graph-of-Thought: Stakeholder mapping
3. Atomic Elements: Action plan decomposition
```

## Technical Notes

### Computational Complexity
These prompts may require:
- Extended context windows (>8K tokens)
- Multiple inference passes
- Significant compute resources
- Longer response times

### Model Requirements
Recommended for:
- GPT-4 or equivalent
- Claude Opus/Sonnet
- Gemini Pro/Ultra
- Command R+

May not work well with:
- Smaller models (<7B parameters)
- Non-instruction-tuned models
- Models without strong reasoning capabilities

## Best Practices

1. **Start Specific**: Provide clear, well-defined problems
2. **Allow Time**: These techniques require thorough processing
3. **Iterate**: Use outputs as inputs for refinement
4. **Combine Selectively**: Don't use all techniques simultaneously
5. **Validate**: Cross-check results with simpler methods
6. **Document**: Track reasoning paths for future reference

## Academic Foundations

These techniques are based on recent AI research:
- Graph-of-Thought: [arXiv:2308.09687](https://arxiv.org/abs/2308.09687)
- Tree-of-Thought: [arXiv:2305.10601](https://arxiv.org/abs/2305.10601)
- Chain-of-Thought: [arXiv:2201.11903](https://arxiv.org/abs/2201.11903)
- ReAct: [arXiv:2210.03629](https://arxiv.org/abs/2210.03629)
