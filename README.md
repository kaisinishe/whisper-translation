# Otty - Real time voice translation 

OpenAI's Whisper for transcript and ChatCompletion for translation.

![](./img/_848c080e-2ccb-460f-badb-e8e1f454be7c.jpg)

![](./img/2023-03-29-20-35-51.png)

## Features

- From a dropdown, select your spoken language and the language you want to translate to
- `Speech to text transcription & Translation` - Once you begin recording, Whisper and GPT3.5 will attempt to translate each word you speak in real-time
- `Summarize` - Once you are done recording, stop the recording and you will be able to summarize the transcription
- `Voice` - _buggy_. Once you are done speaking, stopping the recording session will give you an option for `Voice`. Which will read the translated text out via the TTS feature

## AI Models

- [Whisper Open Source Model](https://github.com/openai/whisper)
- [GPT3.5-Turbo through Azure](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/chatgpt-quickstart?tabs=command-line&pivots=programming-language-python)
- [ElevenLabs](https://beta.elevenlabs.io/voice-lab) - VoiceAI

## Running locally

### Setup Backend

Requirements:

- **Python version 3.9+** - [Download](https://www.python.org/downloads/)
- **FFmpeg**
  - Mac: `brew install ffmpeg`
  - Windows: follow this [README](https://github.com/openai/whisper#:~:text=It%20also%20requires%20the%20command%2Dline%20tool%20ffmpeg%20to%20be%20installed%20on%20your%20system%2C%20which%20is%20available%20from%20most%20package%20managers%3A)

Setup:

- Follow the [Backend README](./backend/README.md) for further steps

Run the websocket server:

- run `cd backend`
- run `python3 main.py`

### Setup Frontend

Requirements:

- Yarn
- Node (v16+)

Setup:

- run `cd frontend`
- run `yarn install`

Run the WebApp:

- run `yarn start`

