<h1>🦊 Kitsumi <img src="https://komarev.com/ghpvc/?username=Olexify&repo=Kitsumi&label=visitors&color=orange&style=flat-square" alt="visitors" /></h1>

### Learn Japanese from the anime, YouTube and shows you already watch - native subtitles with a dictionary under your cursor.

Watching foreign videos with *English* subtitles never taught anyone a language. You read English, you learn English. What actually works is *native* subtitles with the meaning one hover away - and until now that meant gluing five plugins together, pausing every ten seconds and pasting half-remembered kana into Google.

**Kitsumi collapses all of that into the page you're already on.** Open YouTube and it just works. Watching anime? It finds the subtitles for you. Then **hover a word** - no pausing, no tab switching, no copy-paste. That's the whole idea 😎

Japanese is the main focus; 45+ other languages come along for the ride.

<p align="center"><a href="https://addons.mozilla.org/firefox/addon/Kitsumi/"><img src="https://img.shields.io/badge/Firefox-Install-18181B?style=for-the-badge&logo=firefoxbrowser&logoColor=white&labelColor=FF7139&color=18181B" height="44" alt="Firefox Install"></a>&nbsp;<a href="https://chromewebstore.google.com/detail/Kitsumi/ciiembegoahhehnfdkbanhioobokjdkd"><img src="https://img.shields.io/badge/Chrome-Install-18181B?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=4285F4&color=18181B" height="44" alt="Chrome Install"></a>&nbsp;<a href="https://discord.gg/UpmNHxT7PF"><img src="https://img.shields.io/badge/Discord-Join-18181B?style=for-the-badge&logo=discord&logoColor=white&labelColor=5865F2&color=18181B" height="44" alt="Discord Join"></a></p>

<p align="center"><a href="https://chromewebstore.google.com/detail/Kitsumi/ciiembegoahhehnfdkbanhioobokjdkd"><img src="https://github.com/user-attachments/assets/95f715d9-313d-4fc8-8159-c3ee13482009" width="900" alt="Kitsumi subtitle overlay with dictionary popup"></a></p>

<p align="center"><b>Free · no account · no subscription · no telemetry · Firefox & Chrome · interface in 20 languages</b><br><a href="https://kitsumi.org/">kitsumi.org</a></p>

---

## 🦊 The honest pitch

Kitsumi started from one problem: *"I want to study Japanese from anime - without spending 40 minutes setting up plugins before episode 7."*

**What it does:** deletes the setup tax. Finding subtitles, syncing them, finding dictionaries, cutting audio for a card - that's overhead, and overhead deserves to be automated.

**What it doesn't do:** learn the language for you. Hovering a word is *recognition*, and recognition feels like progress while mostly not being progress. Memory gets built when you guess before you look, retell the scene, and say the sentence yourself. Kitsumi gives you the tools for that - the doing is still yours. Anyone selling passive fluency is selling a fairy tale.

| Kitsumi handles | You handle |
| :--- | :--- |
| Subtitles, timing, dictionaries, lookups, cards, stats | Attention, guessing, recall, output |

### 🌱 Micro-dose learning

A hover gives you two seconds with one word, then straight back to the story. Alone, it's nothing. But the same word turns up again two scenes later, next episode, next week - and every time it's one hover away. Hundreds of tiny, well-spaced contacts with words you actually care about is how recognition quietly piles up, without ever turning the episode into homework. (Recognition, not fluency - see above. The guessing and speaking are still on you.)

It doesn't replace your course, Anki, textbooks or a tutor. It's the missing layer between *"I'm watching something"* and *"wait - I actually learned something."*

And yes, Japanese gets special treatment. Kanji declared war first. 🇯🇵⚔️

### 👀 Who it's for

