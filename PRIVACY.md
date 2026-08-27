# Jabbersnap privacy policy

Effective August 26, 2026. This policy covers the Jabbersnap Mac app and the
Jabbersnap remote.

## The short version

What you record, capture, and write stays on your Mac. It goes only to the AI
services you connect with your own accounts, and to the apps you deliver
prompts to. If you leave anonymous usage statistics on, the app reports which
features and settings get used, under a random ID. It never reports what you
say, type, or copy, and no IP address or location is stored.

The app contacts the internet for exactly three things: the AI services you
configured, anonymous usage statistics (if on), and a one-time download of the
On this Mac transcription model. There is nothing else.

## Your recordings and prompts

Audio recordings, transcripts, screenshots, copied text, and prompts are
stored on your Mac. They leave it in only two ways:

- When you deliver a prompt, its content goes to the app or site you sent it
  to.
- When a feature uses an AI service you configured, the content that feature
  needs goes directly from your Mac to that service under your own API key.
  Transcribing with a Whisper (Groq) model sends the recording's audio to
  Groq. Voice Commands in Natural language mode sends the transcribed command
  text to Google Gemini. Transcribing with the On this Mac model happens
  entirely on your Mac and sends nothing.

Jabbersnap has no server of its own in any of these paths. We never receive
your recordings, transcripts, screenshots, clipboard contents, or prompts.
Your API keys are stored on your Mac and are sent only to the service each
key belongs to.

## Anonymous usage statistics

With "Share anonymous usage statistics" on (Jabbersnap settings, General),
the app reports how it is used so we can improve it:

- A random install ID, created on first launch. It is not connected to your
  name, email, or any account. "Start over" in General creates a new one.
- Feature usage: a recording finished (which transcription model, the
  transcript's length in characters, how many captures it carried), a prompt
  was delivered (to which app or site, by which method, and whether it
  worked), a voice command ran (which built-in actions, the outcome, the
  recording's length in seconds), the remote connected, remote button
  assignments changed (which kinds of actions are assigned), and the live
  transcription preview was hidden during a recording.
- A daily snapshot of the app's settings and remote button assignments, plus
  the app version and macOS version.

It never includes audio, speech, transcript text, prompt or clipboard
contents, screenshots, API keys, or any name you typed in the app, such as a
Shortcut's name.

These events are collected with PostHog (PostHog, Inc., hosted in the United
States). The project is configured to discard the sending IP address at
ingestion and to derive nothing from it, so stored events carry no IP address
and no location.

To turn it off, open Jabbersnap's settings, choose General, and turn off
"Share anonymous usage statistics". Turning it off sends one final event
recording the opt out, and after that nothing leaves your Mac.

## Questions

Open an [issue](../../issues) in this repository, or use
[private vulnerability reporting](../../security/advisories/new) for anything
security sensitive.

## Changes

This policy is updated in place. This repository's history shows every
previous version.
