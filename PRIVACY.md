# Privacy Policy

**Kitsumi browser extension**
Last updated: 28 September 2026

## Summary

Kitsumi has no accounts, no servers, and no analytics. Everything it stores,
it stores in your own browser. It makes network requests only when you use a
feature that needs one, and every one of those is listed below.

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
  asked about: **online dictionary lookups** send the single word you hovered
  to the dictionary service, and the **AI features** send the subtitle line, or
  the audio of the video, to the provider whose key you entered. Both are off
  until you switch them on, and both go to those services rather than to
  anything of Kitsumi's.
- **Authentication information.** The API keys you choose to type in, for
  Jimaku, OpenSubtitles, SubDL, Groq or WaveSpeed. They sit in your browser and
  go only to the service that issued them.
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
| Search with a custom provider you added yourself (advanced - none exists unless you add one) | The site you added. Kitsumi does not choose, check or vouch for it | The title you search, the language code, the id of a result you open, and the key you gave it for that site - nothing else: no cookies, no page address, no referrer |
| Download a dictionary | GitHub Releases, Hugging Face and the other hosts named in the dictionary catalog | A file request. No personal data |
| Download a font in the Subs tab | raw.githubusercontent.com (the Google Fonts repository on GitHub) | A file request for that font and its licence. No personal data |
| Download a word pack for Advanced scanning in the Dict tab | raw.githubusercontent.com (Kitsumi's own public repository on GitHub, Olexify/KitsumiOPS) | A file request for that pack, and - while a pack is installed - for the list of pack versions (index.json), at most once a week when you open the Dict tab. No personal data. Subtitle lines are split on your device and never sent anywhere |
| Look up a word online, off until you turn it on | The dictionary services you selected: Jisho, Jotoba, KRDict (with your own key), Wiktionary, freedictionaryapi.com, dictionaryapi.dev or MyMemory | The word you looked up, and forms of it Kitsumi works out to find its entry: its dictionary form (食べていた → 食べる, 먹었어요 → 먹다), the word a "form of" definition names, the spelling a Wiktionary page points to (准备 → 準備), or the words inside a compound no dictionary lists whole (楽園歴 → 楽園, 歴) |
| Play a word's pronunciation | assets.languagepod101.com | The word and its reading. Kitsumi fetches the recording once to check that one exists before playing it |
| Read text from an image | Nothing, for Japanese vertical text. For any other language, tessdata.projectnaptha.com | The name of the language. The picture is recognised on your device and never leaves it |
| Generate subtitles with AI, optional | Groq | The audio of the video or file you chose, plus your own Groq API key |
| Enable AI definitions, optional | Groq | The word and the subtitle line being worked on, plus your own Groq API key |
| Enable AI imagery, optional | WaveSpeed | The prompt text, plus your own WaveSpeed API key |
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
own API key. With no key present, no request is made to Groq or WaveSpeed at
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

## Site access

Kitsumi requests access to all sites because subtitles have to be rendered
over video players it cannot know about in advance, including players inside
embedded frames. It reads the page only to find the video player and its
subtitle track, the word under your cursor on a site where you turned the
article reader on (it runs only on sites you add yourself), and any image you
point the OCR at.

Reading the page is how the overlay gets drawn, and it is why the store
listing declares website content. What Kitsumi does not do is keep any of it or
send it away. Page content is read, used to render the thing you are looking
at, and discarded; nothing about the pages you visit is stored beyond the show
title Kitsumi remembers so the next episode finds its subtitles.

There are two exceptions, both entirely in your hands and both off until you
switch them on:

- **Online dictionary lookups** send the single word you hovered to the
  dictionary service you picked, because that is the only way it can look the
  word up.
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
