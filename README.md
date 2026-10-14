# 辰宝的一天 · Inton päivä

A small bilingual picture game for a toddler (around 2.5 years old). Six scenes follow a little boy, **辰宝 / Into**, through his day. Tap anything in the picture and it says its name out loud, in Chinese (the mum's voice) or Finnish (the dad's voice).

The game is a single HTML file. There is nothing to install and no build step.

## Scenes

| # | Chinese | Finnish | What happens |
|---|---|---|---|
| 1 | 脱外套啦 | Takki pois! | Into takes off his jacket |
| 2 | 早餐时间 | Aamupala | Breakfast |
| 3 | 沙坑游戏 | Hiekkaleikit | Sandpit play with two friends |
| 4 | 午睡时间 | Päiväunet | Nap time |
| 5 | 森林采蘑菇 | Sienimetsässä | Mushroom picking in the forest |
| 6 | 玩汽车 | Autoleikit | Playing with cars with a friend |

Each scene has a caption at the bottom that reads the whole sentence aloud. Words in the picture also appear as chips, so a child can tap a word and hear it again.

## How to play

1. Open `index.html` in a browser.
2. Pick a language at the top: **妈妈 / 中文** or **Isä / SUOMI**.
3. Tap a character or object in the scene. It is named aloud and its word chip pops up.
4. Tap the caption or the speaker button to hear the whole scene sentence.
5. Use the arrows or the dots at the bottom to move between scenes.

On a phone held upright, the words appear in a row under the scene instead of on top of it.

## Running it

** Open the file.** Double-click `index.html`, or drag it into a browser window.


## Voices and audio

- **Recorded clips:** Each word and sentence has an embedded MP3 recording (about 47 clips), stored inside the HTML file as base64. The game works offline once it has loaded.
- **Fallback speech:** If a clip is missing, the game uses the device's text-to-speech. Chinese needs a Mandarin voice (普通话) and Finnish needs a Finnish voice. If none is installed, the game shows a short message explaining how to add one in the system settings.
- **Fonts:** The Chinese typeface (Noto Sans SC) loads from Google Fonts. If you are offline, the browser falls back to a system Chinese font.

## Technical notes

- One file: HTML, CSS, JavaScript, images (WebP) and audio (MP3) are all in `index.html`. It is about 830 KB.
- No frameworks and no dependencies, apart from the Google Fonts link.
- Animations are plain CSS keyframes. They are reduced when the device has "reduce motion" turned on.
- Layout adapts to phones, tablets, and short landscape screens.
- Voice availability depends on the device and browser.

## Folder contents

```
02-into-kindergarden-game/
├── index.html   The game
├── README.md    This file
└── reference/   Working files: the Figma test file and the voice recording scripts (Chinese and Finnish)
```

The recording scripts in `reference/Voice/` list the words and sentences in the order they should be recorded.

## LICENSE

* This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/) - [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/)