- **Japanese learners who watch anime or Japanese YouTube** - the reason Kitsumi exists.
- **Immersion learners and sentence miners** - Anki / Yomitan people who want the setup to disappear.
- **JLPT students** - levels on every word, and real context to meet them in.
- **Learners of 45+ other languages** - Yomitan-format dictionaries, the same overlay, the same loop.

---

## ⚡ Your first episode in about five minutes

1. **Install**, open a video, click the 🦊 icon.
2. **Pick your language** on the welcome screen - it sets sensible defaults.
3. **Download one dictionary** from the Dict tab. One is enough to start.
4. **Get subtitles** - pick the track on YouTube, *Search* the providers, or drop in your own `.srt` / `.vtt` / `.ass`.
5. **Hover a word.** That's the whole loop.

Everything below is optional. Leave the defaults alone until you actually want something.

---

## 🎬 Subtitles: yours, on top of anything

Load your own `.srt` · `.vtt` · `.ass`, or pull them from the player - over YouTube, Netflix, Crunchyroll, local files and most HTML5 players.

| 🎨 Appearance | ⚙️ Control | 🔁 Continuity |
| :--- | :--- | :--- |
| Font, size, colours, outline, position, presets | Timing offsets down to ±10 ms | Offsets saved **per show** |
| Resizable, movable overlay | Nudge strip: -1000 ms → +1000 ms | Auto-next episode keeps your setup |

Because some subtitle files have perfect translation, perfect timing, and the visual design of a 2007 fansub made in Microsoft Paint.

### 🔍 Find subtitles without leaving the video

| 🦊 Jimaku | 🌐 OpenSubtitles | 📥 SubDL | 🎌 Kitsunekko |
| :---: | :---: | :---: | :---: |
| Anime · 🇯🇵 JP | Movies & anime · 🌍 | Large database · 🌍 | Anime · 🇯🇵 JP |

No more `anime → Google → random subtitle site → popup → popup → wrong episode → wrong format → why am I here`. **Side quest: skipped.**

---

## 📖 Hover a word. Know a word.

Every subtitle line becomes an interactive dictionary: readings with furigana, definitions, part of speech, JLPT level and frequency wherever the data exists.

<p align="center"><a href="https://youtu.be/cirDXY3CkSk"><img src="https://github.com/user-attachments/assets/189a8bc1-b207-40f1-bc77-ff08d0b962f8" width="900" alt="Interactive dictionary popup over a subtitle line"></a></p>

**Two rows, two readings.** Japanese has no spaces, so any word splitter will sometimes guess wrong. Kitsumi reads each line twice: hover the **lower half** of a word for the whole thing (`ひび割れた`, `近づかなきゃ`), the **upper half** for its pieces (`ひび割れ | た`, `近づか | なきゃ`). The rows are built to disagree when the line is ambiguous - if one of them guessed wrong, the other gives you a way out.

**Hover the pieces too.** When a word is shown through its parts (`曇りなく = 曇り + なく`), hover a part and a small card explains it - including the endings nobody explains to beginners: `なく`, `ず`, `ながら`, `なきゃ`, `んだ`. Particles and endings get a plain-language grammar note first, so `なく` reads as *"without"*, not as *泣く, to cry*.

**Built for real subtitles, tested on real ones.** The splitting is checked line by line against anime, games and song lyrics - in **both Chrome and Firefox**, whose word breakers disagree more than you'd think. Want dictionary-grade splitting? Download the **Advanced scanning** word pack (JMdict, one click in the Dict tab) and every line is cut by a real dictionary.

**A popup that stays out of your way.** It sits pinned just above the line and grows upward, so it doesn't jump around as definitions arrive; moving across words it glides instead of teleporting. Choose how it appears - instant, fade, rise, pop or slide - and nudge its position to the pixel.

**🇯🇵 Japanese runs the full stack:** `Jitendex` · `JMdict` · `JMnedict` · `KANJIDIC` · JLPT levels · example sentences.

