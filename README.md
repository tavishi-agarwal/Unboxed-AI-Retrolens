# RetroLens 🖐️✨

**Real-time hand gesture portal filters using Python, OpenCV, and MediaPipe.**

RetroLens lets you create a virtual portal using your hands. Spread your hands to open the portal and apply visual effects to the area inside it. Switch between filters using hand gestures or keyboard shortcuts.

## ✨ Features

- 🖐️ Real-time hand tracking using MediaPipe
- 🌀 Interactive portal controlled by hand gestures
- 🎨 Multiple visual filters, including Dual-Tone, Thermal, Sketch, Pixelate, Glitch, Invert, Edge, Cartoon, Blur, and Rainbow Wave
- 🕹️ Gesture-based filter switching
- 🔄 2D and 3D display modes
- 📸 Screenshot capture

## 🛠️ Requirements

Before running RetroLens, make sure you have:

- Python **3.11 (64-bit recommended)**
- Git
- A working webcam
- An internet connection to install the dependencies

> **Compatibility note:** This project uses pinned Python package versions. Python 3.11 is the recommended version for the setup instructions below.

---

## 🚀 Installation and Setup

Follow the instructions for your operating system.

### Step 1: Install Python

Download and install Python 3.11:

https://www.python.org/downloads/release/python-3110/

**Windows users:**
1. Run the installer.
2. If the installer offers **Add Python to PATH**, enable it.
3. Complete the installation.
4. Open Command Prompt and verify:

```bash
py -3.11 --version
```

You should see a Python 3.11 version number.

**macOS users:**

Install Python 3.11 from the link above, or use a trusted Python version manager. Then verify:

```bash
python3.11 --version
```

**Linux users:**

Install Python 3.11 and its virtual environment support using your distribution's package manager. Package names and available versions vary by distribution. Verify:

```bash
python3.11 --version
```

### Step 2: Install Git

Download Git from:

https://git-scm.com/downloads

Follow the installation instructions for your operating system.

Verify the installation:

```bash
git --version
```

### Step 3: Clone the Repository

Open a terminal or Command Prompt and run:

```bash
git clone https://github.com/tavishi-agarwal/Unboxed-AI-Retrolens.git
cd Unboxed-AI-Retrolens
```

### Step 4: Create a Virtual Environment

A virtual environment keeps this project's Python dependencies separate from other projects on your computer.

**Windows — Command Prompt:**

```bat
py -3.11 -m venv .venv
.venv\Scripts\activate
```

**Windows — PowerShell:**

```powershell
py -3.11 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, use Command Prompt instead, or follow Microsoft's guidance for PowerShell execution policies.

**macOS / Linux:**

```bash
python3.11 -m venv .venv
source .venv/bin/activate
```

After activation, your terminal will usually show `(.venv)` at the beginning of the command prompt.

### Step 5: Install Dependencies

Upgrade pip:

```bash
python -m pip install --upgrade pip
```

Install the packages listed in `requirements.txt`:

```bash
python -m pip install -r requirements.txt
```

The project uses these pinned dependencies:

- `mediapipe==0.10.21`
- `opencv-contrib-python==4.10.0.84`
- `numpy==1.26.4`

You do not need to install these packages individually if you have installed `requirements.txt`.

### Step 6: Run RetroLens

Make sure your virtual environment is activated and your webcam is connected.

**Windows:**

```bash
python Retrolens.py
```

**macOS / Linux:**

```bash
python Retrolens.py
```

If your system uses `python3` instead of `python`, you can try:

```bash
python3 Retrolens.py
```

Allow camera access if your operating system asks for permission.

---

## 🎮 Controls

| Gesture / Key | Action |
|---|---|
| Spread both hands | Open or control the portal |
| Pinch thumb and pinky | Switch to the next filter |
| Make fists with both hands | Toggle 2D / 3D mode |
| `C` | Toggle 2D / 3D mode |
| `N` | Next filter |
| `P` | Previous filter |
| `S` | Save a screenshot |
| `Q` | Quit the application |

> Gesture recognition depends on hand visibility, lighting, and camera quality. Keep your hands inside the camera frame for best results.

## 🎨 Available Filters

RetroLens includes visual effects such as:

- Dual-Tone
- Thermal
- Sketch
- Pixelate
- Glitch
- Invert
- Red Channel
- Edge Detection
- Blur
- Cartoon
- Rainbow Wave

Use a pinch gesture or the keyboard controls to switch between filters.

## 🧰 Troubleshooting

### `python` or `py` is not recognized

Python may not be installed correctly or may not be available on your PATH. Reopen your terminal after installation and verify the command. On Windows, try:

```bash
py -3.11 --version
```

### `No module named ...`

Activate the virtual environment and reinstall the dependencies:

```bash
python -m pip install -r requirements.txt
```

### `No module named mediapipe` or MediaPipe installation fails

Confirm that you are using Python 3.11 and that your virtual environment is activated:

```bash
python --version
python -m pip --version
```

Then retry the dependency installation. If it still fails, check the full error output and your operating system and processor architecture.

### Webcam is not opening

- Close other applications that may be using the camera.
- Check your operating system's camera permissions.
- Make sure the webcam is connected and working.
- If you have multiple cameras, you may need to adjust the camera index in `Retrolens.py`.

### Hand tracking is inaccurate

- Improve the lighting in your room.
- Keep your hands clearly visible.
- Avoid moving your hands too quickly.
- Make sure the camera has a clear view of your hands.

## 🔄 Running the Project Again

After the initial setup, you do not need to recreate the virtual environment or reinstall dependencies every time.

Open a terminal in the project folder, activate the environment, and run the program.

**Windows:**

```bat
.venv\Scripts\activate
python Retrolens.py
```

**macOS / Linux:**

```bash
source .venv/bin/activate
python Retrolens.py
```

To leave the virtual environment, run:

```bash
deactivate
```

## 🤝 Contributing

Contributions, ideas, and improvements are welcome!

1. Fork this repository.
2. Create a branch for your changes.
3. Make and test your changes.
4. Open a pull request describing your contribution.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Built while learning and experimenting with Python, OpenCV, and MediaPipe. ❤️
