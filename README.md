# BUD-E explains itself

<p align="center">
  <a href="https://youtu.be/RYdWd7hRZQk">
    <img src="https://github.com/LAION-AI/Desktop_BUD-E/blob/main/BUD-E-Yt.jpg?raw=true" alt="BUD-E Framework Introduction">
  </a>
</p>

## Project Vision

BUD-E, short for "Buddy", is an innovative voice assistant framework designed to be a plug-and-play interface that allows seamless interaction with open-source AI models and API interfaces. The framework aims to empower anyone to contribute and innovate, particularly in education and research, by maintaining a low entry threshold for writing new skills and building a supportive community.

## Key Features and Flexibility

BUD-E integrates several core components including a speech-to-text model, a language model, and a text-to-speech model. These components are interchangeable and can be accessed either locally or through APIs. The framework supports integration with services from leading providers like OpenAI and Anthropic, or allows users to deploy their own models using open-source frameworks like Ollama or VLLM.

### Skills Interface

Any Python function can become a skill, allowing the voice assistant to handle tasks ranging from processing screenshots with captioning and OCR models to interacting with clipboard contents including text, images, and links. BUD-E supports dynamic skill activation, either by allowing the language model to choose a skill from a "menu" that gets dynamically added to the system prompt or through direct keywords said by the user. 
Skills get dynamically added from the "skills" folder to the system, without any need to change the main code (buddy.py). Think of it as similar to adding mods to the "Mods" folder in Minecraft.

## Community and Educational Focus

BUD-E is dedicated to fostering a community-centric development environment with a strong emphasis on education and research. The framework encourages the development of skills that aid in educational content delivery, such as navigating through specific online courses or generating custom learning paths from YouTube playlists.

## Installation Instructions

The current version of BUD-E currently uses Deepgram for the audio service and Groq the LLM. For the wake word detection it uses Porcupine from Pico Voice ( https://picovoice.ai/platform/porcupine/ ). We are working on a stack of open source models that can very soon run it completely local or on your own API server.

Recommendation: Make a venv and install everything in the venv. Make sure your microphone works.

Set your API keys here:
'''
echo 'export PORCUPINE_API_KEY="yourgroqapikeyhere"' >> ~/.bashrc
echo 'export GROQ_API_KEY="yourgroqapikeyhere"' >> ~/.bashrc
echo 'export DEEPGRAM_API_KEY="yourdeepgramapikeyhere"' >> ~/.bashrc
source ~/.bashrc

git clone https://github.com/christophschuhmann/Desktop_BUD-E

pip install -U -r requirements.txt
 
python3 buddy.py
'''

## Skills

### Types of Skills
[Description of the different types of skills that can be integrated with BUD-E.]

### Skill Usage
[Instructions on how to use skills within the BUD-E framework.]

### Coding New Skills
[Guidelines and examples for coding new skills to extend the functionality of BUD-E.]

## Call for Collaboration

This project is led by LAION, with support from Intel, Camb AI, Alignment Labs, the Max Planck Institute for Intelligent Systems in Tübingen, and the Tübingen AI Center. We invite collaboration from open-source communities, educational and research institutions, and interested companies to help scale BUD-E’s impact.

We encourage contributions that push the boundaries of educational and research tools, leveraging the collective creativity and expertise of the global open-source community.
