# Privacy Policy

**Kitsumi browser extension**
Last updated: 9 November 2026

## Summary

Kitsumi has no accounts, no servers, and no analytics. Everything it stores,
it stores in your own browser. It makes network requests only when you use a
feature that needs one, or to show this month's support total on the occasional
support reminder, and every one of those is listed below.

On a fresh install, nothing you type, hover, watch or listen to is sent
anywhere. The features that would send something are off until you turn them
on.

## What the store listings declare, and what that means

The Chrome Web Store asks every developer to tick which categories of user data
their extension **handles**. Google defines handling as "collecting,
transmitting, using, or sharing", and requires the declaration "even when data
is processed or stored locally on a user's device and is not transmitted to
external servers or third parties".

That is a much wider word than most people read into it. Reading the subtitle
line on your screen in order to draw it back with a dictionary attached is
handling, even though the line never goes anywhere. Kitsumi ticks the
categories honestly rather than picking the flattering reading, so here is what
each one actually is:

- **Website content.** The subtitle text on the page, read so the overlay can
  be drawn and so you can hover a word. That reading happens on your device.
  Two optional features then send a piece of it onward, and only the piece you
  asked about: **online dictionary lookups** send the word you hovered to the
  dictionary service (and, when you click the star to explain a line, that
  line and each of its words), and the **AI features** send the subtitle line,
  or the audio of the video, to the provider whose key you entered. Both are
  off until you switch them on, and both go to those services rather than to
  anything of Kitsumi's.
- **Authentication information.** The API keys you choose to type in, for
  Jimaku, OpenSubtitles, SubDL, Groq, OpenAI, Google Gemini, OpenRouter,
  WaveSpeed, KRDict or DeepL. They sit in
  your browser and go only to the service that issued them.
- **Personally identifiable information.** Only the email you may type in for
  MyMemory (Dict tab -> Keys, optional), which raises MyMemory's free daily
  limit. It sits in your browser and goes only to MyMemory, with its requests.
- **Web browsing activity.** The title and address of the tab you are
  watching, used to work out which show it is, and remembered per show so the
  next episode finds its subtitles. It is sent to a subtitle provider only on
  the sites you have put on your list, and only after you have accepted the
  providers notice inside the extension (see below).

**None of it reaches the developer, because there is nowhere for it to go.**
Kitsumi has no server, no account, no analytics and no telemetry. Those
categories describe what the software touches on your machine, not what anybody
collects about you. Everything below sets out exactly where each thing goes.

## What Kitsumi stores, and where

All of the following is kept locally in your browser, using extension storage
and IndexedDB. None of it is transmitted anywhere.

- Your settings: subtitle appearance, position, timing offsets, per-show sync
  offsets, interface preferences, allowlisted sites.
- Your study data: words you have looked up, words marked as known, study
  time, streaks, active days, ranks and achievements, per-language statistics.
- A safety copy of your settings and study data, made once a day and kept for 3 days, so they can be restored if the browser loses them. It has no API keys, and it is removed with the extension.
- Dictionaries you install, stored as local databases.
- Fonts you download or add for subtitles, and word packs you download for
  Advanced scanning, also stored as local databases.
- Subtitle files you load, for the duration of playback.
- Recognition data for any OCR language you have used, cached after its first
  download.
- API keys you choose to enter for optional third-party services.

You can delete all of it at any time by removing the extension, or by using
the reset controls in the extension's settings.

Subtitles you save from the subtitle timeline (the 📥 button, as .srt or plain
text) are handed to your browser as an ordinary download: a file on your
computer, which Kitsumi does not keep a copy of or send anywhere.

## When Kitsumi makes network requests

Kitsumi does not contact any server operated by the developer, because none
exists. It contacts third-party services only in response to an action you
take:

