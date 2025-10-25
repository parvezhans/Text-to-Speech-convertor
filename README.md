Text to Speech (TTS) using Google Colab
📘 Project Overview

This project demonstrates how to convert text into speech using the Google Text-to-Speech (gTTS) library in Google Colab.
It allows users to enter any text and generate a corresponding audio file (.mp3) that can be played directly in the notebook.

🚀 Features

Converts any text into speech

Supports multiple languages (default: English)

Plays the generated audio directly in Colab

Simple and lightweight implementation

🧰 Requirements

Make sure you have the following installed (automatically handled in Colab):

Python 3.x

gTTS (Google Text-to-Speech)

IPython.display for playing audio


🧠 Code Explanation Table
| **Line of Code**                                    | **Explanation**                                                                                                                                                  |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `!pip install gTTS`                                 | Installs the **Google Text-to-Speech (gTTS)** library, which converts text into spoken voice using Google’s TTS API.                                             |
| `from gtts import gTTS`                             | Imports the `gTTS` class used to create speech from text.                                                                                                        |
| `from IPython.display import Audio`                 | Imports the `Audio` function to play audio files directly inside Google Colab or Jupyter Notebook.                                                               |
| `text = input("Enter text to convert to speech: ")` | Prompts the user to type the text they want to convert into speech and stores it in the variable `text`.                                                         |
| `tts = gTTS(text=text, lang='en', slow=False)`      | Converts the text into speech. <br>• `text`: Input text <br>• `lang='en'`: Language code (English) <br>• `slow=False`: Sets speech speed (False = normal speed). |
| `tts.save("output.mp3")`                            | Saves the generated speech audio as an MP3 file named **`output.mp3`**.                                                                                          |
| `Audio("output.mp3")`                               | Plays the saved MP3 file directly inside the notebook using an interactive audio player.                                                                         |


