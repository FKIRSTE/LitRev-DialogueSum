# Dialogue Summarization Datasets

This page provides a comprehensive overview of datasets used in dialogue summarization research, organized by subdomain.

## Overview of Key Datasets

| Subdomain | Dataset | Primary Challenge | Key Characteristics | Usage Count |
|-----------|---------|-------------------|---------------------|-------------|
| **Daily Chat** | DialogSum | Speaker | 13k dialogues, ~1k tokens input, ~130 tokens summary | 26 |
| **Online Chat** | SAMSum | Speaker, Salience | 16k dialogues, 2-3 speakers, ~94 tokens per conversation | 68 |
| | FORUM | Salience | 100 discussion threads from online forums | 5 |
| | CRD3 | Language | 159 episodes, ~2550 turns per dialogue | 6 |
| **Meeting** | AMI | Salience, Comprehension | 137 business meetings, ~6k tokens, 535 turns, 4 speakers | 63 |
| | ICSI | Salience, Language | 59 academic meetings, ~13k tokens, 819 turns, 6 speakers | 21 |
| | QMSum | Salience, Language | 232 meetings, 1.8k query-summary pairs | 18 |
| | Elitr | Salience | 120 technical project meetings, ~7k words | 7 |
| | MeetingBank | Structure | 1366 city council meetings, ~28k tokens per transcript | 7 |
| **Screenplay** | MediaSum | Structure | 463.6k media interview transcripts | 15 |
| | SummScreen | Speaker, Salience | 27k TV series transcripts, ~6.6k tokens | 8 |
| **Customer Service** | TweetSumm | Language | 1.1k Twitter customer support exchanges | 7 |
| | TODSum | Language, Factuality | 10k task-oriented dialogues | 6 |
| **Medical** | MTS-Dialog | Comprehension | 1.7k doctor-patient conversations | 5 |
| **Debates** | ADSC | Comprehension | 45 two-party dialogues on social/political topics | 5 |
| **Others** | ConvoSumm | Salience | 2k dialogues from various sources | 5 |
| | Ferranti | Factuality | 4k items for factual error correction | 5 |
| | DialSum | Comprehension | Two-party discussion on images | 10 |

## Daily Chat

### DialogSum
- **Size**: 13,000 dialogues
- **Source**: DailyDialog, Dream, Mutual, and English-speaking practice websites
- **Characteristics**: Two-speaker interactions across daily-life scenarios (work, leisure, travel)
- **Input Length**: ~1,000 tokens
- **Summary Length**: ~130 tokens
- **Annotation**: Human annotators with guidelines (summaries no longer than 20% of conversation)
- **Primary Challenge**: Speaker
- **Key Papers**: Chen et al. (2021)

## Online Chat

### SAMSum
- **Size**: 16,000 dialogues
- **Source**: Written online dialogues created by linguists to reflect real-life messenger conversations
- **Characteristics**: Mostly two-speaker conversations with 3-30 turns
- **Input Length**: ~94 tokens per conversation
- **Summary Length**: ~20 tokens
- **Topics**: Chit-chats, gossip, meeting arrangements, politics, university assignments
- **Primary Challenge**: Speaker, Salience
- **Key Papers**: Gliwa et al. (2019), Bertsch et al. (2022)

### FORUM
- **Size**: 100 threads (556 Ubuntu posts, 916 TripAdvisor posts)
- **Source**: Online discussion forums
- **Characteristics**: Multi-participant discussions with thread structure
- **Annotation**: Two human evaluators per sample
- **Primary Challenge**: Salience
- **Key Papers**: Bhatia et al. (2014)

### CRD3
- **Size**: 159 episodes
- **Source**: "Critical Role Dungeon and Dragon" show
- **Characteristics**: Long dialogues with an average of 2,550 turns
- **Summaries**: Collected from Fandom wiki
- **Primary Challenge**: Language
- **Key Papers**: Rameshkumar & Bailey (2020)

## Meeting

