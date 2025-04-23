# Structure Challenge

The structure challenge focuses on extracting a conversation's built-up, identifying topic flow, dialogue phases, and analyzing utterance dependencies to create an ordered summary based on the extracted structures.

## Sub-challenges
- Topic flow (relationships between discussion topics and transitions)
- Dialogue phases (e.g., problem identification, decision making)
- Utterance dependency (relationships between utterances across turns)
- Long-range dependencies (tracking relationships across distant parts of dialogue)

## Progress
**Status**: 🟠 Good progress through graph structures and multi-stage approaches

## Representative Papers

| Year | Title | Authors | Venue | Key Contribution |
|------|-------|---------|-------|-----------------|
| 2021 | A Finer-Grain Universal Dialogue Semantic Structures Based Model for Abstractive Dialogue Summarization | Lei, Y., Zheng, F., Yan, Y., He, K., & Xu, W. | EMNLP Findings | Universal dialogue semantic structure with ConceptNet |
| 2023 | Dialogue Summarization with Static-Dynamic Structure Fusion Graph | Gao, S., Cheng, X., Li, M., Chen, X., Li, J., Zhao, D., & Yan, R. | ACL | Static and dynamic graph integration for dialogue structure |
| 2023 | Improving Long Dialogue Summarization with Semantic Graph Representation | Hua, Y., Deng, Z., & McKeown, K. | ACL Findings | AMR graphs for thematic linking in dialogues |
| 2021 | Language Model as an Annotator: Exploring DialoGPT for Dialogue Summarization | Feng, X., Feng, X., Qin, L., Qin, B., & Liu, T. | ACL | Utilizing dialogue language models for structure annotation |
| 2022 | AMRTVSumm: AMR-augmented Hierarchical Network for TV Transcript Summarization | Hua, Y., Deng, Z., & Xu, Z. | Workshop on Automatic Summarization for Creative Writing | Abstract Meaning Representation for TV dialogue structure |
| 2022 | URAMDS: Utterances Relation Aware Model for Dialogue Summarization | Li, H. | BIOINC | Hybrid approach with graph neural networks for utterance dependency |
| 2023 | Attention Sorting Combats Recency Bias In Long Context Language Models | Peysakhovich, A., & Lerer, A. | arXiv | Addressing recency bias in processing long dialogues |
| 2021 | TANet: Thread-Aware Pretraining for Abstractive Conversational Summarization | Yang, Z., Wang, C., Tian, Z., Wu, W., & Li, Z. | NAACL Findings | Thread-aware pretraining for conversation structure |
| 2021 | SummˆN: A Multi-Stage Summarization Framework for Long Input Dialogues and Documents | Zhang, Y., et al. | ACL | Multi-stage approach for segmenting and summarizing long dialogues |
| 2019 | Sentence-BERT: Sentence Embeddings Using Siamese BERT-networks | Reimers, N., & Gurevych, I. | EMNLP | Embedding-based importance measures for dialogue segmentation |

## Primary Approach Categories

| Approach | Description | Key Papers |
|----------|-------------|------------|
| **Architecture modification** | Graph structures to capture dialogue dynamics | Li (2022), Lei et al. (2021), Gao et al. (2023), Hua et al. (2023) |
| **Pre-training** | Adaptations for handling long context | Lee et al. (2021), Peysakhovich & Lerer (2023), Xu et al. (2024) |
| **Training tasks** | Understanding dialogue structure | Feng et al. (2021), Liu et al. (2021), Yang et al. (2022) |
| **Importance measures** | Grouping sentences into sub-topics | Reimers & Gurevych (2019), Liang et al. (2023) |

## Related Datasets

| Dataset | Key Characteristics | Papers Using |
|---------|---------------------|--------------|
| MeetingBank | Parliament meetings with average 28k tokens per transcript | 7 papers |
| MediaSum | Media interview transcripts | 15 papers |
| AMI | Staged business meetings with topic-based phases | 63 papers |
| ICSI | Academic group meetings with complex structure | 21 papers |
