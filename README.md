# A Systematic Literature Review on the Challenges of Abstractive Dialogue
Summarization


A collection of papers and resources across the four principal components of dialogue summarization: Challenges, Techniques, Datasets, and Metrics.
The sub-folders contain our code to crawl the [Semantic Scholar](https://www.semanticscholar.org/) and [DBLP](https://dblp.org/) databases.
We intend to periodically update this repository for its ongoing relevance in the current era of LLMs. Stay tuned!

## Contents

- [Fundamentals](#fundamentals)
- [Papers](#papers)
  - [Challenges](#challenges)
  - [Techniques](#techniques)
  - [Datasets](#datasets)
  - [Metrics](#metrics) 
  - [Insightful Discussions](#insights)
- [Our Survey](#survey)


<a name="fundamentals" />

## Fundamentals
### Inclusion Criteria
1. long or short paper
2. open-access
3. published since 2019

### Exclusion Criteria
1. non-English primary dataset
2. multi-modal studies
3. focus on extractive summarization
4. usage of non-Transformer-based methods

### Anchor Terms
1. dialogue summarization
2. dialog summarization
3. conversation summarization

### Search Terms
1. technique
2. approach
3. dataset
4. evaluation
5. personalization
6. task
7. metric
8. language model
9. NLP
10. semantic representation
11. information extraction
12. text simplification
13. topic segmentation
14. ethic
15. cost
16. privacy
17. controllable
18. machine
19. automatic
20. training
21. co2
22. meeting summarization
23. chat summarization
24. customer service summarization
25. legal
26. email
27. interview
28. medical

<a name="papers" />

<a name="challenges" />

## Challenges
< Taxonomy goes here? >

|  **Challenges**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|  **arXiv**  | 2018 | A Discourse-Aware Attention Model for Abstractive Summarization of Long Documents `NAACL` [[Paper]](https://arxiv.org/abs/1804.05685) | Scientific |
| **Dataset** | 2022 | SQuALITY: Building a Long-Document Summarization Dataset the Hard Way `EMNLP` [[Paper]](https://arxiv.org/pdf/2205.11465.pdf) | Question-focused Summarization | 


<a name="techniques" />

## Techniques

|  **Technique**  | **Challenge** | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|  **arXiv**  | 2018 | 2018 | A Discourse-Aware Attention Model for Abstractive Summarization of Long Documents `NAACL` [[Paper]](https://arxiv.org/abs/1804.05685) | Scientific |
| **Dataset** | 2022 | 2022 | SQuALITY: Building a Long-Document Summarization Dataset the Hard Way `EMNLP` [[Paper]](https://arxiv.org/pdf/2205.11465.pdf) | Question-focused Summarization | 


<a name="datasets" />

## Datasets 
|  **Dataset**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|  **arXiv**  | 2018 | A Discourse-Aware Attention Model for Abstractive Summarization of Long Documents `NAACL` [[Paper]](https://arxiv.org/abs/1804.05685) | Scientific |
| **Dataset** | 2022 | SQuALITY: Building a Long-Document Summarization Dataset the Hard Way `EMNLP` [[Paper]](https://arxiv.org/pdf/2205.11465.pdf) | Question-focused Summarization | 

<a name="models" />


<a name="metrics" />

## Metrics

The metrics listed below are not specific to dialogue summarization (most summarization metrics are studied under a short/normal summarization setting). Our previous work investigated these metrics for the meeting summarization setting: <LREC LINK

<a name="count-based" />

### Count-based
|  **Metric**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|  **BLEU**  | 2002 | ROUGE: A Package for Automatic Evaluation of Summaries `ACL` [[Paper]](https://aclanthology.org/W04-1013/) | Hard Lexical Matching |
|  **ROUGE**  | 2004 | ROUGE: A Package for Automatic Evaluation of Summaries `ACL` [[Paper]](https://aclanthology.org/W04-1013/) | Hard Lexical Matching |
|  **METEOR**  | 2005 | ROUGE: A Package for Automatic Evaluation of Summaries `ACL` [[Paper]](https://aclanthology.org/W04-1013/) | Hard Lexical Matching |
|  **chrF++**  | 2017 | ROUGE: A Package for Automatic Evaluation of Summaries `ACL` [[Paper]](https://aclanthology.org/W04-1013/) | Hard Lexical Matching |
|  **CIDEr**  | 2015 | ROUGE: A Package for Automatic Evaluation of Summaries `ACL` [[Paper]](https://aclanthology.org/W04-1013/) | Hard Lexical Matching |
|  **Perplexity**  | 1977 | ROUGE: A Package for Automatic Evaluation of Summaries `ACL` [[Paper]](https://aclanthology.org/W04-1013/) | Hard Lexical Matching |

<a name="model-based" />

### Model-based
|  **Metric**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
| **BERTScore** | 2019 | BERTScore: Evaluating Text Generation with BERT `ICLR` [[Paper]](https://arxiv.org/abs/1904.09675?context=cs) | Soft Lexical Matching |
| **MoverScore** | 2019 | BERTScore: Evaluating Text Generation with BERT `ICLR` [[Paper]](https://arxiv.org/abs/1904.09675?context=cs) | Soft Lexical Matching |
| **BARTScore** | 2021 | BARTScore: Evaluating Generated Text as Text Generation `NeurIPS` [[Paper]](https://arxiv.org/abs/2106.11520) | Conditional Text Generation |
| **BLEURT** | 2019 | BERTScore: Evaluating Text Generation with BERT `ICLR` [[Paper]](https://arxiv.org/abs/1904.09675?context=cs) | Soft Lexical Matching |
| **BLANC** | 2019 | BERTScore: Evaluating Text Generation with BERT `ICLR` [[Paper]](https://arxiv.org/abs/1904.09675?context=cs) | Soft Lexical Matching |
|  **FactCC**  | 2019 | Evaluating the Factual Consistency of Abstractive Text Summarization `EMNLP` [[Paper]](https://arxiv.org/abs/1910.12840) | Data Augmentation + Textual Entailment |

<a name="qa-based" />

### QA-based
|  **Metric**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
| **SummaQA** | 2019 | FEQA: A Question Answering Evaluation Framework for Faithfulness Assessment in Abstractive Summarization `ACL` [[Paper]](https://arxiv.org/abs/2005.03754) | Question-Answering | 
| **FEQA** | 2020 | FEQA: A Question Answering Evaluation Framework for Faithfulness Assessment in Abstractive Summarization `ACL` [[Paper]](https://arxiv.org/abs/2005.03754) | Question-Answering | 
| **QuestEval** | 2021 | FEQA: A Question Answering Evaluation Framework for Faithfulness Assessment in Abstractive Summarization `ACL` [[Paper]](https://arxiv.org/abs/2005.03754) | Question-Answering | 

<a name="human-eval" />

### Human Evaluation
|  **Approach**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
| **OpenIE** | 2019 | Assessing The Factual Accuracy of Generated Text `KDD` [[Paper]](https://arxiv.org/abs/1905.13322) | Semantic Matching |
|  **FactCC**  | 2019 | Evaluating the Factual Consistency of Abstractive Text Summarization `EMNLP` [[Paper]](https://arxiv.org/abs/1910.12840) | Data Augmentation + Textual Entailment |
| **DAE** | 2020 | Evaluating Factuality in Generation with Dependency-level Entailment `EMNLP Findings` [[Paper]](https://arxiv.org/abs/2010.05478) | Textual Entailment | 


<a name="insights" />

## Insightful Discussion

Papers that provide insightful discussions related to dialogue summarization. 

### Summarization
|  **Topic**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|  **Metrics**  | 2020 | Re-evaluating Evaluation in Text Summarization `EMNLP` [[Paper]](https://arxiv.org/pdf/2010.07100.pdf) | On Effectiveness of Summarization Models and Metrics |
| **Models** | 2022 | DYLE: Dynamic Latent Extraction for Abstractive Long-Input Summarization `ACL` [[Paper]](https://arxiv.org/abs/2110.08168) | Insighful Approach+Discussion into Extract-then-Summarize Models | 

### General 
|  **Topic**  | **Year** | **Title**                                       |                          **tl;dr**                           |
| :--------: |:---- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|  **Efficient Attention**  | 2020 | Efficient Transformer: A Survey `ACM Comput. Surv.` [[Paper]](https://arxiv.org/pdf/2009.06732.pdf) | Practicality of Efficient Attention (section 4.4) |
| **Fine-tuning** | 2022 | A Closer Look at How Fine-tuning Changes BERT `ACL` [[Paper]](https://aclanthology.org/2022.acl-long.75/) | How Representation Changes after Fine-tuning | 

<a name="survey" />

## A Systematic Literature Review on the Challenges of Abstractive Dialogue Summarization
```
maybe ref to arxiv?
```
