# Introduction

Hi there!  
Each voice model here was trained using the open source [Piper](https://github.com/rhasspy/piper) text-to-speech engine.

I started this journey to get BT-7274 as my Home Assistant Voice PE voice.  
[Demo](https://www.reddit.com/r/titanfall/comments/1i3egi8/this_weeks_project_home_assistant_voice_bt7274/)

The model works decently well given the small dataset it was trained on, but you might find that some words sound a bit off.  
I haven’t figured out a reliable fix yet, I'm open to suggestions!

---

## 📦 Models

### 🎮 Titanfall 2  
- **BT-7274** – Trained using custom audio clips to mimic the voice of BT from Titanfall 2.

---

## 🔧 Projects

### [BT_TTS](https://github.com/rmac-silva/BT_TTS)  
A simple Python script to generate TTS speech using Piper and the BT-7274 model.

---

## 🚀 Usage

1. **Download a voice model** and extract both the `.onnx` and `.onnx.json` files into a folder.

2. **Install Piper** using pip:

```bash
pip install piper-tts
```

3. **Generate speech** with the following command:

```bash
echo "Hello Pilot" | piper \
  --model <pathtoyour>.onnx \
  --config <pathtoyour>.onnx.json \
  --output_file output.wav
```

> Run `piper --help` for more advanced options.

---

## 🧠 Tips

- Make sure the `.onnx` and `.onnx.json` files are in the correct directory.
- For real-time or batch TTS, check out the `BT_TTS` project above.
- Use "Phonetic" Spelling to get around Pronuciation issues

---

## 📝 License

This project is provided for educational and personal use only.  
All trademarks and character likenesses belong to their respective owners.

---

## 📬 Feedback

Found issues or have ideas to improve BT’s voice quality?  
Please open an issue or submit a pull request. Contributions are welcome!
