# Challenge Widget — JSON Text Animation with Anime.js & Tailwind CSS

A simple **Challenge Widget** for Twitch streamers that fetches user-submitted challenge data from JSON (populated by Streamer.bot) and animates the text using [Anime.js](https://animejs.com/), styled with [Tailwind CSS](https://tailwindcss.com/).

---

## Features

- Fetches challenge data from a JSON file updated by Streamer.bot
- Displays challenge name and description in predefined HTML elements
- Animates text letter-by-letter with scaling and fade effects
- Styled with Tailwind CSS for modern responsive design
- Transparent black overlay on background image without affecting text
- Animation starts with a 1-second delay and plays once (no loop)

---

## How It Works with Streamer.bot

- Viewers redeem a Twitch **Channel Point Reward** to submit a challenge (text input).
- Streamer.bot captures this input and updates the `challange.json` file accordingly.
- This widget fetches the latest JSON data and displays the challenge visually on stream.
- The widget is strictly for **visualization**; it does not handle data input or storage.

---

### Import code for Streamer.bot

Paste this into Streamer.bot to import the widget:

```txt
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
```

---

## JSON Format

Your `challange.json` file should contain an array with objects structured like this:

```json
[
  {
    "name": "Challenger Name",
    "desc": "Description of the challenge"
  }
]
```

## Usage

- Clone or download this repository.

- Make sure Streamer.bot writes challange.json in the same folder or adjust the fetch path.

- Open index.html in a browser or add it as a browser source in your streaming software.

- Watch the challenge text animate on screen whenever updated.

## Customization

- Update your JSON file to change challenge content dynamically.

- Modify the animation settings inside the <script> tag to adjust timing, delays, and effects.

- Customize Tailwind CSS classes to change the widget’s styling and layout.

## Dependencies

- Anime.js — animation library (CDN loaded)

- Tailwind CSS — utility-first CSS framework (CDN loaded)
