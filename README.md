# MLX Assistant

MLX Assistant is an AI-powered typing assistant that leverages MLX language models to correct text in real-time. Designed to run in the background, it listens for specific hotkeys to fix typos, casing, and punctuation in the selected text or the current line you're typing. This script is optimized for macOS, taking advantage of MLX's performance on Apple devices.

## Prerequisites

- Python 3
- macOS (since MLX is optimized for Apple devices).

## Setup

1. **Install Dependencies**

First, ensure you have Python 3 installed on your system. Then, install the required Python packages:

```bash
pip3 install pynput pyperclip httpx mlx-lm
```


2. **macOS Permissions**

For the script to work correctly on macOS, you need to grant accessibility and input monitoring permissions to the terminal or IDE you are using to run the script. This is necessary for the script to simulate keyboard inputs and listen for hotkeys.

- Go to `System Preferences` > `Security & Privacy`.
- Select the `Privacy` tab.
- Scroll down and select `Accessibility` on the left pane.
- Click the lock icon at the bottom left to make changes (you might need to enter your password).
- Click the `+` button and add your Terminal or IDE application.
- Repeat the above steps for `Input Monitoring`.

3. **Download the Script**

Download `mlx-assistant.py` to your preferred directory.

## Usage

1. Open a terminal or your IDE in the directory where you downloaded `mlx-assistant.py`.
2. Run the script:

```bash
python3 mlx-assistant.py
```


3. With the script running in the background, you can use the following hotkeys in any text editor:

- `F9`: Fixes the current line you're on.
- `Alt+F10`: Fixes the selected text.

The script will automatically replace the text with the corrected version provided by the MLX model.
Feel free to change to your preferred keys in the script.

## Customization

You can customize the hotkeys and the MLX model used by editing the `mlx-assistant.py` script. Look for the `MLX_MODEL` variable to change the model and the `keyboard.GlobalHotKeys` configuration to modify hotkeys.

## Note

This script is designed for macOS users and has been optimized for performance on Apple devices using the MLX platform. Ensure you have the necessary permissions enabled for your terminal or IDE to allow the script to function correctly.
