# VibeVoice---Understanding-Emotions-from-Vocal-Cues
🔗 🌐 **Open Project in Your Browser**: https://arrao10.github.io/VibeVoice---Understanding-Emotions-from-Vocal-Cues/


### 📖 **Introduction**:
Speech conveys more than just words - it carries **Emotion**, which is essential for human communication and interaction. The project focuses on **Speech Emotion Recognition (SER)** using the **Toronto Emotional Speech Set (TESS)** dataset. I have developed and evaluated a **BiLSTM + Attention** deep learning architecture to classify audio samples into **7 distinct emotions**: **Angry**, **Disgust**, **Fear**, **Happy**, **Neutral**, **Pleasant Surprise**, and **Sad**.

### 🎯 **Problem Statement**: 
The aim is to create a robust and generalizable model capable of recognizing emotions in real-world audio scenarios.

### 📂 **Dataset Details**:
* **Name**: Toronto Emotional Speech Set (TESS)  
* **Link**: https://www.kaggle.com/datasets/ejlok1/toronto-emotional-speech-set-tess
* **Number of Emotion Classes**: **7** classes:
    - **Angry**
    - **Disgust**
    - **Fear**
    - **Happy**
    - **Neutral**
    - **Pleasant Surprise**
    - **Sad**
* **Speakers**:  
    - **OAF** → **Older Adult Female**  
    - **YAF** → **Younger Adult Female** 
* **Utterances**: **200** target words, each spoken in all emotions by both speakers.
* **Format**: **.wav** audio files.
* **Sampling Rate Used**: Resampled to **16 kHz** for uniformity.

### ⚖️ **Balanced Word-Level Cross-Speaker Split**:
A **word-level intersection split** is used to ensure that for each emotion, the same set of words exists in both **OAF** and **YAF** speakers. This prevents **data leakage** (same word in both train and test spoken by different speakers) and improves **generalization**.

**Advantages of Word-Level Split**:
- Avoids speaker and lexical bias in the test set.
- Ensures fair model evaluation on unseen speaker-word combinations.
- Improves real-world performance for unseen vocabulary and voices.
