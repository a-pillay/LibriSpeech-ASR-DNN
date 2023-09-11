# LibriSpeech Automatic Speech Recognition Experiments

These experiments focus on various Speech Classification/Recognition tasks utilizing the [LibriSpeech Dataset](https://www.openslr.org/12).

I completed this work as part of my coursework for Carnegie Mellon University's [11-785: Introduction to Deep Learning (Spring 2023)](https://deeplearning.cs.cmu.edu/S23/index.html) course.

Here's a high-level overview of the tasks:

- **FrameLevelSpeechClassification**: Prediction of phonemes in incoming speech frames using **only** Fully-Connected layers. We leverage inter-frame context to enhance recognition robustness.

- **Utterance2PhonemeMapping**: Predicting phonemes in incoming speech, regardless of their duration. The architecture incorporates [Pyramidal Bi-LSTMs](https://arxiv.org/abs/1508.01211), followed by Connectionist Temporal Classifier (CTC) based decoding and Beam Search for determining the final sequence.

- **AttentionBasedSpeech2Text**: Building upon the Utterance2PhonemeMapping work by incorporating an `encoder-decoder+attention` architecture for converting incoming speech into written text.

For detailed documentation synchronized with the code blocks, please refer to the notebooks in the respective directories.

## Special Note for CMU 11-785 Students

During your time as an 11-785 student, the MIT license **does not** apply to you! 

Using or referring to this repository for your coursework submissions is prohibited. Instead, kindly seek assistance from the teaching staff or your study group. My sincere apologies for any inconvenience!
