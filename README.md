# Jarvis 1.0 - A Python Voice Assistant

Jarvis 1.0 is a desktop voice assistant built using Python, designed to help you automate various tasks and retrieve information through voice commands. It's a personal assistant that lives on your computer, making your interactions more hands-free.

## Features

This voice assistant can perform a variety of tasks, including:

* **Greeting and Personalization:** Greets you based on the time of day and asks for your name to personalize interactions.
* **Information Retrieval:**
    * **Wikipedia Search:** Gets summaries from Wikipedia for your queries.
    * **Time:** Tells you the current time.
    * **Wolfram Alpha Calculation:** Answers computational queries and general knowledge questions using Wolfram Alpha.
    * **News Updates:** Fetches top news headlines from The Times of India.
    * **Weather Updates:** Provides weather information for a specified city using OpenWeatherMap.
    * **Jokes:** Tells you random jokes.
* **Web Automation:**
    * Opens popular websites like YouTube, Google, and Stack Overflow in your default browser.
    * Can open the Opera browser.
    * Performs general web searches for your queries.
* **System Control:**
    * Plays music from a specified directory.
    * Locks your computer window.
    * Initiates system shutdown, restart, hibernate, or log off.
    * Empties the Recycle Bin.
    * Can temporarily stop listening for commands for a specified duration.
    * Changes desktop background wallpaper.
    * Takes photos using your webcam.
* **Communication:**
    * Sends emails via Gmail (requires specific setup).
    * Sends messages via Twilio (requires specific setup).
* **Notes:** Allows you to write and read notes.
* **Self-Awareness:** Responds to questions about its name and creator.

## Getting Started

Follow these steps to set up and run Jarvis 1.0 on your local machine.

### Prerequisites

* **Python 3.x:** Ensure you have Python installed. You can download it from [python.org](https://www.python.org/).
* **API Keys:** You will need API keys for some services.
    * **Wolfram Alpha:** Sign up at [developer.wolframalpha.com](https://developer.wolframalpha.com/) to get an App ID.
    * **News API:** Get an API key from [newsapi.org](https://newsapi.org/).
    * **OpenWeatherMap:** Obtain an API key from [openweathermap.org/api](https://openweathermap.org/api).
    * **Twilio:** Create an account at [twilio.com](https://www.twilio.com/) to get Account SID, Auth Token, and a Twilio phone number.
    * **Gmail:** For sending emails, you'll use your Gmail account. If you have 2-Factor Authentication enabled (highly recommended), you **must** generate an [App Password](https://myaccount.google.com/security) to use in the script instead of your regular password. Directly embedding your regular password is a security risk.

### Installation

1.  **Clone the repository (or download the files):**
    ```bash
    git clone [https://github.com/YourUsername/your-repository-name.git](https://github.com/YourUsername/your-repository-name.git)
    cd your-repository-name
    ```
2.  **Create a Virtual Environment (Recommended):**
    This helps manage project dependencies without conflicts.
    ```bash
    python -m venv .venv
    ```
3.  **Activate the Virtual Environment:**
    * **Windows:**
        ```bash
        .\.venv\Scripts\activate
        ```
    * **macOS/Linux:**
        ```bash
        source .venv/bin/activate
        ```
4.  **Install Dependencies:**
    Install all required Python packages using `pip`.
    ```bash
    pip install -r requirements.txt
    ```
    If `requirements.txt` is not yet created, run:
    ```bash
    pip install pyttsx3 SpeechRecognition wikipedia pyjokes wolframalpha requests beautifulsoup4 feedparser twilio pypiwin32 ecapture # Note: ecapture might need special handling if not on PyPI
    ```
    *Note: `ecapture` is mentioned in your code but is not a standard PyPI package. If you encounter issues, ensure `ecapture.py` is in the same directory as your main script or installed correctly according to its specific instructions.*

### Example Commands You Can Say:
"Jarvis, what time is it?"
"Jarvis, open Google"
"Jarvis, search Wikipedia for [topic]"
"Jarvis, play music"
"Jarvis, tell me a joke"
"Jarvis, calculate 5 plus 7"
"Jarvis, what's the weather in London?"
"Jarvis, send an email to [recipient name/address]" (it will prompt for content)
"Jarvis, write a note"
"Jarvis, read note"
"Jarvis, shutdown system"
"Jarvis, take a photo"
"Jarvis, change my name to [new name]"
"Jarvis, who made you?"
"Jarvis, don't listen for 60 seconds"
"Jarvis, bye"
