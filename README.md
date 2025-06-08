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
