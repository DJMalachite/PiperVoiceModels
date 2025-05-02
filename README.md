# Introduction

Hi there!
Each voice model was trained with the open source [Piper](https://github.com/rhasspy/piper) project.

I mainly started this journey to get BT7274 as my Home Assistant Voice PE voice.
[Demo](https://www.reddit.com/r/titanfall/comments/1i3egi8/this_weeks_project_home_assistant_voice_bt7274/)

The model works decently well given on the small data set it was trained but you might find some words will sound wonky.
I havent figured out a way to get around that issue so i am open to suggestions.


# Models
- ## Titanfall 2
- BT7274

# Projects
  - ### [BT_TTS](https://github.com/rmac-silva/BT_TTS) : A simple python script to generate TTS speech
    

# Usage
Download a voice and extract the ```.onnx``` and ```.onnx.json``` files

install piper with pip
```pip install piper-tts```

Run the following command
```
echo 'Hello Pilot' | piper \
  --model <PATH/TO/YOUR?MODEL>.onnx \
  --output_file output.wav
```
See piper --help for more options.
