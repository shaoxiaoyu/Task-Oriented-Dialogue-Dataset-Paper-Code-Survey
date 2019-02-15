## Task-Oriented Dialogue Dataset Paper Code Survey

### Content
- ##### [Introduction](#intro)
- ##### [Call for Contribution](#call)
- ##### [Leader Boards](#leader)
- ##### [Datasets Introduction](#detail)
- ##### [Acknowledgement](#acknowledgement)


## <a name="intro"></a>Introduction
This repo is a dataset survey for Task-oriented Dialogue.

We investigated most existing dialogue datasets and summarize their basic information, such download link and size.

We also include leader boards of some dataset to present research progress in the task oriented dialogue fields.

A Chinese intro & news for this project is available [here](https://mp.weixin.qq.com/s?__biz=MzIxMjAzNDY5Mg==&mid=2650793618&idx=1&sn=dc5e592c5d8b451531383350af76e254&chksm=8f477379b830fa6fb0b5909f6d6a3f85dae44e8a37aa0ab9763df354cabcc9224c211075f127&mpshare=1&scene=1&srcid=#rd)

## <a name="call"></a> Call for Contributions
Contributions are welcomed, you are encouraged to:
- Directly pull request
- Send me new dataset info
- Send me new experiment results from published paper.

## <a name="leader"></a> Leader Boards

The ranking is depended on published results of related papers. We are trying to keep it up-to-date. The ranking may be unfair because features used and train/dev set splitting in those papers may be different. However it shows a trend of research, and would be helpful for someone to start a project about task-oriented dialogue.

### NLU: Slot Filling
Slot filling task aims to recognize key entity of user utterance, such position and time.

#### ATIS

| Model           | F1  |  Paper / Source | Code|
|-------------|-----|-----|-|
| Intent Gating & self-attention (Li et al., 2018) | 96.52 | [A Self-Attentive Model with Gate Mechanism for Spoken Language Understanding](http://aclweb.org/anthology/D18-1417) |[Self-Attentive-and-Gated-SLU](https://github.com/NinedayWang/Self-Attentive-and-Gated-SLU)|
| Atomic concept (Su Zhu and Kai Yu, 2018) | 96.08 | [Concept Transfer Learning for Adaptive Language Understanding](http://aclweb.org/anthology/W18-5047) |
| Atten.-Based (Liu and Lane, 2016) | 95.98 |  [Attention-based recurrent neural network models for joint intent detection and slot fillin](https://arxiv.org/pdf/1609.01454.pdf) |[rnn-nlu](https://github.com/HadoopIt/rnn-nlu) or [RNN-for-Joint-NLU](https://github.com/applenob/RNN-for-Joint-NLU) or [RNN-for-Joint-NLU](https://github.com/DSKSD/RNN-for-Joint-NLU)
| Encoder-decoder-pointer  (Zhai et al., 2017) | 95.86 |  [Neural Models for Sequence Chunking](https://arxiv.org/pdf/1701.04027.pdf) |**Related implementation** [neural_sequence_labeling](https://github.com/IsaacChanghau/neural_sequence_labeling)
| ELMo + BLSTM-CRF (Siddhant et al., 2018) | 95.62 |  [Unsupervised Transfer Learning for Spoken Language Understanding in Intelligent Agents](https://arxiv.org/pdf/1811.05370.pdf) |
| Capsule Neural Networks (Zhang et al., 2018) | 95.2 | [Joint Slot Filling and Intent Detection via Capsule Neural Networks](https://arxiv.org/pdf/1812.09471.pdf) |
| Slot-Gated (Intent Atten.) (Goo et al., 2018) | 95.2 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |
| Slot-Gated (Full Atten.) (Goo et al., 2018) | 94.8 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |


#### Snips


| Model           | F1  |  Paper / Source |
| ------------- | :-----:| :-----:|
| ELMo + BLSTM-CRF (Siddhant et al., 2018) | 93.90 |  [Unsupervised Transfer Learning for Spoken Language Understanding in Intelligent Agents](https://arxiv.org/pdf/1811.05370.pdf) |
| Capsule Neural Networks (Zhang et al., 2018) | 91.8 | [Joint Slot Filling and Intent Detection via Capsule Neural Networks](https://arxiv.org/pdf/1812.09471.pdf) |
| Slot-Gated (Full Atten.) (Goo et al., 2018) | 88.8 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |
| BLSTM-CRF (Siddhant et al., 2018) | 88.78 |  [Unsupervised Transfer Learning for Spoken Language Understanding in Intelligent Agents](https://arxiv.org/pdf/1811.05370.pdf) |
| Slot-Gated (Intent Atten.) (Goo et al., 2018) | 88.3 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |

### NLU: Intent Detection
Slot filling task aims to classify user utterance into different domain.

#### ATIS

| Model           | Acc.  |  Paper / Source |
| ------------- | :-----:| :-----:|
| Intent Gating & self-attention (Li et al., 2018) | 98.77 | [A Self-Attentive Model with Gate Mechanism for Spoken Language Understanding](http://aclweb.org/anthology/D18-1417) |
| Atten.-Based (Liu and Lane, 2016) | 98.43 |  [Attention-based recurrent neural network models for joint intent detection and slot filling](https://arxiv.org/pdf/1609.01454.pdf) |
| BLSTM (Zhang et al., 2016) | 98.10 | [A Joint Model of Intent Determination and Slot Filling for Spoken Language Understanding](https://www.ijcai.org/Proceedings/16/Papers/425.pdf) |
| Capsule Neural Networks (Zhang et al., 2018) | 95.0 | [Joint Slot Filling and Intent Detection via Capsule Neural Networks](https://arxiv.org/pdf/1812.09471.pdf) |
| Slot-Gated (Intent Atten.) (Goo et al., 2018) | 94.1 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |
| Slot-Gated (Full Atten.) (Goo et al., 2018) | 93.6 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |


#### Snips

| Model           | Acc.  |  Paper / Source |
| ------------- | :-----:| :-----:|
| Capsule Neural Networks (Zhang et al., 2018) | 97.7 | [Joint Slot Filling and Intent Detection via Capsule Neural Networks](https://arxiv.org/pdf/1812.09471.pdf) |
| Slot-Gated (Full Atten.) (Goo et al., 2018) | 97.0 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |
| Slot-Gated (Intent Atten.) (Goo et al., 2018) | 96.8 | [Slot-Gated Modeling for Joint Slot Filling and Intent Prediction](http://www.aclweb.org/anthology/N18-2118) |
