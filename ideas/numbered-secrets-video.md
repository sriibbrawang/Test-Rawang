# Numbered Secrets Video

A saved video idea, studied from a TikTok by @sebintel ("5 secret codes for Claude", 45 seconds, vertical 9:16, 25 fps).
Only the **features and motion style** are recorded here. Reuse them with our own footage and message.

---

## 1. The idea in one line

**A fast numbered list ("5 secret…"). One person announces each number to camera, then the video jumps straight into a full-screen demo of it, with hand-drawn red marks pointing at what matters.**

## 2. Structure (timeline)

| Part | Time | What happens |
|---|---|---|
| **Hook** | 0–2s | **Split screen:** a b-roll image in the top half (a logo over a laptop) and the speaker in the bottom half. A **red X is drawn by hand** over the logo: "Stop using Claude…" |
| **Teaser** | 2–3.5s | The top half turns black with a **blurred list** of the 5 items you can't quite read yet: "…if you don't know about these 5 secret codes". |
| **Number #1–#5** | 3.5–40s | Each item: the speaker says **"Number #N"** (about 1s), then a **full-screen demo** (screen recording) for 4–6s. |
| **Value dump** | 40–43s | A long document ("Here are all 100…") **scrolls fast** past the camera. |
| **CTA** | 43–45s | The speaker says "Comment **CODE** and I'll DM it to you", with a big **3D word "CODE"** on screen. |

## 3. All the features

1. **Split-screen hook.** A graphic or b-roll card in the top half and the face in the bottom half, so the first frame has both context and a person.
2. **Hand-drawn red X.** Two red marker strokes draw over the top graphic in about 0.5s, as if drawn live, meaning "stop / wrong way".
3. **Blurred teaser list.** The list of items is shown heavily blurred on black. Viewers can see there are 5 things but can't read them, which creates curiosity.
4. **"Number #N" chapter titles.**
   - Big black bold sans, sitting on the speaker's chest.
   - It first appears **faint and behind the person** (text-behind-subject depth effect), then **pops to the front**, sharp.
   - On screen for about 1 second.
5. **Word-pill subtitles.** One or two words at a time, in white on a **dark grey translucent rounded pill**, low centre, swapping on every word ("add /ghost", "your prompt", "will make").
6. **Full-screen screen recordings.**
   - The UI demo fills the frame edge to edge.
   - The command is **typed live**.
   - The camera **slowly zooms or pans** to the important part, then **auto-scrolls** through the result.
7. **Hand-drawn red box.** A red rounded rectangle is **drawn around** the key section of a screenshot while it's mentioned, then stays.
8. **Blur and focus transitions.**
   - Moving from one screen to the next uses a quick **blur whoosh**.
   - New screens often start **out of focus and pull into focus** within about 0.3s.
9. **Proof inserts.** A quick full-screen clip shows the result working (a game, a dashboard) for about 1 second.
10. **Value-dump scroll.** A long list or document scrolls fast to show "there's much more", and the title line is highlighted in yellow.
11. **Keyword CTA.** "Comment CODE": a **big 3D extruded word** (grey, with depth and shadow) sits over the speaker, and the pill subtitles continue ("DM them", "to you").
12. **Pacing.**
    - Each number is about 7s: 1s of announcement, then 5–6s of demo.
    - There's a cut at least every 1–2s.
    - The speaker shots use the same framing, so every return to the face feels like a "chapter" beat.

## 4. Visual style

- **Speaker:** moody background (neon and blue light), a light t-shirt, a medium close-up.
- **Graphics:**
  - Mostly plain black text with no box for chapter titles.
  - Grey pills for subtitles.
  - **Red** (#E02424-ish) only for the marker X and boxes.
- **Screens:** the real UI, bright, with no extra decoration.

## 5. How we can use it at SRIIBB

- **Format:** "**5 things we learned at …**" or "**5 secrets of the Ulul Albab system**". Each number gets a short facilitator or teacher shot, then full-screen slides or footage.
- **Slides as screen demos:** show the slide full screen. **Zoom into** the key part, then **draw a red box** around it, for example the hafazan flow or the juzuk targets.
- **Hook:** split screen with a school photo on top and the speaker below, plus a hand-drawn red X over a common mistake ("Stop memorising like this…").
- **Teaser:** a blurred list of the 5 points before revealing them one by one.
- **CTA:** "Comment **ULUL** and we'll share the slides", using the big 3D word.
- **Word-pill subtitles** come from a speech-to-text transcript, timed word by word. We already do this for the Day 2 video.

## 6. Production notes

- **What works now:**
  - The red X and red box: animated stroke drawing (draw the path progressively over a few frames).
  - Blurred lists, blur and focus transitions, zoom and pan, fast scroll and pill subtitles. These can all be done with Pillow and FFmpeg.
- **Text-behind-subject** needs a person-segmentation mask for each frame (for example MediaPipe Selfie Segmentation or rembg). It's doable but heavier. Test it on one shot first.
- **3D extruded word:** stack the text 8–12 times with a 1px offset in darker greys, then put the light face on top.
- **Footage needed:** this format depends on a **talking-head speaker**. Record one person saying the hook, "Number one… Number five…" and the CTA in a quiet spot, in 9:16.
