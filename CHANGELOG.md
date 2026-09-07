# Changelog

What changed in each published version of Kitsumi, written for the people
using it. Newest first.

---

## 7.5.0

_Published September 2026_

### Added

- **Korean dictionary expansion.** The KRDICT Learners' Dictionary from the
  National Institute of Korean Language, in Korean to English, Spanish,
  French and Arabic, with full senses, graded vocabulary and example
  sentences -- alongside a Korean pronunciation dictionary and a frequency
  list. All openly licensed.
- **Wikipedia dictionaries for 19 languages.** Character names, places,
  shows, brands and proper nouns that standard dictionaries do not carry,
  looked up in the language you are studying.
- **Clearer online sources.** Each online lookup source now states which
  language it answers in: Lingva, MyMemory and Glosbe follow your Explain
  language, while Wiktionary, Jisho and Free Dictionary answer in English
  because that is the only edition their API serves.
- **Foldable Review panel and Anki draft queue**, both remembering whether
  you left them open.
- **An occasional support note.** A small dismissible banner at a few streak
  milestones -- each shown once, never more than one a day, never in your
  first session.

### Improved

- **Reliable subtitle loading on YouTube.** YouTube identifies a video in the
  URL's query string rather than its path, and its player keeps reporting the
  previous video for a moment after you navigate. Kitsumi now recognises a
  genuine video change and waits for the player to finish swapping before
  fetching, so clicking through to a new video loads that video's subtitles.
- **Subtitles appear without opening the popup.** Under the default "wait for
  play" timing, downloaded subtitles were held until a play event arrived --
  which never comes if the video was already playing by the time the download
  finished. A short-lived watcher now checks whether a video is genuinely
  playing and hands the subtitles over. It exists only while something is
  waiting and stops itself the moment it is done, so it costs nothing the
  rest of the time.
- **Honest episode matching on long series.** Past the point where later
  episodes are only available inside archives, Kitsumi now reports which
  episode it could not match and leaves your current subtitles in place,
  rather than falling back to the first episode.
- **Steadier review sessions.** Grading is now single-action, and going back
  to regrade a word keeps one copy of it in the queue.
- **Multi-line subtitles copy with their line breaks intact.**
- **Full theme coverage.** A handful of elements kept their original colours
  whichever theme was selected. The cause was a subtlety in how CSS custom
  properties work: a property resolves the references inside it where it is
  *declared*, not where it is used -- so theme tokens declared once at the
  document root locked to the default palette and never saw the per-theme
  overrides applied further down. Declaring them where the theme is applied
  brought provider descriptions, status messages and section titles back into
  line together.
- **Redesigned level-up and achievement celebrations** -- a frosted card with
  new particle effects, gold for level-ups and pink for achievements.
- **Consistent layout throughout** -- even spacing between settings
  categories, breathing room in the dictionary, subtitle and episode lists,
  keyboard focus rings, themed scrollbars and themed text selection.
- **Cleaner number fields**, without the operating system's stepper arrows.
  Typing, arrow keys and scrolling all still work.
- **New Discord invite link.**

---

## 7.2

The release that turned the overlay into a study tool and gave the interface
its current look.

### Added

- **Known words and a comprehension score.** Mark the words you know and see
  how much of a line is new to you, so you can choose material at the right
  difficulty instead of guessing.
- **Built-in review, no Anki required.** A spaced-repetition queue inside the
  extension: grade a word Again, Hard, Good or Easy and it returns when you
  need it. Anki mining continues to work exactly as before for anyone who
  prefers it.
- **Dual subtitles.** Target language and your own language together, with
  the second line easy to switch off once you stop needing it.
- **OCR into live dictionary words.** Text pulled from images and hardsubbed
  frames behaves like any other subtitle text -- hover it and look it up.
- **Drag to reorder tabs.**
- **A guided welcome page** -- pick your study language, try the hover
  dictionary on a real sentence, and start with sensible defaults.
- **The popup remembers its size.**

### Improved

- **A complete visual redesign** -- frosted surfaces, a consistent icon set
  in place of emoji, ranks drawn as icons, and every element following the
  theme you choose.
- **Reworked episode re-detection**, so subtitles keep pace as you move
  through a series.
- **Grouped and labelled dictionary lists**, with the recommendations for
  your language surfaced first.
- **Anki cards now capture audio and video clips** along with the screenshot
  and sentence.
- **Precise subtitle text selection**, including on YouTube.
- **Language filtering in subtitle search** now actually narrows the list.
- **Manually loaded subtitles stay loaded** through the first cues.

---

## 7.1

The groundwork: subtitles you control, a dictionary for every supported
language, and lookups beyond the video player.

### Added

- **Undock the overlay into its own window**, sized and positioned
  independently of the page.
- **Per-language recommended dictionaries**, so every supported language
  opens with a starting point rather than an empty list.
- **Articles Reader** -- the same hover dictionary on ordinary webpages.
- **An optional Tesseract OCR engine** alongside the browser's built-in one.
- **Timing offsets saved per show**, surviving episode changes.
- **Episode re-detection** for sites that do not announce navigation clearly.
- **Performance controls** -- response-time presets and background-tab
  pausing.

---

<!--
HOW TO ADD AN ENTRY

Copy a block above. Keep it short, and drop any group that is empty.

Write from the user's side of the screen, and describe what now works rather
than what used to be broken:

  Good:  "Subtitle offsets are now saved per show."
  Bad:   "Fixed offsets being wiped on every episode change."
  Bad:   "Refactored the offset persistence layer into the cache module."

Never include: file names, function names, storage keys, internal version
numbers, unreleased plans, opinions about people or places, or details of how
a security issue worked. Those belong in the private notes.
-->
