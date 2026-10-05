# 🎵 AI-Based Mood-Based Music Recommendation Chatbot

## Using Text and Speech Analysis with NLP

An intelligent **Mood-Based Music Recommendation Chatbot** developed using **Python, Natural Language Processing (NLP), Speech-to-Text, and Gradio**.

The system analyzes the user's **text or voice**, identifies their approximate emotional mood, and recommends suitable music based on the detected mood.

The complete project is designed to run directly in **Google Colab** and generates a temporary **public Gradio URL (`gradio.live`)** after execution.

---

## 📌 Project Title

**AI-Based Mood-Based Music Recommendation Chatbot using Text and Speech Analysis**

---

## 🎯 Objective

The main objective of this project is to develop an interactive chatbot that can:

* Analyze user text
* Accept voice input
* Convert speech into text
* Detect the user's mood using NLP
* Classify the detected mood
* Recommend suitable music
* Display a confidence score
* Maintain conversation history
* Generate a final mood analysis report

---

## ✨ Features

### 💬 1. Text-Based Chatbot

Users can type how they are feeling.

Example:

> I am very stressed because I have an exam tomorrow.

The chatbot analyzes the sentence and detects the likely mood.

---

### 🎙️ 2. Voice Analysis

Users can record their voice using the microphone.

The system performs:

```text
Voice Input
     ↓
Speech-to-Text
     ↓
Text Analysis
     ↓
Mood Detection
```

---

### 🗣️ 3. Speech-to-Text

The project uses **Faster-Whisper** to convert the user's voice into text.

Example:

```text
Voice:
"I am feeling very tired today."

↓

Text:
"I am feeling very tired today."
```

---

### 🧠 4. NLP-Based Mood Detection

The chatbot uses Natural Language Processing techniques to identify emotional keywords and classify the user's mood.

Supported moods include:

* 😊 Happy
* 😢 Sad
* 😡 Angry
* 😰 Stressed
* 😌 Relaxed
* ⚡ Energetic
* ❤️ Romantic
* 😴 Tired
* 🙂 Neutral

---

### 🎧 5. Music Recommendation

After detecting the mood, the system recommends suitable:

* Songs
* Music genres
* Listening suggestions

Example:

```text
Mood: Stressed

Recommended Genres:
• Lo-fi
• Ambient
• Soft Piano

Recommended Songs:
• Weightless
• River Flows in You
• Sunset Lover
```

---

### 📊 6. Confidence Score

The chatbot provides an approximate confidence percentage for the detected mood.

Example:

```text
Detected Mood: Stressed
Confidence: 91%
```

---

### 📈 7. Mood History

The system maintains the user's recent interactions during the current session.

It displays:

* User message
* Detected mood
* Confidence score

---

### 📋 8. Final Mood Report

The application can generate a final report containing:

* Total interactions
* Most detected mood
* Mood distribution
* Recent mood analysis
* Confidence values

---

## 🛠️ Technologies Used

| Technology          | Purpose                            |
| ------------------- | ---------------------------------- |
| Python              | Main programming language          |
| NLP                 | Text and mood analysis             |
| Faster-Whisper      | Speech-to-text                     |
| Gradio              | Web interface                      |
| Google Colab        | Development and execution platform |
| Regular Expressions | Text preprocessing                 |

---

## 🧠 NLP Concepts Used

This project demonstrates several Text and Speech Analysis concepts:

1. Text preprocessing
2. Text normalization
3. Keyword extraction
4. Keyword matching
5. Emotion detection
6. Mood classification
7. Speech-to-text
8. Chatbot processing
9. Recommendation system
10. Confidence scoring
11. Conversation history
12. Report generation

---

## 🔄 System Workflow

```text
             USER
               |
        ----------------
        |              |
     TEXT INPUT     VOICE INPUT
        |              |
        |        Speech-to-Text
        |              |
        -------> TEXT <-------
                 |
          Text Preprocessing
                 |
          NLP Mood Analysis
                 |
          Keyword Detection
                 |
          Mood Classification
                 |
        ---------------------
        |                   |
   Confidence Score    Mood Detection
        |                   |
        -------+------------
               |
       Music Recommendation
               |
        Chatbot Response
               |
        Conversation History
               |
        Final Mood Report
```

---

# 🚀 How to Run the Project

## Step 1 — Open Google Colab

Open Google Colab and create a new Python notebook.

---

## Step 2 — Copy the Code

Copy the complete project code into **one single Colab cell**.

---

## Step 3 — Run the Cell

Click:

```text
Runtime → Run all
```

or click the ▶ button.

---

## Step 4 — Wait for Installation

The notebook automatically installs:

```text
Gradio
Faster-Whisper
```

The speech recognition model will also be loaded.

The first execution may take some time.

---

## Step 5 — Get the Public URL

At the end of execution, Gradio generates a temporary public URL.

Example:

```text
Running on public URL:
https://abc123.gradio.live
```

Click the URL to open the chatbot.

---

# 🌐 Public URL

The project uses:

```python
app.launch(
    share=True,
    debug=True
)
```

Therefore, Google Colab generates a temporary public URL similar to:

```text
https://xxxxxxxx.gradio.live
```

The URL remains available while the Colab runtime and Gradio application are running.

---

# 💬 Example Inputs

## 😊 Happy

```text
I am very happy today because I completed my project successfully.
```

Expected result:

```text
Mood: Happy
```

---

## 😰 Stressed

```text
I am very stressed because I have an exam tomorrow and I cannot focus.
```

Expected result:

```text
Mood: Stressed
```

Recommended music:

```text
Lo-fi
Ambient
Soft Piano
```

---

## 😢 Sad

```text
I feel lonely and upset today.
```

