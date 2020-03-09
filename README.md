# Udacity-Project-Showcase-

Text Detection, Translation and Text to Speech

I would be using the "text-recognition-0012" pretrained model and translate using AuotML Translation and then use Google's text To Speech to give out an Audio.


Text-to-Speech is ideal for any application that plays audio of human speech to users. It allows you to convert arbitrary strings, words, and sentences into the sound of a person speaking the same things.

Imagine that you have a voice assistant app that provides natural language feedback to your users as playable audio files. Your app might take an action and then provide human speech as feedback to the user.

For example, your app may want to report that it successfully added an event to the user's calendar. Your app constructs a response string to report the success to the user, something like "I've added the event to your calendar."


Sample code and how to change it.



Google Cloud Text-to-Speech API Python Samples
https://gstatic.com/cloudssh/images/open-btn.png
This directory contains samples for Google Cloud Text-to-Speech API. The `Google Cloud Text To Speech API`_ enables you to generate and customize synthesized speech from text or SSML.

Setup
Authentication
This sample requires you to have authentication setup. Refer to the Authentication Getting Started Guide for instructions on setting up credentials for applications.

Install Dependencies
Clone python-docs-samples and change directory to the sample directory you want to use.

$ git clone https://github.com/GoogleCloudPlatform/python-docs-samples.git
Install pip and virtualenv if you do not already have them. You may want to refer to the Python Development Environment Setup Guide for Google Cloud Platform for instructions.

Create a virtualenv. Samples are compatible with Python 2.7 and 3.4+.

$ virtualenv env
$ source env/bin/activate
Install the dependencies needed to run the samples.

$ pip install -r requirements.txt
Samples
Quickstart
https://gstatic.com/cloudssh/images/open-btn.png
To run this sample:

$ python quickstart.py
List voices
https://gstatic.com/cloudssh/images/open-btn.png
To run this sample:

$ python list_voices.py
Synthesize text
https://gstatic.com/cloudssh/images/open-btn.png
To run this sample:

$ python synthesize_text.py

usage: synthesize_text.py [-h] (--text TEXT | --ssml SSML)

Google Cloud Text-To-Speech API sample application .

Example usage:
    python synthesize_text.py --text "hello"
    python synthesize_text.py --ssml "<speak>Hello there.</speak>"

optional arguments:
  -h, --help   show this help message and exit
  --text TEXT  The text from which to synthesize speech.
  --ssml SSML  The ssml string from which to synthesize speech.
Synthesize file
https://gstatic.com/cloudssh/images/open-btn.png
To run this sample:

$ python synthesize_file.py

usage: synthesize_file.py [-h] (--text TEXT | --ssml SSML)

Google Cloud Text-To-Speech API sample application .

Example usage:
    python synthesize_file.py --text resources/hello.txt
    python synthesize_file.py --ssml resources/hello.ssml

optional arguments:
  -h, --help   show this help message and exit
  --text TEXT  The text file from which to synthesize speech.
  --ssml SSML  The ssml file from which to synthesize speech.
Audio profile
https://gstatic.com/cloudssh/images/open-btn.png
To run this sample:

$ python audio_profile.py

usage: audio_profile.py [-h] [--output OUTPUT] [--text TEXT]
                        [--effects_profile_id EFFECTS_PROFILE_ID]

Google Cloud Text-To-Speech API sample application for audio profile.

Example usage:
    python audio_profile.py --text "hello" --effects_profile_id
        "telephony-class-application"

optional arguments:
  -h, --help            show this help message and exit
  --output OUTPUT       The output mp3 file.
  --text TEXT           The text from which to synthesize speech.
  --effects_profile_id EFFECTS_PROFILE_ID
                        The audio effects profile id to be applied.
The client library
This sample uses the Google Cloud Client Library for Python. You can read the documentation for more details on API usage and use GitHub to browse the source and report issues.



https://github.com/GoogleCloudPlatform/python-docs-samples/tree/master/texttospeech/cloud-client
