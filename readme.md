# DeepSeek Code

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![Powered by DeepSeek](https://img.shields.io/badge/Powered%20by-DeepSeek-4D6BFE)

A coding agent that lives in your terminal. It reads, writes, tests and fixes your project while you stay in control of every action. Models are provided by [DeepSeek](https://www.deepseek.com).

DeepSeek Code is an independent project. It is not affiliated with, endorsed by, or sponsored by DeepSeek-AI.

## What it does

- Chat with a coding assistant directly from your terminal.
- Let the assistant work on your machine: run commands, read and write files, and edit `.docx` and `.odt` documents.
- Stay in control: every action is shown in full and runs only after you type `y`. Any other answer cancels it.
- Analyze images (beta): read the text in a screenshot or photo and get a description of what it shows.
- Track your usage: see your plan and remaining tokens at any time with `/me`.
- Works on Linux and Windows.

## Requirements

- Python 3.8 or newer
- An access key (see the website for how to get one)

## Installation

Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -e .
```

Windows:

```powershell
py -3 -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -e .
```

Windows users can also run `setup.bat` once, then `start.bat` to launch.

## First launch

```bash
deepseek-code
```

On the first launch you are asked for your access key. It is saved locally next to the client. You can also set it yourself:

```bash
deepseek-code --set-key YOUR_KEY
```

## Commands

| Command | Description |
|---|---|
| `/help` | Show the list of commands |
| `/me` | Show your plan and remaining tokens |
| `/clear` | Clear the current conversation |
| `/exit` | Quit |

## Image analysis (beta)

The beta client can look at an image for you.

```
/image screenshot.png
/image invoice.png extract only the total
```

You can also just give the assistant the path of an image in your message and let it use the image tool, after your confirmation.

- Supported formats: JPEG, PNG, GIF and WebP.
- The default mode is designed to use very few tokens per image.
- The analysis describes what is visible and reads the text. It does not identify people by name.
- This feature is experimental and may change.

## Your data and your safety

- The client never asks for or stores any secret other than your own access key, kept locally in `key.txt`. Do not share this file.
- Nothing runs on your computer without your explicit confirmation.
- Always review code produced by an AI model before running or deploying it.

## Acceptable use

DeepSeek Code is intended for lawful software development and for learning. Using it to attack, probe, or gain unauthorized access to systems you do not own or do not have explicit written permission to test is prohibited and may be illegal. You are solely responsible for how you use the tool and for the instructions you give it. Access keys used in violation of the terms may be suspended or permanently revoked.

The full terms of sale and privacy policy are available on the website.

## Support

Open a ticket on the official Discord server linked on the website. [Discord Server](https://discord.gg/cgrgCsWVr9)

## License

All rights reserved. Contact the author for any licensing question.

## Credits

Designed and developed by exyzcx. Language models provided by DeepSeek.
