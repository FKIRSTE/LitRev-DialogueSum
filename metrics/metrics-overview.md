# Evaluation Metrics for Dialogue Summarization

This page provides a comprehensive overview of metrics used to evaluate dialogue summarization systems, organized by category.

## Metric Categories Overview

| Category | Description | Popular Metrics | Usage Count |
|----------|-------------|-----------------|-------------|
| **Count-based** | Lexical overlap between generated and reference summaries | ROUGE, BLEU, METEOR | 127, 21, 3 |
| **Model-based** | Neural models to assess semantic similarity and quality | BERTScore, BARTScore, FactCC | 38, 13, 9 |
| **QA-based** | Question generation and answering to assess faithfulness | FEQA, SummaQA, QuestEval | 38, 3, 3 |
| **Human Evaluation** | Manual assessment by human annotators | Likert scales, pairwise comparison | Various |

## 1. Count-Based Metrics

### ROUGE (Recall-Oriented Understudy for Gisting Evaluation)
- **Usage**: 127 papers
- **Year**: 2004
- **Description**: Measures recall of n-gram overlap between generated and reference summaries
- **Variants**: ROUGE-1 (unigrams), ROUGE-2 (bigrams), ROUGE-L (longest common subsequence)
- **Strengths**: Simple to implement, fast computation, established baseline
- **Limitations**: Limited semantic understanding, penalizes paraphrasing, less effective for abstractive summarization
- **Key Paper**: Lin (2004)

### BLEU (Bilingual Evaluation Understudy)
- **Usage**: 21 papers
- **Year**: 2002
- **Description**: Measures precision of n-gram overlap, originally for machine translation
- **Strengths**: Supports multiple references, established in NLP
- **Limitations**: Poor correlation with human judgments for summarization
- **Key Paper**: Papineni et al. (2002)

### METEOR (Metric for Evaluation of Translation with Explicit ORdering)
- **Usage**: 3 papers
- **Year**: 2005
- **Description**: Incorporates both precision and recall with synonym matching
- **Strengths**: Better handling of synonyms, more semantic awareness than ROUGE/BLEU
- **Limitations**: More complex to implement, still limited in semantic understanding
- **Key Paper**: Banerjee & Lavie (2005)

### chrF++
- **Usage**: 2 papers
- **Year**: 2017
- **Description**: Character and word n-gram F-score
- **Strengths**: Better for morphologically rich languages, robust to slight word variations
- **Limitations**: Less established in summarization literature
- **Key Paper**: Popović (2017)

### CIDEr (Consensus-based Image Description Evaluation)
- **Usage**: 3 papers
- **Year**: 2015
- **Description**: Consensus-based evaluation using TF-IDF weighting
- **Strengths**: Handles multiple references well, uses TF-IDF to focus on informative words
- **Limitations**: Initially designed for image captioning
- **Key Paper**: Vedantam et al. (2015)

### Perplexity
- **Usage**: 3 papers
- **Year**: 1977
- **Description**: Measures how well a probability model predicts a sample
- **Strengths**: Good for assessing fluency, model-independent
- **Limitations**: Doesn't measure content quality or accuracy
- **Key Paper**: Jelinek et al. (1977)

## 2. Model-Based Metrics

### BERTScore
- **Usage**: 38 papers
- **Year**: 2019
- **Description**: Uses BERT embeddings to compute similarity between tokens
- **Strengths**: Better semantic understanding, handles synonyms and paraphrasing
- **Limitations**: Computationally expensive, may not align perfectly with human judgment
- **Key Paper**: Zhang et al. (2020)

### BARTScore
- **Usage**: 13 papers
- **Year**: 2021
- **Description**: Calculates likelihood of generating reference from candidate and vice versa
- **Strengths**: Evaluates both fluency and accuracy, directional evaluation possible
- **Limitations**: Requires BART model, domain dependence
- **Key Paper**: Yuan et al. (2021)

### FactCC
- **Usage**: 9 papers
- **Year**: 2019
- **Description**: Evaluates factual consistency using entailment classifier
- **Strengths**: Focuses on factuality, task-specific for summarization
- **Limitations**: May miss subtle factual errors, limited by entailment model capabilities
- **Key Paper**: Kryscinski et al. (2020)

### BLEURT (BERT-based Learned Evaluation Understudy for Reference-less Translation)
- **Usage**: 7 papers
- **Year**: 2020
- **Description**: BERT model fine-tuned on human judgments
- **Strengths**: Closer to human evaluation, pre-trained for this purpose
- **Limitations**: Less transparent than simpler metrics
- **Key Paper**: Sellam et al. (2020)

### BLANC (BERT-based Learning for Answer Necessary Correctness)
- **Usage**: 2 papers
- **Year**: 2020
- **Description**: Measures how helpful a summary is for filling in blanks
- **Strengths**: Measures utility of summary, no reference needed
- **Limitations**: Indirect measure of quality
- **Key Paper**: Vasilyev et al. (2020)