**🌐 Everything else runs on Yomitan-format dictionaries** - the ecosystem Yomitan users already have. 46 languages ship with a ready-to-install catalog; the few long-tail languages with no Yomitan dictionary yet are labelled as such, so you're never left guessing.

**📚 Bring your own:** `.tsv`, Yomitan `.json`, Yomitan `.zip`. Personal word lists, anime terminology, domain glossaries - Kitsumi would like to meet your dictionary.

### ✦ Explain this line

Lost the whole sentence, not just one word? Hover the subtitle and click the small star in its corner. The video pauses and a glass panel opens with the line's translation and **every word in it**, in order - reading, dictionary form, meanings, and grammar notes for the particles and endings. Click any word for its full entry. Click the star again and you're back in the episode.

---

## 🧠 Study Mode and mining

Study Mode turns the current line into a row of word cards - the same words the dictionary rows see, with furigana, and with particles and endings getting their own cards and grammar notes instead of disappearing. Mark words you already know as **memories**: they shrink to tiny chips and stop competing for attention, so whatever is still big is what's actually new.

Later, add **AnkiConnect** - the moment you want flashcards for the words you meet:

| 📝 Word | 📖 Reading | 💡 Definition | 💬 Sentence | 📸 Screenshot | 🔊 Audio | 🎬 Clip |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

Quick-mine hotkey, draft queue, configurable context. Cards are the *residue* of understanding something, not a substitute for it - mine the words you'd be annoyed to forget, not every word you saw. Future you reviews every card present you makes. Be kind to future you.

### 🎯 Comprehension target

Kitsumi can show how much of an episode is already known to you and underline unknown words, so you can pick material you understand **~90-95%** of - hard enough to learn from, easy enough to keep watching. That one setting will do more for you than any XP bar in this README.

### ⏸️ A pause that doesn't slam the brakes

Pause-on-hover stops the video while you read. If an instant cut feels harsh, pick a **smooth pause**: *Fade*, *Tape stop*, *Soft* or *Vinyl* - the sound eases out (and the tape winds down) before it stops, and fades back in when you move on. Your volume and speed always come back exactly as they were.

---

## 🤖 Optional AI · 🖱️ Beyond the player

AI is **opt-in and dormant** until you paste your own key. No key, no AI, no quiet background requests.

| Service | What it does | Setup |
| :--- | :--- | :--- |
| Groq | Cleaner definitions & example sentences | Your own API key |
| WaveSpeed | Generated scene imagery for cards | Your own API key |

**📚 Articles Reader** brings the same hover dictionary to ordinary web pages - news, Wikipedia, docs, blogs, or that Japanese site you should not have opened at 3 AM. **🖼️ OCR** (browser TextDetector or Tesseract.js) pulls text out of images, video frames and manga pages. Both opt-in.

---

## 🪶 Light on purpose

Kitsumi runs on every video page for hours, so it's built to do nothing when nothing is happening: no background polling, no timers left running, animations only on the GPU-friendly properties. The window opens straight into your theme and layout. Three performance modes - **Beauty**, **Optimal** (default) and **Super optimized** for older laptops - decide how much glass and motion you get. The interface speaks **20 languages**.

---

## 🕹️ Progression - and what it actually measures

**36 ranks**, from 🌱 Sprout to 🫀 Soul of the Language, 200+ achievements, streaks, per-language profiles, and a stats page that answers *"have I actually been doing this?"*

<p align="center"><a href="https://addons.mozilla.org/firefox/addon/Kitsumi/"><img src="https://github.com/user-attachments/assets/f7f2618a-9dcc-46b4-9968-6576e6e28413" width="900" alt="Progression, ranks and per-language statistics"></a></p>

> **Read this part honestly.** XP and ranks measure **activity, not ability**. Minutes watched and words hovered are a log of what you did, not a certificate of what you know. They exist because a visible streak is a decent reason to open the app on a bad day - that's the whole job. Level estimates (JLPT-style where a framework exists) are rough signals, not certifications. Kitsumi is not secretly your examiner.

