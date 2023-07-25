# Jarvis A.I Documentation

Jarvis A.I is an artificial intelligence assistant that can perform various tasks, including answering questions, performing web searches, opening applications, and more. This documentation will guide you through the functionalities of Jarvis A.I and how to use them effectively.

## Getting Started

To use Jarvis A.I, you need to have Python and some required libraries installed on your system. You can install the necessary libraries using pip:

```bash
pip install speech_recognition
pip install openai
```

Make sure you have an API key for the OpenAI GPT-3 model. You can get it from the OpenAI website.

## Setting up the API Key

Before you can use Jarvis A.I, you need to set up the API key for the OpenAI GPT-3 model. Replace the value of `apikey` variable with your API key.

```python
apikey = "your_api_key_here"
```

## Function: chat(query)

The `chat` function allows you to have a conversation with Jarvis A.I. It takes a `query` as input and returns the AI's response. The conversation history is stored in the `chatStr` variable, allowing for a more coherent conversation.

Usage:

```python
response = chat("Hello, Jarvis. How are you?")
print(response)
```

## Function: ai(prompt)

The `ai` function utilizes the OpenAI GPT-3 model to generate a response based on the given `prompt`. It saves the response to a file for later reference.

Usage:

```python
ai(prompt="Write an email to my boss for resignation?")
```

## Function: takeCommand()

The `takeCommand` function utilizes the SpeechRecognition library to convert speech to text. It listens to the user's voice input through the microphone and returns the recognized query.

Usage:

```python
query = takeCommand()
print(f"User said: {query}")
```

## Using Jarvis A.I

To interact with Jarvis A.I, run the script and speak your queries or type them directly in the terminal. Below are some example interactions:

1. **Opening Websites:**

   - "Open YouTube" - Jarvis will open YouTube in your default web browser.
   - "Open Wikipedia" - Jarvis will open Wikipedia in your default web browser.
   - "Open Google" - Jarvis will open Google in your default web browser.

2. **Playing Music:**

   - "Open Music" - Jarvis will open your music directory (specified in the script) using the default file explorer.

3. **Asking for the Time:**

   - "What's the time?" - Jarvis will tell you the current time.

4. **Opening Applications:**

   - "Open FaceTime" - Jarvis will open FaceTime if you're using a macOS system.
   - "Open Pass" - Jarvis will open the "Passky" application if installed.

5. **Using Artificial Intelligence:**

   - "Using artificial intelligence" - Jarvis will interact with the OpenAI GPT-3 model based on your input.

6. **Resetting Chat:**

   - "Reset chat" - Jarvis will clear the conversation history (`chatStr`).

7. **Exiting Jarvis:**

   - "Jarvis Quit" - Jarvis will exit and stop listening.

Remember to speak clearly and concisely for better recognition.

## Note

The `say(text)` function utilizes the `os.system` command to speak the given `text`. This function is designed to work on macOS systems. If you are using a different operating system, you may need to modify this function to use a different text-to-speech method.

Keep in mind that Jarvis A.I uses the OpenAI GPT-3 model, and the responses it generates depend on the model's training data and configuration. The `model="text-davinci-003"` in the code refers to a specific version of the model, and you can explore different models provided by OpenAI to find the one that best suits your needs.

Enjoy your interactions with Jarvis A.I and explore its capabilities for various tasks!
