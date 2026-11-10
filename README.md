# Smile Bloom

Smile at your webcam and flowers bloom behind you, with a soft portrait blur and a golden aura.

**[Try it live](https://shrer488.github.io/Smile-Bloom/)**

## How to use it

1. Open the link in a desktop browser. Chrome works best.
2. Click **Start camera** and allow camera access.
3. Smile.
4. Tap a sticker at the top right to change the flower.
5. Use the buttons at the bottom of the video to take a photo or record a video. The timer button on the left adds a 3 or 10 second countdown first.

At the top left you can switch between wide and vertical video and watch your smile meter. Flowers bloom when your smile passes the white line; drag the line up or down to change how big a smile it takes.

The first load can take a few seconds while the face-tracking models download.

## Flowers

| Flower | Look |
|---|---|
| Gardenia | White blooms with a little sparkle |
| Marigold | Bright orange |
| Carnation | Soft pink |
| Hydrangea | Light blue |
| Sunflower | Bright yellow, with up to 3 honey bees flying around the outside |
| Dahlia | Warm and full |

## Keyboard shortcuts

| Key | What it does |
|---|---|
| `F` | Next flower |
| `T` | Preview the flowers without smiling |
| `V` | Switch to vertical video |
| `R` | Start or stop recording |
| `P` | Take a photo |
| `C` | Timer: off, 3 or 10 seconds |
| `?` | Show the shortcuts in the app |
| `D` | Show debug view |
| `I` | Invert the person mask |

## Privacy

Your camera video is processed in your browser and is not uploaded anywhere by this site.

## Run it locally

The camera needs the page to be served, not opened as a file:

```bash
python3 -m http.server 8765
```

Then open <http://localhost:8765>.

## Built with

- [MediaPipe Tasks Vision](https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker) for face, hand and person tracking
- HTML Canvas for drawing the flowers and effects
- GitHub Pages for hosting
