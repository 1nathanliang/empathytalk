# The EmpathyTalk Project 💖 💬

## Introduction

> *How does priming interlocutors to think and behave empathically toward others influence the quality of naturalistic conversation?*

During the pandemic, ~50 speaker dyads engaged in ~20-minute long conversations and were provided the option of relying on various prewritten prompts to guide the direction of their chat. Both cameras and microphones were on for the duration of each video call over Zoom allowing for recording of both video and audio data. The speech extracted from the latter was manually transcribed by professional transcriptionists and stored in text files. Participants were randomly assigned to either an empathy or control condition, and the former involved a pre-experiment intervention consisting of a reading task emphasizing the malleability and importance of empathy in interpersonal relationships. Participants from dyads in the empathy condition were aware of each others' belonging in the same condition, and they were encouraged to incorporate the information gleaned from their reading tasks into their chat.


## Method
We aimed to answer our main research question algorithmically and computationally by adopting a convergent three-pronged approach to analyzing this pilot dataset:

1. NLP 📝
2. Computer Vision 👁️‍🗨️ 
3. Audio Signal Processing 🔉

A host of interrelated methods were implemented in Python and R to analyze the transcribed speech:

### NLP: Using natural language processing to analyze the semantic differences catalyzed by empathy
> *Does priming empathy cause speakers to...*
* ...linguistically mirror each other *affectively*?
  * Sentiment analysis (`transformers`, Microsoft Azure Cognitive Services, AFINN, LIWC, SEANCE)
* ...linguistically mirror each other *semantically*?
  * Semantic similarity (`tensorflow`: universal sentence encoder)
* ...self-disclose more frequently?
  * First-person pronoun counts (`spacy`)
* ...speak more *freely*?
  * Profanity detection (`profanity-check`)

### Computer vision: Using facial detection software to identify the visual effects of empathy on self-presentation
> *Does priming empathy cause speakers to...*
* ...visually mirror each other's body language *affectively*?
  * Facial emotion detection (`cv2`, Microsoft Azure Face Detect API)

### Audio signal processing: Assesing the effect of empathy on the acoustic profile of conversations
> *Does priming empathy cause speakers to...*
* ...acoustically mirror each other's pitch and volumne more strongly? (`pydub`, `scipy`)
