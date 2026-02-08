# Estimation & Mathematical Reasoning

Specialized prompts for quantitative reasoning, approximation, and back-of-the-envelope calculations.

## Prompts in This Category

### Comprehensive Fermi Estimation Framework (`fermi.txt`)

A world-class framework for solving Fermi estimation problems with exceptional rigor.

**Key Features:**
- 15-step comprehensive process
- Multiple validation loops
- Iterative rephrasing for accuracy
- Scientific notation throughout
- Three worked examples (simple to highly complex)

**Process Overview:**
1. Initial question analysis and rephrasing
2. Question reframing and scope definition
3. Problem decomposition and visual mapping
4. Assumption articulation and justification
5. Multi-disciplinary data gathering
6. Estimation techniques application
7. Calculation execution and documentation
8. Sensitivity analysis and error estimation
9. Cross-validation and sanity checking
10. Iterative refinement process
11. Comprehensive result presentation
12. Limitation acknowledgment
13. Final re-reading and verification
14. Reiterative rephrasing
15. Cross-validation of rephrased solution

**Example Problems Included:**

**Example 1: Moderate Complexity**
- **Question:** How many piano strings are tuned annually worldwide?
- **Approach:** Population-based estimation with categorical breakdown
- **Result:** ~21 billion strings/year

**Example 2: High Complexity**
- **Question:** How many photons from Betelgeuse have interacted with DNA molecules on Earth in the last century?
- **Approach:** Multi-domain physics calculation (astrophysics + biology)
- **Result:** ~4.78 × 10^36 photons

**Main Example: Very High Complexity**
- **Question:** Canoe upstream/downstream word problem with multiple constraints
- **Demonstrates:** Full framework application including constraint identification

## When to Use Fermi Estimation

**Perfect For:**
- Order-of-magnitude calculations
- "Guesstimate" problems in interviews
- Resource planning and capacity estimation
- Scientific approximations
- Market sizing questions
- Physics and astronomy calculations

**Not Ideal For:**
- Precise calculations requiring exact values
- Problems with readily available data
- Simple arithmetic

## Key Techniques Demonstrated

1. **Problem Rephrasing**: Multiple attempts to extract critical information
2. **Assumption Documentation**: Explicit listing with justifications
3. **Dimensional Analysis**: Tracking units throughout
4. **Scientific Notation**: Maintaining precision at scale
5. **Cross-Validation**: Verifying results through multiple methods
6. **Sensitivity Analysis**: Understanding key variables

## Usage Tips

### 1. Replace the Placeholder
```
Find: {{FERMI_QUESTION}}
Replace with your estimation problem
```

### 2. Use Liberal Scratchpad
The prompt emphasizes using `<scratchpad>` for complex calculations:
```xml
<scratchpad>
Step 1: Define variables
- World population: 8 billion
- Assumptions: ...
</scratchpad>
```

### 3. Follow the Rephrasing Loop
The prompt includes a critical validation step:
- Solve the original question
- Rephrase iteratively (becoming more abstract)
- Solve the most abstract version
- Compare results - if they differ, find the flaw

### 4. Output Format
The prompt specifies:
- Work within `<answer>` tags
- Remove XML tags from user-facing response
- Use proper formatting (headings, spacing, emphasis)
- Include confidence intervals when applicable

## Fermi Estimation Principles

### The 80/20 Rule
Focus on the 20% of factors that drive 80% of the result.

### Order of Magnitude Thinking
Being within 10x is often good enough:
- 10^6 vs 10^7: Acceptable
- 10^3 vs 10^9: Problem in reasoning

### Bounds Checking
Establish upper and lower bounds:
- Optimistic estimate
- Pessimistic estimate
- Geometric mean as final answer

## Examples of Good Fermi Questions

1. **Business**: How many gas stations are there in the United States?
2. **Physics**: What is the total energy output of the sun in one year?
3. **Biology**: How many cells are in the human body?
4. **Technology**: How much data is transmitted over the internet per day?
5. **Environment**: How many trees are there on Earth?

## Advanced Features

### Multi-Domain Integration
The prompt explicitly calls for:
- Consulting diverse sources
- Cross-referencing across fields
- Benchmarking against known quantities

### Error Quantification
Built-in sensitivity analysis:
- Identify key variables
- Perform uncertainty quantification
- Present confidence intervals

### Iterative Refinement
Structured improvement process:
- Define refinement criteria
- Execute improvement cycles
- Document evolution of estimate

## Common Pitfalls to Avoid

1. **Forgetting Units**: Always track dimensional consistency
2. **Compound Errors**: Small errors multiply in multi-step calculations
3. **Unrealistic Assumptions**: Ground assumptions in reality
4. **Skipping Validation**: Always sanity check results
5. **Over-Precision**: 3.7842 × 10^6 → Use 4 × 10^6

## Academic References

The Fermi estimation technique is named after physicist Enrico Fermi, who was known for his ability to make good approximate calculations with little or no actual data.

**Famous Fermi Problems:**
- Fermi's original: How many piano tuners in Chicago? (1930s)
- Drake Equation: Estimating intelligent civilizations in the galaxy
- Manhattan Project: Various radiation and yield calculations
