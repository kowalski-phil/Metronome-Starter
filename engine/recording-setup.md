# RECORDING SETUP — camera, green screen, keying

*This is the original run's setup. Your numbers will differ, but treat these as a tested starting point.*

## The one big lesson
For weeks, the webcam background was removed by **AI segmentation**, a model guessing which pixels are "person". When it loses confidence it punches holes, eventually **in the middle of the face**. Swapping AI models didn't fix it.

The fix was a **physical green screen keyed live in OBS**. A chroma key doesn't guess anything; it just removes a colour, so face holes can't happen.

**Tried and rejected in the original run:** other AI matte models · Camtasia's chroma key · DaVinci Resolve's Delta Keyer · DaVinci Magic Mask (too slow per beat) · the OBS "Advanced Masks" plugin (worse than the built-in key) · NVIDIA Broadcast and similar (all AI segmentation again).

## 1. Physical setup
- **Green screen directly behind you**, as close as it goes.
- Normal recording lights. Perfectly even backdrop lighting is **not** required with these settings.

## 2. Signal chain
```
Webcam  →  OBS (Chroma Key + crop + background image source)
        →  OBS Virtual Camera
        →  your recorder (Camtasia in the original; per-beat recording)
```
Your editing pipeline then receives an already-keyed picture and doesn't have to key anything.

## 3. OBS settings: starting values
The filter goes on the **camera source itself**, not on the scene.

| Setting | Value |
|---|---|
| Filter | **Chroma Key** (OBS built-in) |
| Key colour type | Green |
| Similarity | 467 |
| Smoothness | 45 |
| Spill reduction | 103 |
| Opacity | 1.0 |
| Contrast / Brightness / Gamma | 0 / 0 / 0 |

- The background image is a **separate OBS source** behind the camera source.
- The camera source is **cropped**; see below.

## 4. The crop is load-bearing
If the green screen doesn't fill the camera's full view, the crop is what hides the room at the edges. So:
- **Camera and seat must land in the same place every time.** Mark them.
- Before recording, check the OBS preview and confirm no room shows at the edges.

## 5. Backgrounds
- **Full-frame beats:** brand background with your logo.
- **Webcam-bubble beats:** a logo that's only partly visible inside the bubble reads as a real room rather than a virtual background. That's deliberate, not a mistake.
