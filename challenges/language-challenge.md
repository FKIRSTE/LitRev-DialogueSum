# Language Challenge

The language challenge addresses the idiosyncratic nature of spoken language and individual speech patterns, including informal expressions, ungrammatical structures, colloquialisms, and domain-specific terminology.

## Sub-challenges
- Linguistic noise (e.g., filler words, disfluencies)
- Content repetition (speakers restating or rephrasing information)
- Domain-specific terminology (e.g., medical jargon)

## Progress
**Status**: 🟠 Good progress through pre-training and additional training tasks

## Representative Papers

| Year | Title | Authors | Venue | Key Contribution |
|------|-------|---------|-------|-----------------|
| 2021 | A Bag of Tricks for Dialogue Summarization | Khalifa, M., Ballesteros, M., & McKeown, K. | EMNLP | Training tasks for dialogue-specific features including masking key elements |
| 2021 | Low-Resource Dialogue Summarization with Domain-Agnostic Multi-Source Pretraining | Zou, Y., Zhu, B., Hu, X., Gui, T., & Zhang, Q. | EMNLP | Domain adaptation techniques for dialogue summarization |
| 2022 | He Said, She Said: Style Transfer for Shifting the Perspective of Dialogues | Bertsch, A., Neubig, G., & Gormley, M. R. | EMNLP Findings | Style transformation from informal first-person to structured third-person |
| 2022 | Post-Training Dialogue Summarization Using Pseudo-Paraphrasing | Jia, Q., Liu, Y., Tang, H., & Zhu, K. | NAACL Findings | Paraphrasing techniques for style transfer |
| 2020 | A Hierarchical Network for Abstractive Meeting Summarization with Cross-Domain Pretraining | Zhu, C., Xu, R., Zeng, M., & Huang, X. | EMNLP Findings | Dialogue structure simulation through document modification |
| 2019 | Restructuring Conversations Using Discourse Relations for Zero-shot Abstractive Dialogue Summarization | Ganesh, P., & Dingliwal, S. | arXiv | Anaphora resolution pre-processing technique |
| 2024 | Automatic Summarization of Doctor-Patient Encounter Dialogues Using Large Language Model through Prompt Tuning | Lyu, M., Peng, C., Li, X., Balian, P., Bian, J., & Wu, Y. | arXiv | Adapting LLMs to medical dialogue summarization |
| 2023 | Multi-Stage Pre-training Enhanced by ChatGPT for Multi-Scenario Dialogue Summarization | Zhou, W., Li, G., Cheng, X., Liang, X., Zhu, J., Zhai, F., & Li, Z. | EMNLP Findings | LLM integration for pre-training in dialogue summarization |
| 2021 | Who Speaks Like a Style of Vitamin: Towards Syntax-Aware Dialogue Summarization Using Multi-Task Learning | Lee, S., Yang, K., Park, C., Sedoc, J., & Lim, H. | IEEE Access | Part-of-speech tagging for syntax-aware summarization |
| 2020 | How Domain Terminology Affects Meeting Summarization Performance | Koay, J. J., Roustai, A., Dai, X., Burns, D., Kerrigan, A., & Liu, F. | COLING | Handling domain-specific terminology in meeting summarization |

## Primary Approach Categories

| Approach | Description | Key Papers |
|----------|-------------|------------|
| **Pre-training** | Adapting models to dialogue-specific language patterns | Raffel et al. (2020), Zou et al. (2021), Zhou et al. (2023) |
| **Training tasks** | Tasks like masking key dialogue elements, POS-tagging | Zhu et al. (2020), Khalifa et al. (2021), Bertsch et al. (2022) |
| **Pre-processing** | Techniques like anaphora resolution | Ganesh and Dingliwal (2019) |

## Related Datasets

| Dataset | Key Characteristics | Papers Using |
|---------|---------------------|--------------|
| SAMSum | Written online dialogues from messaging apps | 68 papers |
| DialogSum | Two-speaker interactions across daily-life scenarios | 26 papers |
| CRD3 | Live-streamed show dialogue with an average of 2550 turns | 6 papers |
| TweetSumm | Twitter customer support exchanges | 7 papers |
| TODSum | Task-oriented dialogues | 6 papers |
