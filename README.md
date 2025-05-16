# speech-based-search-engine-4-.py


# 🎙️ Speech-Based Search Engine

This Python script allows users to perform Google searches using their **voice input**. It listens to your voice command, converts it into text using **Google Speech Recognition**, and opens the corresponding search results in your web browser.

---

## 📦 Dependencies

Make sure you have the following packages installed:

```bash
pip install SpeechRecognition pyttsx3
```

You also need:

* An internet connection (for Google's speech recognition)
* A working microphone

---

## 🚀 How It Works

1. The script starts and prompts you with:

   > "What do you want to search for?"

2. It listens to your voice via the microphone.

3. The voice is transcribed to text using Google’s Speech Recognition API.

4. The recognized text is searched on Google, and your default browser opens the results.

---

## 🧠 Code Overview

* `speak(text)`
  Uses `pyttsx3` to convert text to speech.

* `take_command()`
  Captures audio, transcribes it, and handles errors like no speech or request failure.

* `search_web(query)`
  Opens a Google search URL with the recognized query.

* `main()`
  Ties everything together—listens, recognizes, and searches.

---

## 🛠️ Example Usage

When you run the script:

```bash
python "speech based search engine (4).py"
```

Say something like:

> "Python programming tutorials"

Your browser will open:
**[https://www.google.com/search?q=Python+programming+tutorials](https://www.google.com/search?q=Python+programming+tutorials)**

---

## 📌 Notes

* If speech isn’t recognized clearly, the script responds:

  > "Sorry, I did not catch that."

* In case of API/network issues:

  > "Sorry, there was a problem with the speech recognition service."

---


