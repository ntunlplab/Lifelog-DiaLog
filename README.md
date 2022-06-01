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

# Dataset
First click [here](https://www.aclweb.org/anthology/I17-1099/) to download the original dataset, DailyDialog, then download ```DiaLog_v1.zip``` for the DiaLog dataset.

The file ```preprocess.py``` in the zip file is an example to format ```DiaLog.json``` into ```train.csv``` and ```test.csv```.</br>
Run ```python3 preprocess.py [DailyDialog_Dir]``` to generate the two files.

# How to Cite the Corpus
Please cite the following papers when referring to the DiaLog in academic publications and papers.

Pei-Wei Kao, An-Zi Yen, Hen-Hsen Huang, and Hsin-Hsi Chen. 2021. ConvLogMiner: A Real-Time Conversational Lifelog Miner. In Proceedings of the 30th International Joint Conference on Artificial Intelligence.