No quests, no lives, no virtual fox whose emotional wellbeing depends on your Tuesday. It just records what happened while you were busy enjoying something - and one day you open the profile and go *"...huh. I'm actually pretty far."*

---

## 🔒 Privacy and permissions, stated plainly

| ❌ No accounts | ❌ No subscriptions | ❌ No telemetry | ❌ No analytics |
| :---: | :---: | :---: | :---: |

Your study data, mined words and settings live in your browser. Nothing goes to a Kitsumi server, because there is no Kitsumi server.

**Network requests happen only when you ask for them:** searching subtitles, downloading a dictionary, looking a word up in an online dictionary you switched on (explaining a line sends that line to MyMemory only if it's one of your sources), or an AI feature running on your own key. "No collection" is not the same as "no network", and you should be suspicious of any extension that blurs the two. The full list, service by service, is in the [privacy policy](https://kitsumi.org/privacy).

**About permissions:** the extension asks for broad site access because subtitles have to be drawn over players it can't predict, including ones inside iframes. If that's more than you want to grant, restrict it - right-click the icon → **This can read and change site data** → *On specific sites*, and allow only the streaming sites you use. Everything still works. That's a supported way to run it, not a workaround.

---

## 🚀 Get Kitsumi

<p align="center"><a href="https://addons.mozilla.org/firefox/addon/Kitsumi/"><img src="https://img.shields.io/badge/Firefox-Install-18181B?style=for-the-badge&logo=firefoxbrowser&logoColor=white&labelColor=FF7139&color=18181B" height="56" alt="Firefox Install"></a>&nbsp;&nbsp;<a href="https://chromewebstore.google.com/detail/Kitsumi/ciiembegoahhehnfdkbanhioobokjdkd"><img src="https://img.shields.io/badge/Chrome-Install-18181B?style=for-the-badge&logo=googlechrome&logoColor=white&labelColor=4285F4&color=18181B" height="56" alt="Chrome Install"></a></p>

## ❤️ Support and links

Free, no subscription, no paywalled features, built by one person and a fox. If Kitsumi saved you from subtitle suffering - or from handcrafting Anki cards like it's 2014 - you can share some love:

<p align="center"><a href="https://ko-fi.com/olexify"><img src="https://img.shields.io/badge/Ko--fi-Support-18181B?style=for-the-badge&logo=kofi&logoColor=white&labelColor=FF5E5B&color=18181B" height="44" alt="Ko-fi"></a>&nbsp;<a href="https://www.patreon.com/Olexifyyy"><img src="https://img.shields.io/badge/Patreon-Support-18181B?style=for-the-badge&logo=patreon&logoColor=white&labelColor=FF424D&color=18181B" height="44" alt="Patreon"></a>&nbsp;<a href="https://buymeacoffee.com/olexify"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Support-18181B?style=for-the-badge&logo=buymeacoffee&logoColor=white&labelColor=FFDD00&color=18181B" height="44" alt="Buy Me a Coffee"></a></p>

Bugs and feature requests go in [Issues](../../issues). Questions, recommendations and general fox business go to [Discord](https://discord.gg/UpmNHxT7PF).

---

```text
Kitsumi - status

[ OK ]   subtitle overlay · search · precision sync · auto-next
[ OK ]   two-row word splitting · part cards · explain-this-line
[ OK ]   46 dictionary languages · 20 interface languages · custom dictionaries
[ OK ]   study mode · anki mining · articles reader · OCR
[ OK ]   smooth pause · progression · statistics · privacy

[WARN]   "just one more episode"
[WARN]   user has been watching for 6 hours
[WARN]   user somehow knows 1,200 new words
[WARN]   kanji remain undefeated

[STATUS] 🦊
```

*"I-it's not like I built you an entire language-learning ecosystem disguised as a subtitle extension or anything..."* **...baka.** 🦊✨
