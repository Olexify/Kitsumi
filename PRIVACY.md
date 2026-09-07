# Privacy Policy

**Kitsumi browser extension**
Last updated: 8 September 2026

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
  be drawn and so you can hover a word. That happens on your device. It is also
  what is sent, and only the part you asked about, if you switch on an AI
  feature with your own key.
- **Authentication information.** The API keys you choose to type in, for
  Jimaku, OpenSubtitles, SubDL, Groq or WaveSpeed. They sit in your browser and
  go only to the service that issued them.
- **Web browsing activity.** The title of the tab you are watching, used to
  work out which show it is, and remembered per show so the next episode finds
  its subtitles.

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
- Subtitle files you load, for the duration of playback.
- Recognition data for any OCR language you have used, cached after its first
  download.
- API keys you choose to enter for optional third-party services.

You can delete all of it at any time by removing the extension, or by using
the reset controls in the extension's settings.

## When Kitsumi makes network requests

Kitsumi does not contact any server operated by the developer, because none
exists. It contacts third-party services only in response to an action you
take:

| You do this | Kitsumi contacts | What is sent |
| :--- | :--- | :--- |
| Search for subtitles | Jimaku, OpenSubtitles or SubDL, whichever you have set up with your own key | The show title taken from the page, or the terms you typed |
| Search for subtitles | Kitsunekko | Nothing. Kitsumi fetches its public directory index and matches your show against it on your device |
| Download a dictionary | GitHub Releases, Hugging Face and the other hosts named in the dictionary catalog | A file request. No personal data |
| Look up a word online, off until you turn it on | The dictionary service you selected | The word you looked up |
| Play a word's pronunciation | assets.languagepod101.com | The word and its reading |
| Read text from an image | Nothing, for Japanese vertical text. For any other language, tessdata.projectnaptha.com | The name of the language. The picture is recognised on your device and never leaves it |
| Generate subtitles with AI, optional | Groq | The audio of the video or file you chose, plus your own Groq API key |
| Enable AI definitions, optional | Groq | The word and the subtitle line being worked on, plus your own Groq API key |
| Enable AI imagery, optional | WaveSpeed | The prompt text, plus your own WaveSpeed API key |
| Mine a card to Anki | AnkiConnect on `http://localhost:8765` | The card contents, including a screenshot or clip if you turned those on. This request never leaves your computer |

**Online dictionary lookups are off on a fresh install.** Until you switch them
on, every lookup is answered from the dictionaries stored on your device, with
no network request at all. You can turn them on from the welcome page or in
the Dict tab, and turning every source off again switches them back off.

**Subtitle providers need a key of your own.** Kitsumi ships no shared key.
Jimaku, OpenSubtitles and SubDL each stay dormant until you enter one, so none
of them is contacted until you decide to set it up. Kitsunekko needs no key,
and it receives no search terms.

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
embedded frames. It reads the page only to find the video player, its subtitle
track, and any image you point the OCR at, and only on pages where you use it
or that you have allowlisted.

Reading the page is how the overlay gets drawn, and it is why the store
listing declares website content. What Kitsumi does not do is keep any of it or
send it away. Page content is read, used to render the thing you are looking
at, and discarded; nothing about the pages you visit is stored beyond the show
title Kitsumi remembers so the next episode finds its subtitles.

There is one exception, entirely in your hands: if you switch on an AI feature
with your own API key, the subtitle line, or the audio of the video you asked
it to transcribe, is sent to that provider so it can do the thing you asked
for. Nothing else from the page is ever transmitted, and none of it is ever
stored outside your browser.

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
- No cookies. Kitsumi neither sets nor reads any.
- No selling or sharing of data.
- No transmission of your study history, vocabulary, or statistics anywhere.
- No sending of your API keys to anyone but the service that issued them.

## Children

Kitsumi is a general-purpose study tool and does not knowingly collect data
from anyone, including children.

## Changes

Material changes to this policy will be published in this file, and its
"last updated" date will change. The version history is public in this
repository.

## Contact

Questions about this policy: olexifyyy@gmail.com
Or ask in the [Discord](https://discord.gg/UpmNHxT7PF).