### MoverScore
- **Usage**: 3 papers
- **Year**: 2019
- **Description**: Uses BERT embeddings with Word Mover's Distance
- **Strengths**: Flexible word alignment, handles many-to-one mapping
- **Limitations**: Computationally expensive
- **Key Paper**: Zhao et al. (2019)

## 3. QA-Based Metrics

### FEQA (Faithfulness Evaluation for Question Answering)
- **Usage**: 38 papers
- **Year**: 2020
- **Description**: Generates questions from summary, answers using source
- **Strengths**: Directly measures factuality, intuitive approach
- **Limitations**: Depends on QA system quality, limited by question generation
- **Key Paper**: Durmus et al. (2020)

### SummaQA
- **Usage**: 3 papers
- **Year**: 2019
- **Description**: Generates questions from source, answers using summary
- **Strengths**: Measures informativeness, complementary to FEQA
- **Limitations**: May not capture all important information
- **Key Paper**: Scialom et al. (2019)

### QuestEval
- **Usage**: 3 papers
- **Year**: 2021
- **Description**: Combines both FEQA and SummaQA approaches
- **Strengths**: More comprehensive evaluation, bidirectional assessment
- **Limitations**: Complex implementation, combines limitations of both approaches
- **Key Paper**: Scialom et al. (2021)

## 4. Human Evaluation

### Performance Assessment

#### Likert Scale
- **Usage**: 6 papers
- **Description**: Rating summaries on ordinal scales (e.g., 1-5)
- **Strengths**: Simple to implement, familiar to annotators
- **Limitations**: Subject to individual bias, limited detail on specific issues
- **Key Papers**: Feng et al. (2021), Lu et al. (2022)

#### Pairwise Comparison
- **Usage**: 9 papers
- **Description**: Choosing better summary between two alternatives
- **Strengths**: More reliable than absolute judgments, clearer distinction between systems
- **Limitations**: Limited to comparing two systems at a time
- **Key Papers**: Elder et al. (2018), Liu et al. (2021)

#### Best-Worst Scaling
- **Usage**: 5 papers
- **Description**: Selecting best and worst summaries from a set
- **Strengths**: Higher reliability than Likert scales, better statistical properties
- **Limitations**: More complex for annotators, requires careful design
- **Key Papers**: Kiritchenko & Mohammad (2017), Rothe et al. (2020)

### Agreement Metrics

#### Krippendorff's Alpha
- **Usage**: 2 papers
- **Description**: Measures disagreement across multiple raters
- **Strengths**: Flexible for different measurement types, handles missing data
- **Target Range**: 0.65-0.85 (reported)
- **Key Paper**: Krippendorff (1970)

#### Cohen's Kappa
- **Usage**: 3 papers
- **Description**: Measures agreement between two raters
- **Strengths**: Good for categorical assessments and binary judgments
- **Target Range**: 0.65-0.85 (reported)
- **Key Paper**: Cohen (1960)

#### Fleiss' Kappa
- **Usage**: 2 papers
- **Description**: Extension of Cohen's Kappa for multiple raters
- **Strengths**: Handles fixed categories with multiple annotators
- **Target Range**: 0.65-0.85 (reported)
- **Key Paper**: Fleiss (1971)

## Evaluated Characteristics

| Category | Characteristic | Description | Common Metrics |
|----------|----------------|-------------|----------------|
| **Accuracy** | Factuality | Adherence to facts in the source | FactCC, FEQA, QuestEval |
| **Content** | Relevance | Importance of included information | ROUGE, Human evaluation |
|  | Coverage | Inclusion of all key topics | ROUGE-L, Human evaluation |
|  | Informativeness | Depth and usefulness of information | SummaQA, Human evaluation |
| **Readability** | Coherence | Logical flow and connections | Human evaluation, BARTScore |
|  | Structure | Organization of information | Human evaluation |
|  | Conciseness | Brevity without redundancy | Human evaluation |
| **Style** | Consistency | Uniform perspective and tense | Human evaluation |
|  | Fluency | Grammatical correctness | Perplexity, Human evaluation |

## Recent Developments in Evaluation

### LLM-Based Evaluation
- **GEMBA**: LLM-based evaluation metric (Kocmi & Federmann, 2023)
- **ICE**: Multi-dimensional evaluation using LLMs (Jain et al., 2023)
- Advantages: Customizable, aligned with human judgment
- Status: Emerging area with limited exploration in dialogue summarization

### Limitations of Current Metrics
Recent analyses (Gao & Wan, 2022; Kirstein et al., 2024) highlight limitations:
- Established metrics provide only superficial understanding of model performance
- Poor alignment with human judgment in discerning error nuances
- Individual metrics fail to adequately reflect specific error types (e.g., hallucination)
- Impact of information omission is difficult to quantify

### Recommendation for Evaluation
Use a composite approach combining:
1. Count-based metrics (e.g., ROUGE) for basic coverage
2. Model-based metrics (e.g., BERTScore) for semantic similarity
3. QA-based metrics (e.g., FEQA) for faithfulness
4. Human evaluation for holistic assessment
