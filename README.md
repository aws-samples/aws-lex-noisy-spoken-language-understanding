## Lex datasets for noisy spoken language understanding 

This repository contains dataset for evaluating spoken language understanding system with audio input. The utterances, intent and slot labeling in the dataset comes from SNIPS dataset published by the Snips team:
-  [Coucke A. et al., "Snips Voice Platform: an embedded Spoken Language Understanding system for private-by-design voice interfaces." 2018](https://arxiv.org/abs/1805.10190)
- [github repo](https://github.com/sonos/nlu-benchmark)


Here we extend the natural language understanding (NLU) dataset with audio by synthesizing the utterance with different voices provided by [Amazon Polly](https://aws.amazon.com/polly/). More information about the voices can be found [here](https://docs.aws.amazon.com/polly/latest/dg/voicelist.html).

## Dataset
### Audio
Due to the size of the dataset, we provide the audio as a [zip file](data/audio_slu.zip). After unzipping the file, you will see a folder with following structure

```
audio_slu/
│
├── audio_$voice_id_1/
│   └── snips
│       ├── $utterance_id_1.mp3
│       ├── $utterance_id_2.mp3
│       ├── ...
│ 
├── audio_$voice_id_2/
│   └── snips
│       ├── $utterance_id_1.mp3
│       ├── $utterance_id_2.mp3
│       ├── ...
│
├── ...
```

voice_id is the Amazon polly voice used to synthesize the audio as listed in the [doc](https://docs.aws.amazon.com/polly/latest/dg/voicelist.html). 
utterance_id is the utterance id can be used to relate the audio with its transcript and NLU annotation.

### NLU annotation

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

See the [LICENSE](LICENSE) file for more information.