### AMI
- **Size**: 137 meetings
- **Source**: Staged business meetings on product design process
- **Characteristics**: 4 participants (project manager, marketing expert, UI designer, industrial designer)
- **Input Length**: ~6,000 tokens, 535 turns
- **Annotation**: Human summaries
- **Variants**: AMI-ITS (incremental temporal summaries for 100-second segments)
- **Primary Challenge**: Salience, Comprehension
- **Key Papers**: Carletta et al. (2006), Manuvinakurike et al. (2021)

### ICSI
- **Size**: 59 meetings
- **Source**: Academic group meetings at ICSI Berkeley
- **Characteristics**: ~13,000 tokens, 819 turns, 6 speakers
- **Content**: Research discussions among students, computer scientists, linguists, engineers
- **Primary Challenge**: Salience, Language
- **Key Papers**: Janin et al. (2003)

### QMSum
- **Size**: 232 meetings (1,800 query-summary pairs)
- **Source**: Combined from AMI, ICSI, and committee meetings
- **Characteristics**: Query-based summarization, up to 13,000 tokens and 6 speakers
- **Task**: Summarize meeting based on a specific question
- **Variants**: MACSum-Dial (for controllable summarization)
- **Primary Challenge**: Salience, Language
- **Key Papers**: Zhong et al. (2021), Zhang et al. (2023)

### Elitr
- **Size**: 120 meetings
- **Source**: English technical project meetings in computer science
- **Characteristics**: ~7,000 words, 730 turns, 6 speakers, duration 10 minutes to 2+ hours
- **Task**: Producing meeting minutes in bullet points
- **Primary Challenge**: Salience
- **Key Papers**: Nedoluzhko et al. (2022)

### MeetingBank
- **Size**: 1,366 meetings (3,600+ hours)
- **Source**: City council meetings from six major U.S. cities
- **Characteristics**: 2.6 hours average duration, ~28,000 tokens per transcript
- **Primary Challenge**: Structure
- **Key Papers**: Hu et al. (2023)

## Screenplay

### MediaSum
- **Size**: 463,600 transcripts
- **Source**: National Public Radio and CNN interviews
- **Characteristics**: 1,500 words per transcript, ~11 words per summary, 7 speakers average
- **Topics**: Politics, news, crime, economy
- **Primary Challenge**: Structure
- **Key Papers**: Zhu et al. (2021), Majumder et al. (2020)

### SummScreen
- **Size**: 27,000 instances
- **Source**: TV series transcripts with human-written recaps from TV MegaSite and ForeverDreaming
- **Characteristics**: 28 speakers average, 6,600 tokens per transcript, 380 tokens per summary
- **Primary Challenge**: Speaker, Salience
- **Key Papers**: Chen et al. (2022)

## Data Augmentation Techniques

| Technique | Description | Key Papers |
|-----------|-------------|------------|
| **Weak labeling** | Selecting leading or longest utterance as proxy summary | Sznajder et al. (2022) |
| **Paraphrasing** | Modifying existing dialogues while maintaining coherence | Liu et al. (2022), Wahle et al. (2022, 2023) |
| **Structure alteration** | Random modifications to conversation structures | Chen & Yang (2021), Park et al. (2022) |
| **LLM generation** | Using language models to create ground truth summaries | Asi et al. (2022), Nair et al. (2023), Zhou et al. (2023) |

## Dataset Utility Maximization Techniques

| Technique | Description | Key Papers |
|-----------|-------------|------------|
| **Curriculum learning** | Gradually increasing prompt perturbation difficulty | Li et al. (2022) |
| **Dynamic prompts** | Selecting best-fitting few-shot samples based on content | Prodan & Pelican (2022) |
| **Domain transfer** | Transferring prompts from related dialogue domains | Xie et al. (2023) |
| **Parameter freezing** | Training only specific parameters for domain adaptation | Chen et al. (2023), Suri et al. (2023), Zhu et al. (2023) |
