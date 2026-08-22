# voice-assistant:
# 🎙️ Angel - AI Voice Assistant

**Angel** is a Python-based voice assistant developed as a TechExpo project. It allows users to interact with the computer using voice commands and provides features such as web browsing, music playback, weather information, general knowledge, jokes, application launching, quizzes, and an interactive Tic-Tac-Toe game.

The project combines **Speech Recognition, Text-to-Speech, APIs, Web Automation, and Python-based Game Development** into a single voice-controlled assistant.

---

## 🚀 Features

### 🎤 Voice Interaction

* Recognizes commands through the microphone.
* Converts speech into text using Google Speech Recognition.
* Responds using text-to-speech.
* Uses the assistant name **Angel** as the wake word.

### 🌐 Web Automation

Angel can open:

* YouTube
* Google
* Stack Overflow

It can also play songs on YouTube using voice commands.

### 💻 Application Launcher

The assistant can launch desktop applications through voice commands, including:

* Google Chrome
* Microsoft Power BI
* Microsoft Excel

> Application paths may need to be changed based on the computer's installation location.

### ⏰ Time & Weather

* Provides the current time.
* Retrieves weather information using the **OpenWeatherMap API**.
* Displays the weather condition and temperature for a selected city.

### 📚 Knowledge & Information

Angel can answer basic questions such as:

* Who is the father of Computer Science?
* Who founded Artificial Intelligence?
* Who invented the computer?
* Who is the father of voice assistants?
* What recent technologies are popular?

Wikipedia is also used to retrieve information about people and topics.

### 😂 Entertainment

Angel includes:

* Random jokes using `pyjokes`
* Heads or tails
* Basic quiz functionality
* Interactive Tic-Tac-Toe game

### 🎮 Tic-Tac-Toe

The project includes a graphical Tic-Tac-Toe game built using:

* **Pygame**
* **NumPy**

Features include:

* 3 × 3 game board
* Two-player gameplay
* Mouse-based controls
* Win detection
* Draw detection
* Game restart using the `R` key

---

## 🛠️ Technology Stack

| Technology        | Purpose                        |
| ----------------- | ------------------------------ |
| Python            | Core programming language      |
| SpeechRecognition | Voice command recognition      |
| pyttsx3           | Text-to-speech                 |
| PyWhatKit         | YouTube automation             |
| Wikipedia         | Information retrieval          |
| Requests          | Weather API requests           |
| Pygame            | Tic-Tac-Toe interface          |
| NumPy             | Game board management          |
| PyJokes           | Joke generation                |
| Webbrowser        | Opening websites               |
| OS                | Launching desktop applications |

---

## 📦 Python Libraries

Install the required packages using:

```bash
pip install pyttsx3
pip install SpeechRecognition
pip install pywhatkit
pip install wikipedia
pip install requests
pip install pygame
pip install numpy
pip install pyjokes
pip install pyaudio
```

If `pyaudio` installation fails on Windows, use a compatible PyAudio package for your Python version.

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Angel-Voice-Assistant.git
```

```bash
cd Angel-Voice-Assistant
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure the Weather API

The application uses the OpenWeatherMap API.

Create your own API key and replace the API key in the Python file:

```python
api_key = "YOUR_API_KEY"
```

**Do not upload your actual API key to GitHub.**

A better approach is to store it as an environment variable:

```python
api_key = os.getenv("OPENWEATHER_API_KEY")
```

### 4. Configure Application Paths

If you want Angel to open desktop applications, update the paths according to your system.

Example:

```python
os.startfile(
    r"C:\Program Files\Microsoft Power BI Desktop\bin\PBIDesktop.exe"
)
```

The paths may be different on another computer.

### 5. Run the Assistant

```bash
python angel.py
```

Angel will start with a welcome message and begin listening for voice commands.

---

## 🗣️ Example Voice Commands

You can try commands such as:

```text
Angel, play Shape of You
Angel, what is the time?
Angel, who is Alan Turing?
Angel, open Chrome
Angel, open Power BI
Angel, open Excel
Angel, open YouTube
Angel, open Google
Angel, tell me a joke
Angel, heads or tails
Angel, what is the weather?
Angel, are you an AI?
Angel, who created you?
Angel, what is your name?
Angel, play Tic-Tac-Toe
Angel, goodbye
```

---

## 🔄 How It Works

```text
              ┌─────────────────┐
              │  User Speaks    │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Speech          │
              │ Recognition     │
              └────────┬────────┘
                       │
                       ▼
              ┌─────────────────┐
              │ Command         │
              │ Processing      │
              └────────┬────────┘
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
     Web Search    Applications   Games
          │            │            │
          └────────────┼────────────┘
                       ▼
              ┌─────────────────┐
              │ Voice Response  │
              │   using TTS     │
              └─────────────────┘
```

---

## 📂 Project Structure

```text
Angel-Voice-Assistant/
│
├── angel.py
├── requirements.txt
├── README.md
└── assets/
    └── screenshots/
```

---

## 🔐 Security Note

The original project contains an API key directly in the source code.

Before uploading the project to GitHub:

1. Remove the API key.
2. Revoke the exposed key if it has already been published.
3. Create a new API key.
4. Store the new key using an environment variable.

Example:

```python
import os

api_key = os.getenv("OPENWEATHER_API_KEY")
```

---

## 🔮 Future Enhancements

* Add a graphical user interface.
* Add wake-word detection without requiring the word in every command.
* Add conversational AI using an LLM.
* Add voice-controlled email and messaging.
* Add Spotify integration.
* Add reminders and alarms.
* Add system controls such as volume and brightness.
* Improve natural-language understanding.
* Add multilingual voice support.
* Add face recognition for personalized access.
* Store user preferences and conversation history.

---

## 🎓 Project Information

**Project Name:** Angel Voice Assistant

**Event:** TechExpo

**Language:** Python

**Project Type:** Voice Assistant / Desktop Automation

**Author:** D. Dafnika

**Institution:** PSG College of Arts & Science, Coimbatore, India

---

## 📜 License

This project is developed for **educational and demonstration purposes**.

---

## ⭐ Acknowledgement

This project demonstrates how Python can be used to integrate **Speech Recognition, Text-to-Speech, APIs, Web Automation, Desktop Automation, and Game Development** into a practical voice assistant application.
