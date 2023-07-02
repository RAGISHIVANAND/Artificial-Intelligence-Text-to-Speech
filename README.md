# Text-to-Speech

To import text-to-speech functionality in Google Colab, you can use the gTTS (Google Text-to-Speech) library, which allows you to convert text into speech. Here's a step-by-step guide:

Install the required libraries: In a code cell in your Colab notebook, install the gTTS library using pip:



!pip install gTTS



Import the necessary modules: In the next code cell, import the gTTS library and the IPython library to display the audio:


from gtts import gTTS
from IPython.display import Audio


Generate the speech: In the next code cell, provide the text you want to convert into speech and create an instance of the gTTS class to generate the speech:



# Specify the text to convert into speech
text = "Hello, how are you?"

# Create a gTTS instance and generate the speech
tts = gTTS(text=text, lang='en')
tts.save("/content/speech.mp3")


Make sure to replace "Hello, how are you?" with the desired text you want to convert to speech.

Play the speech: In the final code cell, use the IPython library to play the generated speech:


# Specify the path to the generated speech file
audio_path = "/content/speech.mp3"

# Play the speech
Audio(audio_path)



Make sure to replace "/content/speech.mp3" with the actual path to your generated speech file.

Run the code: Execute the code cells to generate the speech and play it. The gTTS library will convert the provided text into speech, save it as an audio file, and play the audio in your Colab notebook.
By following these steps, you can import text-to-speech functionality in Google Colab using the gTTS library.