| You do this | Kitsumi contacts | What is sent |
| :--- | :--- | :--- |
| Search for subtitles, on a site you listed | Jimaku, OpenSubtitles or SubDL, whichever you have set up with your own key | The show title and page address, or the terms you typed |
| In Kitsumi's player for your own video files, you press Search under "Online" or Find online in the bar (then play an episode) | The same providers, set up with your own key | The title in that search box (the folder name, cleaned, until you change it), the id of the result you pick, and the file of the episode you play. Never your video files, their names or anything else from your computer |
| Search with a custom provider you added yourself (advanced - none exists unless you add one) | The site you added. Kitsumi does not choose, check or vouch for it | The title you search, the language code, the id of a result you open, and the key you gave it for that site - nothing else: no cookies, no page address, no referrer |
| A support reminder appears in the popup (at most once a day) | olexify.dev, the developer's own website | A plain request for this month's support total (`/goal.json`). Nothing about you is sent; like any web request, the server sees your IP address |
| The welcome page opens (after install, or from the popup's Kitsumi menu) | olexify.dev, the developer's own website | A plain request for this month's support total (`/goal.json`). Nothing about you is sent; like any web request, the server sees your IP address |
| Download a dictionary | GitHub Releases, Hugging Face and the other hosts named in the dictionary catalog | A file request. No personal data |
| Download a font in the Subs tab | raw.githubusercontent.com (the Google Fonts repository on GitHub) | A file request for that font and its licence. No personal data |
| Download a word pack for Advanced scanning in the Dict tab | raw.githubusercontent.com (Kitsumi's own public repository on GitHub, Olexify/KitsumiOPS) | A file request for that pack, and - while a pack is installed - for the list of pack versions (index.json), at most once a week when you open the Dict tab. No personal data. Subtitle lines are split on your device and never sent anywhere |
| Look up a word online, off until you turn it on | The dictionary services you selected: Jisho, Jotoba, KRDict (with your own key), Wiktionary, freedictionaryapi.com, dictionaryapi.dev or MyMemory | The word you looked up, and forms of it Kitsumi works out to find its entry: its dictionary form (食べていた → 食べる, 먹었어요 → 먹다), the word a "form of" definition names, the spelling a Wiktionary page points to (准备 → 準備), the words inside a compound no dictionary lists whole (楽園歴 → 楽園, 歴) or inside a stretch of kana read as one piece (はいもう → はい, もう), and a part of a word you hover in the popup (曇りなく → なく) |
| Explain a subtitle line (the star on the line), off until you turn online dictionaries on | The dictionary services you selected; MyMemory if it is one of them; DeepL if you entered your own DeepL API key | Each word of that line, looked up as above; and the line itself (at most 500 characters) for a translation - to MyMemory (with your email, if you entered one) and/or DeepL (with your key), in the order you chose |
| Furigana over Japanese subtitles when no Japanese dictionary is installed, off until you turn online dictionaries on (and furigana off turns it off) | The dictionary services you selected | The words of the subtitle line on screen (at most 6 per line, one at a time, only while the tab is visible and the line stays on screen), looked up as above - each word once, then remembered on that page |
| A card's sentence translation or word list (Anki drafts window: Translate / Look up each word, or the card layout asking for them when a card is sent or mined to Anki), off unless you use them | MyMemory if it is one of your online dictionaries, DeepL if you entered your own key, the AI service you chose in Anki tab -> AI cards (Groq, OpenAI, Google Gemini or OpenRouter) if you chose AI as the translator (your own key); the dictionaries you chose as flashcard dictionaries | The card's sentence (at most 500 characters) for a translation, in the order you chose; each word of that sentence (at most 10), looked up as above |
| Play a word's pronunciation | assets.languagepod101.com | The word and its reading. Kitsumi fetches the recording once to check that one exists before playing it |
| A card's word audio, off until you turn it on (Anki tab -> Card attachments -> Word audio from JapanesePod101), for a note type with a word-audio field (Lapis / Kiku ExpressionAudio, Senren wordAudio) | assets.languagepod101.com | The mined word and its reading, once per card sent to Anki. The recording goes from Kitsumi to your own Anki (AnkiConnect, on your computer) |
| Read text from an image | Nothing, for Japanese vertical text. For any other language, tessdata.projectnaptha.com | The name of the language. The picture is recognised on your device and never leaves it |
| Generate subtitles with AI, optional | Groq | The audio of the video or file you chose, plus your own Groq API key |
| AI card text, optional (Anki tab -> AI cards: the field prompts on the cards you make - never auto-mine - the Anki drafts window's "AI: write" button, and AI as the sentence translator) | The one service you chose there: Groq, OpenAI, Google Gemini or OpenRouter (OpenRouter passes it on to the model's provider you picked) | Your field prompts with the card's word, reading, subtitle line, definition and translation filled in (or the word and the line for "AI: write"), plus your own API key for that service |
| Sync across browsers, optional (Settings -> Sync across browsers; off until you say yes) | Your browser's own sync service, under your own browser account: Google (Chrome, Edge, Brave) or Mozilla (Firefox Account). Never a server of Kitsumi's | Your Memories, known words, Review and game progress and your Kitsumi settings (never API keys, dictionaries or clips), compressed, in the extension's sync storage of your account, which your browser keeps in sync between your own signed-in browsers |
| "Speak it" speaking drill, optional (Study tab -> Speak it) | The AI service you chose in Anki tab -> AI cards (Groq, OpenAI, Google Gemini or OpenRouter) | For each batch of 10 sentences: up to 6 of your saved words, the language you learn and yours, the level, topic and grammar you picked, a short summary of your recent drill mistakes (the words and what you said) and the last sentences you saw; "Why?" sends the sentence, the word and your answer; Settings -> "Test the connection" sends the word "Ping". Your own rules for a language (Settings) go with each batch for it. Plus your own API key for that service |
| "Speak it": checking a spoken answer, optional (the "Speak it" check) | Groq if you entered a Groq key, else OpenAI with your OpenAI key | The recording of your answer (at most 15 seconds) and the language, plus your own key. Nothing is recorded until you press the button |
| "Speak it": an AI voice, optional (Settings -> Voice: an OpenAI or Google Gemini voice) | OpenAI or Google Gemini, the one you picked | The sentence to be read aloud and the voice name, plus your own key. Browser voices stay on your device or go to the browser's own speech service |
| Enable AI imagery, optional (also the Anki drafts window's "AI: picture" button) | WaveSpeed | The prompt text (a one-sentence description of the scene), plus your own WaveSpeed API key |
| Check for updates (Settings -> Import / export), when you press it | Your browser's add-on store (Chrome Web Store or addons.mozilla.org), asked by the browser itself | What the browser always sends when it checks for add-on updates: Kitsumi's ID and version |
| Mine a card to Anki | AnkiConnect on `http://localhost:8765` | The card contents, including a screenshot or clip if you turned those on. This request never leaves your computer |

**Online dictionary lookups are off on a fresh install.** Until you switch them
on, every lookup is answered from the dictionaries stored on your device, with
no network request at all. You can turn them on in the popup, from the Dict
tab or the switch on its main screen; the first time, Kitsumi shows a short notice saying exactly what
is sent and to whom, and nothing is sent before you accept it. Turning every
source off again switches them back off.

**Custom subtitle providers are yours, not Kitsumi's.** In Settings, Subtitle
providers, you can add a subtitle site Kitsumi does not support (advanced). Kitsumi
shows three warnings first and adds nothing until you pass all three; it records on
your device when you accepted them. A custom provider only ever talks to the one
site you confirmed, and only over https; your key goes to that site and nowhere
else, and a request carrying it is never followed to another address. What comes
back is limited to titles, ids and file names as plain text, and subtitle files that
really are subtitles (anything else is refused, and web code in them is removed).
Everything that site receives or does is between you and it; see the licence.

**Subtitle providers need a key of your own.** Kitsumi ships no shared key.
Jimaku, OpenSubtitles and SubDL each stay dormant until you enter one, so none
of them is contacted until you decide to set it up.

**Subtitle providers are asked only on sites you list.** The automatic search
(in the background, and the one that runs when you open Kitsumi) is built from
the page's title and address, so it runs only on the sites you have added to
your list in the extension. On every other site nothing is sent to any
provider. The first time you enable a provider, turn on the background search,
or search by hand, Kitsumi shows a short notice saying exactly this and asks
you to accept it; nothing is sent to a provider before you do. Declining
switches the providers off again. Your list stays empty until you accept the
notice, and YouTube is never on it: there Kitsumi uses YouTube's own subtitle
tracks and asks no provider. Kitsumi never reads anything you type into a
page - no passwords, no forms, no messages - on any site, listed or not.

**The AI features are off by default** and stay dormant until you enter your
own API key. With no key present, no request is made to Groq, OpenAI, Google
Gemini, OpenRouter or WaveSpeed at
any time.

**About the OCR download.** Japanese vertical recognition works entirely
offline; its data ships inside the extension. Any other language downloads its
recognition data once, from tessdata.projectnaptha.com, and keeps it on your
device afterwards. The only thing sent is the name of the language. In the
Opera version of Kitsumi this also applies to Japanese, because Opera's store
does not accept that file type in a package. What is downloaded is recognition
data, not program code, and none of your images or text is uploaded for it.

Each third-party service handles the data it receives under its own privacy
policy. If you enable one of these features, you are choosing to send that
content to that provider, under your own account where a key is involved.

## Donations

Kitsumi shows optional donation options: Patreon, a Monobank Jar, Ko-fi, and crypto addresses (USDT, USDC, BTC, ETH, XMR, SOL, LTC). Donating unlocks nothing.

Showing them sends nothing. A link opens that service's own page in a new tab, and its own terms and privacy policy apply there. The addresses and QR codes ship inside the extension, and Copy address puts the address on your clipboard.

Kitsumi does not see your payment, card details or wallet. Most blockchains are public, so anyone can see a transaction to these addresses, including the developer. Only the support total above is fetched, and that request says nothing about you.

## Site access

Kitsumi requests access to all sites because subtitles have to be rendered
over video players it cannot know about in advance, including players inside
embedded frames. It reads the page only to find the video player and its
subtitle track, the word under your cursor on a site where you turned the
article reader on (it runs only on sites you add yourself), and any image you
point the OCR at. On YouTube (and wherever Kitsumi shows subtitles) the
subtitle text itself is read so its words can be hovered and looked up - with
no site to add, since that is the overlay. The rest of the page, such as titles
or comments, is read only where you added the site to the article reader.

Reading the page is how the overlay gets drawn, and it is why the store
listing declares website content. What Kitsumi does not do is keep any of it or
send it away. Page content is read, used to render the thing you are looking
at, and discarded; nothing about the pages you visit is stored beyond the show
title Kitsumi remembers so the next episode finds its subtitles.

There are two exceptions, both entirely in your hands and both off until you
switch them on:

- **Online dictionary lookups** send the word you hovered to the dictionary
  service you picked, because that is the only way it can look the word up.
  When you click the star on a subtitle to explain the whole line, each word of
  that line is looked up the same way, and the line itself goes to MyMemory for
  a translation - only if MyMemory is one of your online dictionaries.
  If you enter an email in the Dict tab (MyMemory email, optional), it is sent to
  MyMemory with each MyMemory request, which gives a higher free daily limit;
  it is kept only in your browser and sent nowhere else. Kitsumi asks before you
  type it the first time.
  If you enter your own DeepL API key (optional), the line you explain can go to
  DeepL with that key for its translation, in the order you choose (by default
  only when MyMemory's daily limit is used up); the key is kept only in your
  browser.
- **The AI features** send the subtitle line, or the audio of the video you
  asked to transcribe, to the provider whose API key you entered.

Nothing else from the page is ever transmitted, and none of it is ever stored
outside your browser.

If you would rather narrow this, both browsers let you restrict an extension
to specific sites:

- **Chrome:** right-click the extension icon, "This can read and change site
  data", "On specific sites".
- **Firefox:** Add-ons Manager, Kitsumi, Permissions.

All features continue to work on the sites you allow.

## What Kitsumi never does

- No user accounts, sign-in, or registration.
- No analytics, telemetry, crash reporting, or usage tracking.
- No advertising and no advertising identifiers.
- No cookies. Kitsumi neither sets nor reads any. When it loads a caption file or
  an image from the site you are on, your browser sends that site's own cookies
  with the request, as it does for the page itself.
- No selling or sharing of data.
- No transmission of your study history, vocabulary, or statistics anywhere.
- No sending of your API keys to anyone but the service that issued them.
- No reading of what you type into pages: passwords, forms and messages are never read, on any site.
- No contacting a subtitle provider on a site you have not listed, or before you have accepted the providers notice.

## The kitsumi.org website

Everything above is about the extension. The website where this policy is
published, kitsumi.org, is hosted on Cloudflare Workers:

- It sets no cookies, has no accounts, and shows no advertising. Its fonts and
  scripts come from kitsumi.org itself (no Google Fonts or other font
  services).
- Cloudflare, as the host, processes visitors' IP addresses and request data
  to deliver the pages and to protect the site from attacks, under
  Cloudflare's own privacy policy: https://www.cloudflare.com/privacypolicy/
- The site counts visits with Cloudflare Web Analytics. It uses no cookies and
  no fingerprinting; it records the page visited, the referring site, the
  browser type and how fast the page loaded, and reports them only as totals.
  Nothing it records is used to identify you.
- Download counter: when you download a PDF from the site, a Cloudflare D1
  table adds 1 to that file's total - the table holds only the file name and
  its count. To avoid counting the same download twice, a Cloudflare rate
  limiter looks at your IP address together with the file name for one
  minute. Kitsumi does not store your IP address, and no record is kept per
  person.
- Settings the site remembers stay in your browser and are never sent
  anywhere: in localStorage the colour theme (k-theme), the page language
  (k-lang) and a dismissed hint (k-coach); in sessionStorage the lighter
  animations choice (k-lite) and the scroll position of each page.
- Videos: the home page and /videos show a thumbnail only. The YouTube player
  (youtube-nocookie.com) loads only after you press play; from then on
  YouTube's and Google's privacy policies apply.
- Donations (/support): the links to Patreon and Monobank open their own pages,
  where their terms and privacy policies apply. The site never receives card
  details. Those services may show the developer your name and message. If
  you donate in cryptocurrency, the transaction is public on its blockchain.
- Links to the Chrome Web Store, Firefox Add-ons, GitHub, Discord and social
  sites are ordinary links: nothing loads from them until you click one.

## Children

Kitsumi is a general-purpose study tool and does not knowingly collect data
from anyone, including children.

## Changes

Material changes to this policy will be published at kitsumi.org/privacy and
in the project's repository, and its "last updated" date will change. The
version history is public in the repository.

## Contact

Questions about this policy: olexifyyy@gmail.com
Or ask in the [Discord](https://discord.gg/UpmNHxT7PF).
