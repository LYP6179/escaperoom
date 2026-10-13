# OLAHRAGA Escape Room — Mobile Portrait

A phone-first, single-page HTML game for Tahun 4–6. It is designed for a portrait phone screen and uses a fixed viewport so the game does not need page scrolling.

## Folder layout

```text
index.html
assets/
  backgrounds/
    intro.png
    stor-sukan.png
    dewan.png          <-- add your Dewan background here
    padang.png
    ending.png
  ui/
    intro-story.png
    arahan-frame.png
    ending-student.png
  room1/                <-- 10 equipment images included
  room2/warmup/         <-- add the five cropped warm-up PNGs here
    1-kepala.png
    2-bahu.png
    3-tangan.png
    4-pinggang.png
    5-kaki.png
  room3/scenarios/      <-- add the five cropped scenario PNGs here
    q1-sebelum-bersukan.png
    q2-pakaian-sukan.png
    q3-semasa-bersukan.png
    q4-apabila-cedera.png
    q5-lontar-peluru.png
```

## Notes before publishing

- Keep filenames exactly as shown, including spaces and capitalization. GitHub Pages paths are case-sensitive.
- The 10 Room 1 equipment PNGs are included and resized to make the download lighter. Their displayed option images are inside a white card.
- Add your own `dewan.png` and crop the warm-up/scenario sheets into the named individual files. If those images are missing, the game shows a fallback emoji rather than breaking.
- `intro-story.png` is shown after a 3-second intro. Tap the story card / MULA area to start.
- Room 1: each event needs exactly two correct equipment images.
- Room 2: arrange Kepala → Bahu → Tangan → Pinggang → Kaki. On phones, the ▲ and ▼ controls work as a touch-friendly alternative to dragging.
- Room 3: five Malay multiple-choice questions. Wrong answers can be retried.
- The game uses no external libraries, no login, and no backend.

## Publish with GitHub Pages

1. Create/open your GitHub repository.
2. Upload the contents of this folder (upload `index.html` and the `assets` folder, not the ZIP file itself).
3. In the repository, open **Settings → Pages**.
4. Choose **Deploy from a branch**, select your main branch and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish and open the generated site URL on a phone to test all scenes.


## Audio
- Built-in synthesized ambience: quiet spooky drone + soft night-cricket chirps.
- Sound effects: button taps, popup, correct/wrong answers, door opening, transition whoosh, and ending alarm/surprise sting.
- No extra audio files or external libraries are required.
- Browsers usually block autoplay audio. Sound starts after the student taps **MULA**; the 🔊/🔇 button can toggle it at any time.
