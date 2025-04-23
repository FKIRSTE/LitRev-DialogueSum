# Salience Challenge

The salience challenge involves identifying and focusing on the most relevant information within a dialogue, including content critical for insightful summaries and information relevant to specific audiences.

## Sub-challenges
- Identifying content critical for insightful summaries
- Aligning summaries with different viewpoints, values, and ethics
- Locating relevant text spans in lengthy dialogues
- Adapting to dynamic, evolving information flow
- Personalizing summaries to individual needs

## Progress
**Status**: 🟠 Good progress through contrastive learning and prompt engineering

## Representative Papers

| Year | Title | Authors | Venue | Key Contribution |
|------|-------|---------|-------|-----------------|
| 2021 | Controllable Neural Dialogue Summarization with Personal Named Entity Planning | Liu, Z., & Chen, N. | EMNLP | Entity-focused planning for personalized summaries |
| 2023 | SWING: Balancing Coverage and Faithfulness for Dialogue Summarization | Huang, K.-H., et al. | EACL Findings | Balancing content coverage and factuality |
| 2023 | Human-in-the-Loop Abstractive Dialogue Summarization | Chen, J., Dodda, M., & Yang, D. | ACL Findings | Interactive summarization with human feedback |
| 2021 | Learn to Copy from the Copying History: Correlational Copy Network for Abstractive Summarization | Li, H., et al. | EMNLP | Enhanced copy mechanism for salient content |
| 2022 | TCS WITM 2022 @ DialogSum: Topic Oriented Summarization Using Transformer Based Encoder Decoder Model | Chauhan, V., et al. | INLG | Topic-oriented summarization with content filtering |
| 2023 | MACSum: Controllable Summarization with Mixed Attributes | Zhang, Y., et al. | TACL | Controllable summarization with mixed attributes |
| 2023 | Socratic Pretraining: Question-Driven Pretraining for Controllable Summarization | Pagnoni, A., et al. | ACL | Question-driven pre-training for salience identification |
| 2022 | Hybrid Multi-Document Summarization Using Pre-Trained Language Models | Ghadimi, A., & Beigy, H. | Expert Systems With Applications | Combining extraction and abstraction for salient content |
| 2020 | Multi-View Sequence-to-Sequence Models with Conversational Structure for Abstractive Dialogue Summarization | Chen, J., & Yang, D. | EMNLP | Multi-view approach to identify salient information |
| 2023 | Enhancing Dialogue Summarization with Topic-Aware Global- and Local-Level Centrality | Liang, X., et al. | EACL | Topic-aware centrality for identifying important content |

## Primary Approach Categories

| Approach | Description | Key Papers |
|----------|-------------|------------|
| **Training tasks** | Distinguishing between salient and non-salient content | Chauhan et al. (2022), Liu et al. (2022), Ghadimi & Beigy (2022) |
| **Architecture modification** | Modified attention mechanisms for important content | Li et al. (2021), Hua et al. (2023) |
| **Human feedback** | Incorporating human judgment to identify importance | Chen et al. (2023) |
| **Loss function** | Special losses for missing or irrelevant information | Huang et al. (2023) |
| **Pre-processing** | Methods to identify and prioritize key entities | Liu & Chen (2021), Jung et al. (2023) |
| **Pre-training** | Question-driven pre-training to identify important content | Pagnoni et al. (2023), Zhang et al. (2023) |

## Related Datasets

| Dataset | Key Characteristics | Papers Using |
|---------|---------------------|--------------|
| SAMSum | Messaging app dialogues with diverse topics | 68 papers |
| AMI | Business meetings with defined agenda items | 63 papers |
| ICSI | Academic group meetings with research discussions | 21 papers |
| QMSum | Query-based summarization across diverse domains | 18 papers |
| SummScreen | TV series transcripts with plot developments | 8 papers |
| ConvoSumm | Dialogues from various sources with different focuses | 5 papers |

## Special Focus: Personalized Summarization

A growing area within the salience challenge is personalized summarization, which tailors content to specific user needs:

| Year | Title | Authors | Venue | Key Contribution |
|------|-------|---------|-------|-----------------|
| 2021 | Controllable Neural Dialogue Summarization with Personal Named Entity Planning | Liu, Z., & Chen, N. | EMNLP | Named entity planning for personalization |
| 2023 | Interactive User Interface for Dialogue Summarization | Jung, J., et al. | IUI | User-guided topic selection and emphasis |
| 2022 | CSDS: A Fine-Grained Chinese Dataset for Customer Service Dialogue Summarization | Lin, H., et al. | EMNLP | Role-oriented dialogue summarization |
| 2022 | Other Roles Matter! Enhancing Role-Oriented Dialogue Summarization via Role Interactions | Lin, H., et al. | ACL | Role interactions for personalized summaries |
| 2018 | Collabot: Personalized Group Chat Summarization | Tepper, N., et al. | WSDM | Personalized chat summarization system |

## Technical Approaches for Salience

### Content Prioritization Methods
- **Contrastive Learning**: Using positive and negative examples to distinguish important content
- **Entity Planning**: Prioritizing named entities to guide summary generation
- **Topic Modeling**: Identifying core topics as a basis for extracting salient information
- **Centrality Measures**: Computing various centrality metrics to identify key information

### Representation Techniques
- **Mixed-Attribute Control**: Explicitly modeling content attributes (length, specificity, etc.)
- **Global-Local Attention**: Balancing global document understanding with local detail focus
- **Query-Based Filtering**: Using explicit or implicit queries to filter important content
- **Importance Scoring**: Assigning importance scores to dialogue segments
