# The EmpathyTalk Project 💬

> *How does priming interlocutors to think and behave empathically toward others influence the quality of naturalistic conversation?*

We aimed to answer this question algorithmically and computationally by adopting three convergent approaches on one dataset:

1. NLP 📝
2. Computer Vision 👁️‍🗨️ 
3. Audio Signal Processing 🔉

~50 speaker dyads engaged in ~20-minute long conversations and were provided the option of relying on various prewritten prompts to guide the direction of their chat. Both cameras and microphones were on for the duration of each video call over Zoom allowing for recording of both video and audio data. The speech extracted from the latter was manually transcribed by professional transcriptionists and stored in text files. Participants were randomly assigned to either an empathy or control condition, and the former involved a pre-experiment intervention consisting of a reading task emphasizing the malleability and importance of empathy in interpersonal relationships. Specifically, participants from dyads in the empathy condition were aware of each others' belonging in the same condition, and they were encouraged to incorporate the information gleaned from their reading tasks into their chat.

## NLP: Using natural language processing to analyze the linguistic differences catalyzed by empathy
A host of NLP methods were applied through Python to analyze the transcribed speech:
* Sentiment analysis (distilBERT, Microsoft Azure Cognitive Services, LIWC, SEANCE)
* Subject similarity

## Computer Vision: Raw .mp4 data was filtered to extract facial expression and body language differences attributed to empathy
* Emotional detection in facial expression (OpenCV, Microsoft Azure Face Detect)

## Audio Signal Processing: Raw .mp3 data was cleaned and processed to compare average volume and pitch between the two conditions