Expected result:

```text
Mood: Sad
```

---

## ⚡ Energetic

```text
I feel very energetic and motivated to work out today.
```

Expected result:

```text
Mood: Energetic
```

---

## 😴 Tired

```text
I am exhausted after a long day and I need some rest.
```

Expected result:

```text
Mood: Tired
```

---

## ❤️ Romantic

```text
I am thinking about someone I love and feeling romantic today.
```

Expected result:

```text
Mood: Romantic
```

---

# 🎙️ Voice Input Example

Speak:

```text
I am feeling stressed because I have a lot of assignments.
```

The system performs:

```text
Voice
 ↓
Faster-Whisper
 ↓
"I am feeling stressed because I have a lot of assignments."
 ↓
NLP Analysis
 ↓
Stressed
 ↓
Lo-fi / Ambient / Soft Piano
```

---

# 📊 Final Report

The **Final Report** tab provides a summary such as:

```text
Total Interactions: 5

Most Detected Mood:
Stressed

Mood Distribution:

Stressed    40%
Happy       20%
Tired       20%
Relaxed     20%
```

---

# 🖥️ Application Interface

The application contains three major sections:

### 1. 💬 Text Chat

Used for entering text and detecting mood.

### 2. 🎙️ Voice Analysis

Used for recording voice and performing speech-to-text analysis.

### 3. 📊 Final Report

Used to generate the mood history report.

---

# 📁 Project Structure

```text
Mood-Based-Music-Recommendation-Chatbot/
│
├── Mood_Based_Music_Recommendation_Chatbot.ipynb
│
├── README.md
│
└── PROJECT_DETAILS.txt
```

The main notebook contains the complete application in a single code cell.

---

# 🔬 Working Principle

The chatbot follows these steps:

### Step 1 — Input

The user provides either text or voice.

### Step 2 — Speech Processing

If voice is provided, Faster-Whisper converts the speech into text.

### Step 3 — Preprocessing

The text is converted to lowercase and unnecessary characters are removed.

### Step 4 — Keyword Analysis

The system searches for mood-related keywords.

### Step 5 — Mood Classification

The mood with the highest matching score is selected.

### Step 6 — Recommendation

Music genres and songs associated with the detected mood are displayed.

### Step 7 — Response

The chatbot provides a personalized response.

### Step 8 — History

The interaction is stored temporarily for the final report.

---

# 🎓 TSA Relevance

This project is suitable for a **Text and Speech Analysis (TSA)** academic project because it combines both text and speech processing.

### Text Analysis

```text
User Text
   ↓
Preprocessing
   ↓
Keyword Analysis
   ↓
Mood Detection
```

### Speech Analysis

```text
User Voice
   ↓
Speech-to-Text
   ↓
Text Processing
   ↓
Mood Detection
```

---

# 📌 Advantages

* Easy to use
* Interactive chatbot
* Supports text and voice
* No Firebase required
* No database required
* No Node.js required
* No npm required
* Runs directly in Google Colab
* Provides a public URL
* Demonstrates NLP concepts
* Suitable for college project demonstration

---

# ⚠️ Limitations

* Mood detection is based mainly on text keywords.
* It may not correctly understand sarcasm or complex emotions.
* Music recommendations are from a predefined collection.
* The Gradio URL is temporary.
* The application requires the Colab runtime to remain active.
* Voice recognition accuracy can vary depending on audio quality.

---

# 🔮 Future Enhancements

The project can be improved by adding:

* Spotify API integration
* YouTube Music integration
* Advanced transformer-based emotion detection
* Multilingual support
* Tamil + English mixed-language analysis
* Real-time voice emotion recognition
* User login
* Personalized music history
* Database storage
* Machine-learning-based recommendation
* Emotion charts
* Daily mood tracking
* Playlist generation

---

# 🎯 Future Version

A future version can follow this architecture:

```text
User
 ↓
Voice / Text
 ↓
Speech & NLP Processing
 ↓
Advanced Emotion Model
 ↓
Personalized Recommendation Engine
 ↓
Spotify / YouTube API
 ↓
Personalized Playlist
```

---

# 🧪 Testing

The chatbot can be tested using different emotional sentences.

| Input                         | Expected Mood |
| ----------------------------- | ------------- |
| I am very happy today         | Happy         |
| I feel lonely                 | Sad           |
| I am extremely angry          | Angry         |
| I have too much exam pressure | Stressed      |
| I feel calm and peaceful      | Relaxed       |
| I want to go to the gym       | Energetic     |
| I am thinking about my crush  | Romantic      |
| I am exhausted                | Tired         |
| Today is just normal          | Neutral       |

---

# 📜 Academic Project Information

**Project Type:**
Text and Speech Analysis

**Project Domain:**
Artificial Intelligence / NLP

**Project Title:**
AI-Based Mood-Based Music Recommendation Chatbot using Text and Speech Analysis

**Platform:**
Google Colab

**Interface:**
Gradio

**Programming Language:**
Python

---

# 👩‍💻 Conclusion

The **AI-Based Mood-Based Music Recommendation Chatbot** demonstrates how Natural Language Processing and Speech-to-Text technologies can be combined to create an interactive intelligent chatbot.

The system accepts both text and voice input, analyzes the user's message, detects an approximate mood, and recommends suitable music.

The project provides a simple and practical demonstration of **Text Analysis, Speech Analysis, NLP, Emotion Detection, Chatbot Development, and Recommendation Systems**.

---

## ⭐ Final Output

After running the project in Google Colab, the application generates a public Gradio URL:

```text
https://xxxxxxxx.gradio.live
```

Open the URL and start chatting with the **Mood-Based Music Recommendation Chatbot! 🎵🤖**
