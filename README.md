# DiaLog: A Lifelog Dataset for Life Event Detection from Daily Dialog


# Introduction
Conversation, a common way for people to share their experiences and feelings with others, consists of important information about personal life events of individuals, but is rarely explored. In this dataset, we initiate a task of detecting personal life events from daily conversaion. We extend a multi-turn dialog dataset, DailyDialog, with life event annotation. We collect 600 conversations with 4-6 utterances from 4 topics of DailyDialog. Our goal is to detect the life events of each speaker in real-time.

# Format
Each entry in the JSON format is consisted of "dialog_id" (the id of the dialog from DailyDialog), "turns" (the total turns of the dialog), and "events" (annotated result).

"events" is consist of the real-time life events of each speaker. "S1" and "S2" in "events" represent the two speakers in the conversation and the life event is according to FrameNet ontology.

# Example

```yaml
{
    "dialog_id": 6,
    "turns": 4,
    "events": [
        {
            "S1": [],
            "S2": []
        },
        {
            "S1": [],
            "S2": ["Perception_experience", "Request"]
        },
        {
            "S1": [],
            "S2": []
        },
        {
            "S1": [],
            "S2": []
        }
    ]
}
```

# Download
Please go to [resources page](http://nlg.csie.ntu.edu.tw/nlpresource/DiaLog/) to access resources.

# How to Cite the Corpus
Please cite the following papers when referring to the DiaLog in academic publications and papers.

Pei-Wei Kao, An-Zi Yen, Hen-Hsen Huang, and Hsin-Hsi Chen. 2021. ConvLogMiner: A Real-Time Conversational Lifelog Miner. In Proceedings of the 30th International Joint Conference on Artificial Intelligence.
