# Writing & Content Creation Prompts

Professional-grade prompts for content generation, summarization, review, and evaluation.

## Prompts in This Category

### Expert 10-Stage Summarization (`summarisation.txt`)

World-class text summarization with comprehensive quality control.

**Process Stages:**
1. Comprehensive reading and analysis
2. Content prioritization
3. Linguistic analysis
4. Contextualization
5. Summary drafting
6. Accuracy check
7. Clarity and coherence enhancement
8. Final polishing
9. Self-criticism and refinement
10. Meta-analysis

**Output Includes:**
- Polished summary (exact word count)
- Key points captured
- Omitted information notes
- Tone/style preservation assessment
- Challenges in summarization
- Confidence score (95-100)
- Meta-analysis reflection

**Best For:**
- Academic paper summaries
- Executive briefings
- Technical documentation condensation
- Literature reviews

**Variables:**
- `{text}`: Text to summarize
- `{desired_length}`: Target word count

---

### Factual Consistency Checker (`factual-consistency-summarisation.txt`)

Simple but critical validation tool for summary accuracy.

**Purpose:**
Evaluates if a summary contains factual inconsistencies or misleading information not supported by source text.

**Variables:**
- `{{Document}}`: Original source text
- `{{Summary}}`: Summary to validate

**Output:**
Yes/No answer on factual consistency

**Best For:**
- Quality control in summarization pipelines
- Academic integrity verification
- News summary validation
- Legal document review

---

### Publication-Quality Review (`editorial_review_prompt.txt`)

Comprehensive editorial review based on professional style guides.

**Review Criteria:**

**a) Style and Tone**
- Confident, engaging, well-informed writing
- Brief, comprehensible, and clever tone
- Fair and impartial stance

**b) Language and Grammar**
- English spelling and grammar
- Active voice usage
- Sentence and paragraph length
- Punctuation correctness

**c) Numbers and Dates**
- Number formatting
- Percentages and monetary values
- Day-month-year format
- 24-hour clock times

**d) Citations and References**
- Accuracy and consistency
- Appropriate formats
- Hyperlinks for online sources

**e) Headlines and Subheadings**
- Clarity and engagement
- Effective text organization
- Proper capitalization

**f) Fact-checking and Accuracy**
- Verification requirements
- Name, title, and association accuracy

**g) Inclusive Language**
- Gender-inclusive language
- Absence of stereotypes
- Respectful treatment of identities
- Cultural sensitivity

**h) Legal and Ethical Considerations**
- Ethical issues identification
- Copyright concerns

**Output Format:**
- Overall assessment
- Strengths (2-3 key points)
- Areas for improvement (3-5 specific)
- Specific recommendations (3-5 actionable)
- Conclusion with critical changes

**Best For:**
- Magazine/newspaper article review
- Blog post editing
- Academic writing improvement
- Professional content quality assurance

**Variables:**
- `{{ARTICLE_TEXT}}`: Article to review

---

### Expert Q&A Generation (`generate_expert_qna_prompt.txt`)

Creates high-quality question-answer pairs for training or assessment.

**Best For:**
- Creating training datasets
- Knowledge assessment design
- FAQ generation
- Educational material development

---

### Response Comparison & Ranking (`generate-verbal-feedback-in-pairwise-ranking.txt`)

Detailed comparative analysis framework for evaluating two responses.

**Key Features:**
- Experienced editor persona
- Critical deep analysis
- Direct comparison approach
- Focus on commonalities and differences
- No explicit reference to "reference answer"
- Structured reasoning chain

**Input Components:**
- Instruction (user query)
- Response A
- Response B
- Reference Answer (hidden from feedback)
- Score Rubric

**Output:**
Detailed feedback explaining which response is better and why, ending with `[END]`.

**Best For:**
- Model evaluation
- Preference learning
- A/B testing
- Content quality comparison
- Training data for RLHF (Reinforcement Learning from Human Feedback)

**Variables:**
- `{sub_str}`: Placeholder for comparison conclusion

---

## Category Overview

| Prompt | Primary Use | Output Type | Complexity |
|--------|-------------|-------------|------------|
| Summarization | Condensing text | Structured summary | High |
| Factual Consistency | Validation | Yes/No | Low |
| Editorial Review | Quality control | Detailed feedback | Medium |
| Q&A Generation | Dataset creation | Question-answer pairs | Medium |
| Response Comparison | Evaluation | Comparative analysis | Medium-High |

## Workflow Examples

### Academic Paper Processing
```
1. Use summarisation.txt to create initial summary
2. Apply factual-consistency-summarisation.txt to validate
3. Run editorial_review_prompt.txt for style improvement
```

### Content Quality Pipeline
```
1. Generate multiple drafts
2. Use response comparison to select best version
3. Apply editorial review for final polish
4. Validate facts with consistency checker
```

### Training Data Generation
```
1. Use generate_expert_qna_prompt.txt to create Q&A pairs
2. Generate multiple answers per question
3. Use response comparison to rank answers
4. Build preference dataset for fine-tuning
```

## Best Practices

### For Summarization
- Always specify target word count
- Consider your audience when setting length
- Use factual consistency check as validation
- Iterate if confidence score is below 98

### For Editorial Review
- Provide complete style guide context
- Review in multiple passes (content → style → technical)
- Prioritize recommendations by impact
- Consider audience and publication venue

### For Response Comparison
- Ensure responses are comparable (same task)
- Use clear, specific evaluation criteria
- Focus on meaningful differences, not minor variations
- Document reasoning process thoroughly

## Integration with Other Categories

**With Reasoning Prompts:**
- Use CoT for complex editorial decisions
- Apply reflection for important reviews

**With Advanced Techniques:**
- Graph-of-Thought for content structure analysis
- Mystery Solver for investigative journalism review

**With Meta-Utility:**
- Adaptive assistant for versatile content creation
- Meta-codes for standardized review workflows
