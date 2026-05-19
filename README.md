# AURA A.I. Assistant

## What is AURA?

AURA is a **voice-activated AI assistant** for your computer, similar to Siri or Alexa, but running locally on your machine with Google's Gemini AI.

## How It Works (Simple Terms)

### 1. **You Talk or Type**
- Speak into your microphone
- Or type commands in the text box

### 2. **AURA Listens & Thinks**
- Uses Google's Gemini AI (same tech behind Bard/Gemini)
- Remembers what you tell it (like your name, preferences)

### 3. **AURA Responds**
- **Speaks back** to you through speakers
- Shows text responses in the log window
- Can **perform actions** on your computer

To make AURA work need gemini api key

## What Can AURA Do?

| Action | What it does |
|--------|--------------|
| **Open apps** | Opens Chrome, Notepad, Spotify, Terminal |
| **Close apps** | Closes running applications |
| **Take photo** | Uses your webcam to capture a photo |
| **Screenshot** | Takes a picture of your screen |
| **Web search** | Searches Google for information |
| **Weather** | Tells weather for any city |
| **Remember things** | Saves info like "My name is John" |
| **Shutdown** | Turns off AURA |

## The Visual Interface

The window has 3 main parts:

```
┌─────────────────────────────────────────────┐
│  [Quick Commands]  [HUD Animation]  [Log]   │
│  - Take photo      ████             You: hi │
│  - Screenshot      ○○○○             AURA: Hi│
│  - Weather         ◇◇◇◇                   │
│  - Open Chrome                              │
│                          [Type here]        │
└─────────────────────────────────────────────┘
```

- **Left sidebar**: Quick buttons for common commands
- **Center**: Animated "face" that shows if AURA is listening, thinking, or speaking
- **Right panel**: Shows conversation history, file upload, and text input

## Technical Requirements

To run this, you need:

```bash
# Install required packages
pip install sounddevice google-generativeai psutil PyQt6
pip install opencv-python pyautogui pillow  # optional for camera/screenshots
```

## Setup Process

1. **First run** - A setup window appears asking for:
   - Your Google Gemini API key (get from makersuite.google.com)
   - Your operating system (Windows/Mac/Linux)

2. **Save config** - Creates a config file with your API key

3. **Ready to use** - Starts listening for your voice or text commands

## The Cool Visual Effects

The center circle animates:
- **Blue pulsing** = Listening
- **Orange speaking** = Talking to you
- **Spinning rings** = Thinking/Processing
- **Red muted** = Microphone off

## Simple Usage Example

1. Say or type: *"Open Chrome"*
2. AURA thinks for a moment
3. Chrome browser opens
4. AURA says: *"Opened Chrome"*

1. Say: *"Remember my name is Sarah"*
2. AURA saves this to memory
3. Later ask: *"What's my name?"*
4. AURA recalls: *"Your name is Sarah"*

## File Upload Feature

Drag and drop any file onto the interface:
- Images, documents, audio, video
- AURA sees the file and can analyze it

## Keyboard Shortcuts

- **F4** - Mute/unmute microphone
- **F11** - Fullscreen mode

## In Simple Summary

**AURA = Voice + AI + Computer Control**

Think of it as giving your computer ears (microphone), a brain (Gemini AI), and hands (to open apps, take screenshots). All wrapped in a cool futuristic interface that animates to show what it's doing.
