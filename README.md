# 🎛️ Senior Switchman Simulator

## 📌 Project Overview

This project was developed as part of the **WISE (Women In Software Engineering)** program. It simulates a home automation system where a microcontroller controls 16 switches throughout a home, inspired by the classic "Senior Switchman" problem statement.

The simulator includes an interactive GUI with video and audio feedback, allowing users to toggle individual switches, control all switches at once, and query the current switch states.

---

## ✅ Features Implemented

- Toggle any individual switch ON/OFF via GUI buttons  
- Turn all switches ON or OFF at once  
- Query the state of a specific switch or all switches  
- Play unique video and show images based on switch state  
- Sound effect played on startup  
- Cover video when all switches are turned ON  

> ⚠️ The scheduled automatic ON/OFF functionality (`# ON AT τ`, `# OFF AT τ`) is **not implemented**.

---

## 🛠️ Technologies Used

- **Python 3**  
- **Tkinter** — GUI development  
- **MoviePy** — Video playback  
- **Pygame** — Audio playback  
- **Pillow (PIL)** — Image handling  
- **NumPy** — Video frame processing  
- **Threading** — For smooth GUI and video interactions  

---

## 🗂️ File Structure

```
Project Root
│
├── senior_switchman.py           # Main application file
├── audio.mp3                     # Audio played on button click
├── cover page.png                # Welcome screen background
├── cover page.mp4                # Video shown when all switches ON
├── gate1.mp4                     # Entry animation video
├── image_1.png ... image_16.png  # Images for each switch
├── video_1.mp4 ... video_16.mp4  # Videos for each switch
└── README.md                     # This file
```

---

## 🚀 How to Run

1. Make sure Python 3 is installed.  
2. Install the required libraries:

   ```bash
   pip install pygame moviepy pillow numpy
   ```

3. Place all image, audio, and video files in the same directory as `senior_switchman.py`.

4. Run the project:

   ```bash
   python senior_switchman.py
   ```

---

## 💡 Future Improvements

- Implement support for scheduled switch control (`ON AT`, `OFF AT`)
- Load switch configuration from input commands or file
- Display time simulation and schedule tracking
- Add error handling for missing media files

---

## 📸 Example (from problem statement)

```
Input:        1 ON
Meaning:      Turn on Switch #1
Action:       None

Input:        ?1
Meaning:      What is the state of Switch #1?
Action:       Print SWITCH 1 ON

Input:        ?ALL
Meaning:      What is the state of all 16 switches?
Action:       Print ON/OFF states
```

---

## 📚 Credits

Inspired by the Senior Switchman simulation problem statement.  
Developed as part of the **WISE (Women In Software Engineering)** program.
