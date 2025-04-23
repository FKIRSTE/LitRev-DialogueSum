# Speaker Challenge

The speaker challenge addresses tracking participants, their roles, interactions, and references to entities and other participants, including role changes across topics.

## Sub-challenges
- Individual participant roles (e.g., 'project manager', 'customer service agent')
- Topic-dependent role changes
- Participant interactions and contributions
- References to entities and other participants

## Progress
**Status**: 🟠 Good progress through special attention mechanisms and graph-based models

## Representative Papers

| Year | Title | Authors | Venue | Key Contribution |
|------|-------|---------|-------|-----------------|
| 2021 | Hierarchical Speaker-Aware Sequence-to-Sequence Model for Dialogue Summarization | Lei, Y., Yan, Y., Zeng, Z., He, K., Zhang, X., & Xu, W. | ICASSP | Speaker-aware attention mechanism |
| 2022 | Entity-Based De-Noising Modeling for Controllable Dialogue Summarization | Liu, Z., & Chen, N. | SIGDIAL | Entity-based noise reduction for dialogue |
| 2021 | Capturing Speaker Incorrectness: Speaker-focused Post-Correction for Abstractive Dialogue Summarization | Lee, D., Lim, J., Whang, T., Lee, C., Cho, S., Park, M., & Lim, H. | Workshop on New Frontiers in Summarization | Post-correction for speaker attribution |
| 2021 | Coreference-Aware Dialogue Summarization | Liu, Z., Shi, K., & Chen, N. | SIGDIAL | Explicit coreference resolution for dialogues |
| 2022 | Evaluating the Effects of Embedding with Speaker Identity Information in Dialogue Summarization | Naraki, Y., Sakai, T., & Hayashi, Y. | LREC | Speaker identity embedding methods |
| 2022 | From Spoken Dialogue to Formal Summary: An Utterance Rewriting for Dialogue Summarization | Fang, Y., Zhang, H., Chen, H., Ding, Z., Long, B., Lan, Y., & Zhou, Y. | NAACL | Utterance rewriting approach for speaker normalization |
| 2022 | Improving Abstractive Dialogue Summarization with Speaker-Aware Supervised Contrastive Learning | Geng, Z., Zhong, M., Yin, Z., Qiu, X., & Huang, X. | COLING | Contrastive learning for speaker differentiation |
| 2021 | Improving Abstractive Dialogue Summarization with Hierarchical Pretraining and Topic Segment | Qi, M., Liu, H., Fu, Y., & Liu, T. | EMNLP Findings | Hierarchical pretraining for speaker turns |
| 2022 | WHORU: Improving Abstractive Dialogue Summarization with Personal Pronoun Resolution | Zhou, T. | Electronics | Pronoun resolution for speaker identification |
| 2020 | SpanBERT: Improving Pre-Training by Representing and Predicting Spans | Joshi, M., Chen, D., Liu, Y., Weld, D. S., Zettlemoyer, L., & Levy, O. | TACL | Span-based pretraining for entity representation |

## Primary Approach Categories

| Approach | Description | Key Papers |
|----------|-------------|------------|
| **Training tasks** | Tasks to help models understand speaker roles and dynamics | Gan et al. (2021), Qi et al. (2021), Naraki et al. (2022) |
| **Architecture modification** | Graph-based models for speaker structures and interactions | Lei et al. (2021), Liu et al. (2021), Hua et al. (2022) |
| **Pre-processing** | Techniques to enhance speaker representation | Joshi et al. (2020), Lee et al. (2021) |
| **Post-processing** | Methods to improve pronoun resolution and correct errors | Fang et al. (2022), Liu & Chen (2022) |

## Related Datasets

| Dataset | Key Characteristics | Papers Using |
|---------|---------------------|--------------|
| DialogSum | Two-speaker interactions across daily-life scenarios | 26 papers |
| SAMSum | Messaging app dialogues with clearly identified speakers | 68 papers |
| SummScreen | TV series transcripts with multiple speakers (avg. 28) | 8 papers |
| AMI | Business meetings with defined participant roles | 63 papers |
