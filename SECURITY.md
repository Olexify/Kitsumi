# Security Policy

## Reporting a vulnerability

If you have found a security issue in Kitsumi, please report it privately
rather than opening a public issue.

**Email:** olexifyyy@gmail.com
**Subject line:** `Kitsumi security report`

Please include:

- What the issue is, and what an attacker could do with it.
- The extension version and browser you tested on.
- Steps to reproduce, or a proof of concept.

You will get an acknowledgement within a few days. Kitsumi is maintained by
one person, so please allow reasonable time for a fix before disclosing
publicly.

## Scope

In scope:

- The extension package published on the Chrome Web Store and
  addons.mozilla.org.
- Anything that lets a webpage read extension storage, extract stored API
  keys, or run code in the extension's context.
- Anything that causes the extension to send user data somewhere it should
  not.

Out of scope:

- Vulnerabilities in third-party services the extension talks to (Jimaku,
  OpenSubtitles, SubDL, Kitsunekko, Groq, WaveSpeed, Anki). Report those to
  the service concerned.
- Issues that require the user to install a malicious extension or run
  attacker-supplied code in their own browser console.
- The extension's broad site access permission on its own. This is documented
  and necessary; see [PRIVACY.md](PRIVACY.md).

## Supported versions

Only the current published version receives fixes. Please confirm the issue
still exists on the latest release before reporting.
